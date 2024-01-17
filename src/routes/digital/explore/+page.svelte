<script>

    import { Breadcrumb, BreadcrumbItem } from 'flowbite-svelte';
    import { Card, Button, Indicator, Badge  } from 'flowbite-svelte';
    import { ArrowRightOutline } from 'flowbite-svelte-icons';
  
  
    import SmxLoader from "$lib/Components/SmxLoader.svelte";

    import bitcoinlg from "$lib/img/digital/explore/icons/bitcoinlg.svg";
    import ethereumlg from "$lib/img/digital/explore/icons/ethereumlg.svg";
    import tetherlg from "$lib/img/digital/explore/icons/tetherlg.svg";
    import binancelg from "$lib/img/digital/explore/icons/binancelg.svg";
    import solanalg from "$lib/img/digital/explore/icons/solanalg.svg";
    import xrplg from "$lib/img/digital/explore/icons/xrplg.svg";
    import usdclg from "$lib/img/digital/explore/icons/usdclg.svg";
    import cardanolg from "$lib/img/digital/explore/icons/cardanolg.svg";
    import avaxlg from "$lib/img/digital/explore/icons/avaxlg.svg";
    import dogecoinlg from "$lib/img/digital/explore/icons/dogecoinlg.svg";


  
    let x =true;
    const ToOther = () => {
      setTimeout(() => {
        x = false; 
      }, 900); 
    };
  
    ToOther();
  
  </script>
  
  
  
  
  
  
  
  <Breadcrumb aria-label="Default breadcrumb example" class="my-4">
      <BreadcrumbItem href="/" home>Home</BreadcrumbItem>
      <BreadcrumbItem href="/digital">Digital</BreadcrumbItem>
      <BreadcrumbItem >Explore</BreadcrumbItem>
  </Breadcrumb>
  
  
  
  
  
  
  
  
{#if x}
      
    <SmxLoader />
  
{:else}

  <h1 style="font-family: 'Russo One', sans-serif;" class="mx-auto my-5  text-2xl md:text-3xl lg:text-4xl">
      Blockchain 
      <span  class="text-purple-700">
        Explorer
      </span>
  </h1>
  
  
  <div 
  class="font-extrabold min-w-full min-h-full mx-auto my-6 py-8 grid grid-cols-2 gap-10 md:grid-cols-3 lg:grid-cols-5 justify-center items-center text-center border-y-4">
    
    <Card class="col-span-2 lg:col-span-5 m-auto">
      <h5 class="mb-2 text-3xl font-bold tracking-tight text-gray-900 dark:text-white">TOP 10 Crypto</h5>
      <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight">January 2024</p>
      
    </Card>

    <Card class="bg-transparent backdrop-blur-sm dark:bg-transparent dark:backdrop-blur-md m-auto">
      <img src={bitcoinlg} class="mx-auto h-12  md:h-14 lg:h-16  rounded-md hover:scale-105 hover:invert" alt="Bitcoin Logo"/>
      <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Bitcoin</h5>
      <h1>BTC</h1>
      <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight">since 2008</p>
      <Badge color="green" rounded class="">
        <Indicator color="green" size="xs" class="me-1" />
        <h2 class="text-sm text-black dark:text-white">Live</h2>
      </Badge>
      <Button color="blue" class="w-fit mx-auto my-3">
        <a href="https://www.blockchain.com/explorer" target="_blank">Explorer</a> <ArrowRightOutline class="w-3.5 h-3.5 ms-2 text-white" />
      </Button>
    </Card>


    <Card class="bg-transparent backdrop-blur-sm dark:bg-transparent dark:backdrop-blur-md m-auto">
      <img src={ethereumlg} class="mx-auto h-12  md:h-14 lg:h-16  rounded-md hover:scale-105 hover:invert" alt="Ethereum Logo"/>
      <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Ethereum</h5>
      <h1>ETH</h1>
      <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight">since 2013</p>
      <Badge color="green" rounded class="">
        <Indicator color="green" size="xs" class="me-1" />
        <h2 class="text-sm text-black dark:text-white">Live</h2>
      </Badge>
      <Button color="blue" class="w-fit mx-auto my-3">
        <a href="https://etherscan.io/" target="_blank">Explorer</a> <ArrowRightOutline class="w-3.5 h-3.5 ms-2 text-white" />
      </Button>
    </Card>


    <Card class="bg-transparent backdrop-blur-sm dark:bg-transparent dark:backdrop-blur-md m-auto">
      <img src={tetherlg} class="mx-auto h-12  md:h-14 lg:h-16  rounded-md hover:scale-105 hover:invert" alt="Tether Logo"/>
      <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Tether</h5>
      <h1>USDT</h1>
      <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight">since 2014</p>
      <Badge color="green" rounded class="">
        <Indicator color="green" size="xs" class="me-1" />
        <h2 class="text-sm text-black dark:text-white">Live</h2>
      </Badge>
      <Button color="blue" class="w-fit mx-auto my-3">
        <a href="https://www.oklink.com/usdt" target="_blank">Explorer</a> <ArrowRightOutline class="w-3.5 h-3.5 ms-2 text-white" />
      </Button>
    </Card>


    <Card class="bg-transparent backdrop-blur-sm dark:bg-transparent dark:backdrop-blur-md m-auto">
      <img src={binancelg} class="mx-auto h-12  md:h-14 lg:h-16  rounded-md hover:scale-105 hover:invert" alt="Binance Logo"/>
      <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Binance</h5>
      <h1>BNB</h1>
      <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight">since 2017</p>
      <Badge color="green" rounded class="">
        <Indicator color="green" size="xs" class="me-1" />
        <h2 class="text-sm text-black dark:text-white">Live</h2>
      </Badge>
      <Button color="blue" class="w-fit mx-auto my-3">
        <a href="https://explorer.bnbchain.org/" target="_blank">Explorer</a> <ArrowRightOutline class="w-3.5 h-3.5 ms-2 text-white" />
      </Button>
    </Card>


    <Card class="bg-transparent backdrop-blur-sm dark:bg-transparent dark:backdrop-blur-md m-auto">
      <img src={solanalg} class="mx-auto h-12  md:h-14 lg:h-16  rounded-full hover:scale-105 hover:invert" alt="Solana Logo"/>
      <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Solana </h5>
      <h1>SOL</h1>
      <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight">since 2020</p>
      <Badge color="green" rounded class="">
        <Indicator color="green" size="xs" class="me-1" />
        <h2 class="text-sm text-black dark:text-white">Live</h2>
      </Badge>
      <Button color="blue" class="w-fit mx-auto my-3">
        <a href="hhttps://explorer.solana.com/" target="_blank">Explorer</a> <ArrowRightOutline class="w-3.5 h-3.5 ms-2 text-white" />
      </Button>
    </Card>


    <Card class="bg-transparent backdrop-blur-sm dark:bg-transparent dark:backdrop-blur-md m-auto">
      <img src={xrplg} class="mx-auto h-12  md:h-14 lg:h-16  rounded-full bg-white hover:scale-105 hover:invert" alt="XRP Logo"/>
      <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">XRP</h5>
      <h1>XRP</h1>
      <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight">since 2012</p>
      <Badge color="green" rounded class="">
        <Indicator color="green" size="xs" class="me-1" />
        <h2 class="text-sm text-black dark:text-white">Live</h2>
      </Badge>
      <Button color="blue" class="w-fit mx-auto my-3">
        <a href="https://xrpscan.com/" target="_blank">Explorer</a> <ArrowRightOutline class="w-3.5 h-3.5 ms-2 text-white" />
      </Button>
    </Card>


    <Card class="bg-transparent backdrop-blur-sm dark:bg-transparent dark:backdrop-blur-md m-auto">
      <img src={usdclg} class="mx-auto h-12  md:h-14 lg:h-16  rounded-md hover:scale-105 hover:invert" alt="USDC Logo"/>
      <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">USDC</h5>
      <h1>USDC</h1>
      <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight">since 2018</p>
      <Badge color="green" rounded class="">
        <Indicator color="green" size="xs" class="me-1" />
        <h2 class="text-sm text-black dark:text-white">Live</h2>
      </Badge>
      <Button color="blue" class="w-fit mx-auto my-3">
        <a href="https://etherscan.io/token/0xa0b86991c6218b36c1d19d4a2e9eb0ce3606eb48" target="_blank">Explorer</a> <ArrowRightOutline class="w-3.5 h-3.5 ms-2 text-white" />
      </Button>
    </Card>


    <Card class="bg-transparent backdrop-blur-sm dark:bg-transparent dark:backdrop-blur-md m-auto">
      <img src={cardanolg} class="mx-auto h-12  md:h-14 lg:h-16  rounded-md hover:scale-105 hover:invert" alt="Cardano Logo"/>
      <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Cardano</h5>
      <h1>ADA</h1>
      <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight">since 2017</p>
      <Badge color="green" rounded class="">
        <Indicator color="green" size="xs" class="me-1" />
        <h2 class="text-sm text-black dark:text-white">Live</h2>
      </Badge>
      <Button color="blue" class="w-fit mx-auto my-3">
        <a href="https://explorer.cardano.org/en" target="_blank">Explorer</a> <ArrowRightOutline class="w-3.5 h-3.5 ms-2 text-white" />
      </Button>
    </Card>


    <Card class="bg-transparent backdrop-blur-sm dark:bg-transparent dark:backdrop-blur-md m-auto">
      <img src={avaxlg} class="mx-auto h-12  md:h-14 lg:h-16  rounded-full bg-white hover:scale-105 hover:invert" alt="Avalanche Logo"/>
      <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Avalanche</h5>
      <h1>AVAX</h1>
      <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight">since 2021</p>
      <Badge color="green" rounded class="">
        <Indicator color="green" size="xs" class="me-1" />
        <h2 class="text-sm text-black dark:text-white">Live</h2>
      </Badge>
      <Button color="blue" class="w-fit mx-auto my-3">
        <a href="https://subnets.avax.network/" target="_blank">Explorer</a> <ArrowRightOutline class="w-3.5 h-3.5 ms-2 text-white" />
      </Button>
    </Card>

    <Card class="bg-transparent backdrop-blur-sm dark:bg-transparent dark:backdrop-blur-md m-auto">
      <img src={dogecoinlg} class="mx-auto h-12  md:h-14 lg:h-16  rounded-md hover:scale-105 hover:invert" alt="Dogecoin Logo"/>
      <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Dogecoin</h5>
      <h1>DOGE</h1>
      <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight">since 2013</p>
      <Badge color="green" rounded class="">
        <Indicator color="green" size="xs" class="me-1" />
        <h2 class="text-sm text-black dark:text-white">Live</h2>
      </Badge>
      <Button color="blue" class="w-fit mx-auto my-3">
        <a href="https://dogechain.info/" target="_blank">Explorer</a> <ArrowRightOutline class="w-3.5 h-3.5 ms-2 text-white" />
      </Button>
    </Card>
  </div>
{/if}





<style>

</style>