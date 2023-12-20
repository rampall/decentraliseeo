<script lang=""ts>
 import Sign from '$lib/Sign.svelte'
</script>
<main class="relative z-20 mt-32 mb-52">
  <div class="grid lg:grid-cols-12 lg:gap-x-[30px] mx-auto max-w-7xl px-5 lg:px-8 relative">

    <div class="lg:col-span-7 text-[#141516]">
      <h1 class="font-bold text-[64px] leading-[72px] tracking-[-0.64px]">Decentralised EO Manifesto</h1>
      <div class="text-[19px] leading-[26px] mt-6">
        <p>In the vein of collaboration between the Web3 and Earth Observation (EO) communities, we articulate our
          ethos
          for the convergence of blockchain, AI, and EO.</p>
      </div>


      <div class="flex items-center gap-10 mt-12">
        <a href="https://www.ethswarm.org/" target="_blank"><span class="sr-only">Ethswarm</span><img class="h-[50px]"
            src="./swarm.png" alt="" /></a>
        <a href="https://philab.esa.int/" target="_blank"><span class="sr-only">esa</span><img class="h-[72px]"
            src="./esa.png" alt="" /></a>
      </div>
    </div>
  </div>

  <div>
    <img class="w-full mx-auto mt-24 rounded-xl max-w-7xl"
      style="filter: drop-shadow(0px 10px 80px rgba(0, 0, 0, 0.13));" src="./post.png" alt="" />
  </div>

  <div class="lg:grid lg:grid-cols-12 lg:gap-x-[30px] mx-auto max-w-7xl px-5 lg:px-8 mt-36 lg:gap-y-[60px] space-y-8">
    <h2 class="lg:col-span-6 text-[48px] font-bold tracking-[-0.48px]">Premises</h2>
    <div class="hidden lg:block lg:col-span-6"></div>

    <div class="lg:col-span-5">
      <h3 class="text-[32px] font-semibold">
        Data integrity and trust
      </h3>
    </div>
    <div class="lg:col-span-6 lg:col-start-7 text-[17px] leading-[24px]">
      <p>
        We emphasise the importance of keeping Earth Observation data accurate, trustworthy and verifiable.
        Decentralised technologies play a key role here, making sure that the data we get from remote sensing is
        correct and secure.
      </p>
    </div>

    <div class="lg:col-span-5">
      <h3 class="text-[32px] font-semibold">
        Data ownership, security and selective disclosure
      </h3>
    </div>
    <div class="lg:col-span-6 lg:col-start-7 text-[17px] leading-[24px]">
      <p>
        We believe in the power of data ownership. People and organisations should retain ownership and/or control
        over the data, and be able to choose what they share. ​​European Space Agency data cannot be recorded, only
        accessed on a per-need basis, enabling utilisation without appropriation. Moreover, the European Space Agency
        controls the context in which its data are produced and processed and how that context is activated.
      </p>
    </div>

    <div class="lg:col-span-5">
      <h3 class="text-[32px] font-semibold">
        Empowerment through technology
      </h3>
    </div>
    <div class="lg:col-span-6 lg:col-start-7 text-[17px] leading-[24px]">
      <p>
        We highlight how emerging technologies, including blockchain and AI, can make Earth Observation more powerful.
        These technologies help us keep the data safe and share it transparently.
      </p>
    </div>

    <div class="lg:col-span-5">
      <h3 class="text-[32px] font-semibold">
        Commitment to building solutions
      </h3>
    </div>
    <div class="lg:col-span-6 lg:col-start-7 text-[17px] leading-[24px]">
      <p>
        In line with the proactive spirit of problem-solving, we are committed to developing and implementing systems
        that keep Earth Observation data accurate, trustworthy, verifiable and shareable, while at the same time
        giving researchers and organisations data ownership.
      </p>
    </div>

    <div class="lg:col-span-5">
      <h3 class="text-[32px] font-semibold">
        Advocacy for open data
      </h3>
    </div>
    <div class="lg:col-span-6 lg:col-start-7 text-[17px] leading-[24px]">
      <p>
        We stand for the free flow of information. While we ensure that the data is reliable and private, we also
        believe in the importance of openly sharing information
      </p>
    </div>




  </div>

  <div class="lg:grid lg:grid-cols-12 lg:gap-x-[30px] mx-auto max-w-7xl px-5 lg:px-8 mt-36 lg:gap-y-[60px] space-y-8">
    <h2 class="lg:col-span-6 text-[48px] font-bold tracking-[-0.48px] mb-10 lg:mb-0">Challenges</h2>
    <div class="lg:col-span-6"></div>

    <div class="lg:col-span-5">
      <h3 class="text-[32px] font-semibold">
        Data integrity and accessibility
      </h3>
    </div>
    <div class="lg:col-span-6 lg:col-start-7 text-[17px] leading-[24px]">
      <p>
        Ensuring that the output of AI models is not corrupted, maintaining secure communication and ensuring data
        availability.
      </p>
    </div>

    <div class="lg:col-span-5">
      <h3 class="text-[32px] font-semibold">
        Powerful, verifiable storage
      </h3>
    </div>
    <div class="lg:col-span-6 lg:col-start-7 text-[17px] leading-[24px]">
      <p>
        Addressing the need for massive storage capacity, privacy, data provenance, trustless computation, data
        provenance, and the need for verifiable data in legal or critical decision-making scenarios. This includes
        leveraging decentralised networks and implementing for transparent tracking and validation of model
        development, ensuring that each phase of research, from data collection to model output, is authenticated and
        traceable in a tamper-proof ledger
      </p>
    </div>

    <div class="lg:col-span-5">
      <h3 class="text-[32px] font-semibold">
        Tokenisation of EO Data
      </h3>
    </div>
    <div class="lg:col-span-6 lg:col-start-7 text-[17px] leading-[24px]">
      <p>
        Challenges include establishing ownership, transforming data into assets, standardising data to reduce
        friction, and designing and aligning incentives for data sharing and research.
      </p>
    </div>
  </div>

  <div class="lg:grid lg:grid-cols-12 lg:gap-x-[30px] mx-auto max-w-7xl px-5 lg:px-8 mt-36 lg:gap-y-[60px] space-y-8">
    <h2 class="lg:col-span-6 text-[48px] font-bold tracking-[-0.48px] mb-10 lg:mb-0">Vision</h2>
    <div class="lg:col-span-6"></div>

    <div class="lg:col-span-5">
      <h3 class="text-[32px] font-semibold">
        A foundation for future technologies and data-centered
      </h3>
    </div>
    <div class="lg:col-span-6 lg:col-start-7 text-[17px] leading-[24px] space-y-6">
      <p>
        We envision creating a system where EO data is beyond reproach, fostering an environment of trust not just
        among experts but also in the public domain. This aims to break down barriers, making crucial EO data
        accessible to a broader audience, empowering individuals, communities and organisations to make informed
        decisions based on reliable data.
      </p>

      <p>
        In line with the ethos of the Web3 ecosystem, we envision a future where EO data empower public goods,
        accessible and beneficial to all.
      </p>

      <p>
        We aim to ay down a foundation that will not only support current technological needs but also adapt and
        evolve with future advancements, ensuring long-term sustainability and relevance and positive social impact.
      </p>
    </div>
  </div>

  <div class="lg:grid lg:grid-cols-12 lg:gap-x-[30px] mx-auto max-w-7xl px-5 lg:px-8 mt-36 lg:gap-y-[60px] space-y-8">
    <h2 class="lg:col-span-6 text-[48px] font-bold tracking-[-0.48px] mb-10 lg:mb-0">Next steps</h2>
    <div class="lg:col-span-6"></div>

    <div class="lg:col-span-5">
      <h3 class="text-[32px] font-semibold">
        Joining forces
      </h3>
    </div>
    <div class="lg:col-span-6 lg:col-start-7 text-[17px] leading-[24px]">
      <p>
        Initiate a call for proposals to fund research and development projects that align with the integration of
        blockchain, decentralised storage, AI and Earth Observation (EO) data. Establish bounties to encourage the
        development of solutions and innovations that address specific challenges identified in the workshops.
      </p>
    </div>

    <div class="lg:col-span-5">
      <h3 class="text-[32px] font-semibold">
        Sharing resources
      </h3>
    </div>
    <div class="lg:col-span-6 lg:col-start-7 text-[17px] leading-[24px]">
      <p>
        Schedule regular meetings with research fellows to monitor progress, discuss challenges and align ongoing
        research with the workshop's objectives.
      </p>
    </div>

    <div class="lg:col-span-5">
      <h3 class="text-[32px] font-semibold">
        Promotion and community engagement
      </h3>
    </div>
    <div class="lg:col-span-6 lg:col-start-7 text-[17px] leading-[24px]">
      <p>
        Actively promote the findings and discussions from the workshops to a broader audience, including
        stakeholders, industry partners, and academic institutions. Develop and distribute demonstrations or
        prototypes that showcase the practical applications of integrating blockchain, AI and EO data. Engage with
        open source communities to help in developing offline data formats and other relevant technologies.
      </p>
    </div>

    <div class="lg:col-span-5">
      <h3 class="text-[32px] font-semibold">
        Exploring real AI use cases with federated learning
      </h3>
    </div>
    <div class="lg:col-span-6 lg:col-start-7 text-[17px] leading-[24px]">
      <p>
        Investigate practical applications of AI in the context of federated learning, particularly in the management
        and analysis of EO data.
      </p>
    </div>

    <div class="lg:col-span-5">
      <h3 class="text-[32px] font-semibold">
        Defining collaborative projects between Swarm Foundation and Φ-Lab
      </h3>
    </div>
    <div class="lg:col-span-6 lg:col-start-7 text-[17px] leading-[24px]">
      <p>
        Establish specific collaborative projects between the Swarm Foundation and ESA's Φ-Lab, focusing on the
        integration of decentralised storage solutions and federated learning in EO data processing. These projects
        will involve other Web3 players that took part in the workshop.
      </p>
    </div>


    <div class="my-36 h-px bg-[#2D384326] w-full col-span-12 relative">
      <div class="absolute inset-0 w-2/3 mx-auto"
        style="background: linear-gradient(90deg, rgba(95, 109, 124, 0.00) 0%, #778797 51.56%, rgba(95, 109, 124, 0.00) 100%);">
      </div>
    </div>

    <div class="lg:col-span-5">
      <h3 class="text-[32px] font-semibold text-black/60">
        List of workshop participants
      </h3>
    </div>
    <div class="lg:col-span-6 lg:col-start-7 text-[16px] leading-[24px] text-black/60">
      <ol class="list-decimal list-inside">
        <li>Costanza Gallo, Head of Partnerships, Swarm Foundation</li>
        <li>Gregor Žavcer, Director at Swarm Foundation</li>
        <li>Črt Ahlin, Ops, Research, Swarm Foundation </li>
        <li>Niki Papadatou, Product Owner, Swarm Foundation</li>
        <li>Elad Verbin, Lead Scientist & Founding Partner at Lunar Ventures</li>
        <li>Paolo Rollo, Founder, Brian AI</li>
        <li>Tadej Fius, CTO Datafund</li>
        <li>Marco Mosh (Grendel)i, Director, Polygon Labs</li>
        <li>Muhammed Tanrıkulu, Developer, ENS Labs</li>
        <li>Nicolas Longepe, EO Data Scientist, ESA </li>
        <li>Alessandro Sebastianelli, Research Fellow, ESA </li>
        <li>Sabrina Ricci, AI Ecosystem Manager, ESA </li>
        <li>Peter Naylor, Research Fellow, ESA</li>
        <li>Mikolaj Czerkawski, Research Fellow, ESA </li>
        <li>Nikoalaos Dionelis, Research Fellow, ESA </li>
        <li>Claudio Iacopino, EO Digital Platform Engineer, ESA </li>
        <li>Roberto Alacevich, EO Services Coordinator, ESA </li>
        <li>Mattia Stipa, EO service manager, ESA</li>
        <li>Andrea Della Vecchia, EO Data Access System Engineer, ESA </li>
        <li>Albin Lacroix, Incubed Project Manager, ESA</li>
        <li>Giuseppe Borghi, Head of Φ-lab Division, ESA </li>
        <li>Robert Cowlishaw, Researcher, University of Strathclyde</li>
        <li>Mihaela Violeta Gheorghe, Project Manager, GMV</li>
        <li>Derek Ding, Co-founder, Orbuculum (DLTEO GmbH)</li>
        <li>Red Boumghar, CEO and Founder @ Parametry.ai</li>

      </ol>
    </div>
    <div class="my-36 h-px bg-[#2D384326] w-full col-span-12 relative">
      <div class="absolute inset-0 w-2/3 mx-auto"
        style="background: linear-gradient(90deg, rgba(95, 109, 124, 0.00) 0%, #778797 51.56%, rgba(95, 109, 124, 0.00) 100%);">
      </div>
    </div>
  </div>

  <div class="lg:grid lg:grid-cols-12 lg:gap-x-[30px] mx-auto max-w-7xl px-5 lg:px-8 mt-36 lg:gap-y-[60px] space-y-8">
    <h2 class="lg:col-span-6 text-[48px] font-bold tracking-[-0.48px] mb-10 lg:mb-0">Sign</h2>
    <div class="lg:col-span-6"></div>

    <div class="lg:col-span-5">
      <h3 class="text-[32px] font-semibold">
        Sign the Decentralised Earth Observation Manifesto
      </h3>
    </div>
    <Sign></Sign>
  </div>
</main>
