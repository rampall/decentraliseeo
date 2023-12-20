<script lang="ts">
    import { onMount } from 'svelte'
    import { writable } from 'svelte/store';
    import {
      defaultEvmStores as evm,
      connected,
      provider,
      chainId,
      chainData,
      signer,
      signerAddress,
      contracts,
      allChainsData
    } from "ethers-svelte"
  
    // import { Balance } from 'svelte-web3/components'
  
    import { abi } from '$lib/abi'

    const NFT_CONTRACT = '0x35f214397589bed07066839a51c5e1fe9da02f5b';
    const ALREADY_SIGNED_MESSAGE = "You've already signed the Manifesto!"
  
    let isLoading = writable(false);
    let balance = writable('');
    let name = writable('');
    let message = writable('');
    let success = writable(false);
    let totalSigned = writable(0);
    let tx = writable('0x166d3440522b44ccbeff02c580a008eebdb917182435a180945da486dc860db2');
  
    onMount(async () => {
      // console.log({ abi });
      window.onerror = (message, url, line) => {
        // console.log({ message, url, line })
      }
    })
  
    async function connect() {
      $isLoading = true;
      await evm.setProvider();
      await evm.attachContract('DEOManifesto', NFT_CONTRACT, abi);
      // console.log({ $signer, $chainId, $contracts, $signerAddress })
      // console.log($contracts.DEOManifesto.methods().call())
      $isLoading = false;
    }
  
    async function mintNFT() {
      $isLoading = true;
      await evm.setProvider();
      $totalSigned = await $contracts.DEOManifesto.totalSigned()
      // console.log({ $totalSigned })
      // let balance = await $contracts.DEOManifesto.balanceOf($signerAddress)
      try {
        const mintTx = await $contracts.DEOManifesto.mint(0);
        mintTx.wait(10).then((receipt) => {
          // console.log({ mintTx, receipt, $isLoading })
          $tx = receipt.hash;
          $isLoading = false;
        });
        $success = true;
      } catch (e) {
        // console.log({ e })
        $message = (e.reason || '').trim() == 'ALREADY_SIGNED' ? ALREADY_SIGNED_MESSAGE : e.reason
        $isLoading = false;
      } 
      // console.log({$success,$message})
    }
  </script>
  <style>button:disabled{opacity: 0.5;}</style>
<div class="lg:col-span-6 lg:col-start-7 text-[17px] leading-[24px]">
    {#if $message != ALREADY_SIGNED_MESSAGE}
    <p>
        Receive an NFT on Polygon as proof of signing:
    </p>
    {/if}
    {#if !$connected}
    <div class="mt-5">
        <button href="#"  on:click={connect} disabled={$isLoading}
          class="bg-[#02FF9B] px-4 text-sm h-8 rounded-full inline-flex items-center font-semibold hover:bg-opacity-80 duration-200">Connect Wallet
          -></button>
    </div>
    {:else}
        {#if $chainId == 137}
            {#if $success}
            <div class="mt-5">
              <p class="font-bold">🎉 Congratulations! Your NFT has been minted.</p>
              <p class="mt-5">
              <a target="_blank" class="bg-[#02FF9B] px-4 text-sm h-8 rounded-full inline-flex items-center font-semibold hover:bg-opacity-80 duration-200 disabled:opacity-25" 
                  href="https://opensea.io/assets/matic/{NFT_CONTRACT}/{$totalSigned}">Checkout your NFT on Opensea -></a>
              </p>
            </div>
            {:else if ['rejected',''].includes($message)}
                <div class="mt-5">
                    <button on:click={mintNFT} disabled={$isLoading} href="#"
                    class="bg-[#02FF9B] px-4 text-sm h-8 rounded-full inline-flex items-center font-semibold hover:bg-opacity-80 duration-200 disabled:opacity-25">Sign
                    -></button>
                </div>
            {:else}
                <div class="">
                    <p class="font-bold">{$message}</p>
                    {#if $message == ALREADY_SIGNED_MESSAGE}
                    <p class="mt-5">
                    <a target="_blank" class="bg-[#02FF9B] px-4 text-sm h-8 rounded-full inline-flex items-center font-semibold hover:bg-opacity-80 duration-200 disabled:opacity-25" 
                    href="https://opensea.io/{$signerAddress}?search[chains][0]=MATIC&search[query]=Decentralised%20Earth%20Observation%20Manifesto">Checkout your NFT on Opensea -></a>
                  </p>
                    {/if}
                </div>
            {/if}
        {:else}
            <div class="mt-5">
            <p class="font-bold">Connected to wrong network. Please switch to Polygon!</p>
            </div>
        {/if}
    {/if}
  </div>
