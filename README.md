# NFT Minter Dapp for Decentralised Earth Observation Manifesto

## Developing

Once you've cloned the project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```bash
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

## Building Production

To create a production version of your app:

```bash
npm run build
```

## Preview Build

```bash
npm run preview
```

## Test Production Build

```bash
cd build
npx serve
```

## Upload Dapp to Swarm

### Build Dapp

```bash
npm run build
```

### Upload to Swarm

```bash
npm i -g @ethersphere/swarm-cli
swarm-cli upload ./build
```

or upload using [Swarm Desktop](https://www.ethswarm.org/build/desktop)
