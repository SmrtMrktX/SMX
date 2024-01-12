<script>
  import { Breadcrumb, BreadcrumbItem, Card } from 'flowbite-svelte';
  import { Button } from 'flowbite-svelte';
  import { ArrowRightOutline, ShoppingCartSolid } from 'flowbite-svelte-icons';

  import SmxLoader from "$lib/Components/SmxLoader.svelte";

  import cryptowinlg from "$lib/img/bonus/directIncome/cryptowinlg.png";
  import coinpayulg from "$lib/img/bonus/directIncome/coinpayulg.png";
  import adbtclg from "$lib/img/bonus/directIncome/adbtclg.png";
  import cryptoflarelg from "$lib/img/bonus/directIncome/cryptoflarelg.png"


  let x =true;
  const ToOther = () => {
    setTimeout(() => {
      x = false; 
    }, 700); 
  };

  ToOther();

</script>






<Breadcrumb aria-label="Default breadcrumb example" class="my-4">
  <BreadcrumbItem href="/" home>Home</BreadcrumbItem>
  <BreadcrumbItem href="/bonus">Bonus</BreadcrumbItem>
  <BreadcrumbItem>Direct Income</BreadcrumbItem>
</Breadcrumb>









{#if x}
    
  <SmxLoader />

{:else}

  <Card padding="none" size="xl" class="grid md:grid-cols-2 m-auto ">
    <figure class="flex flex-col justify-center items-center p-8 text-center bg-white rounded-t-lg border-b border-gray-200 md:rounded-t-none md:rounded-tl-lg md:border-e dark:bg-gray-800 dark:border-gray-700">
      <blockquote class="mx-auto mb-4 max-w-2xl text-gray-500 dark:text-gray-400">
        <h3 class="text-xl lg:text-2xl font-bold text-gray-900 dark:text-white">
            #1 Bitcoin Rewards Platform.<br>
            <span class="text-lg font-medium">
                Make Money by BTC Faucet, Ads
            </span>
        </h3>
        <p class="my-4 font-light">Claim upto 50 satoshi every 15 min.  BTC Faucet, view Ads,
            do Surveys/Offers, and lots more...</p>
        <Button color="green">
            <a href="https://cryptowin.io/ref/smrket" target="_blank" rel="noreferrer">CLAIM NOW</a><ArrowRightOutline class="w-3.5 h-3.5 ms-2" />
        </Button>
    </blockquote>
      
      <figcaption class="flex justify-center items-center space-x-3 rtl:space-x-reverse">
        <img class="w-9 h-9 rounded-full" src={cryptowinlg} alt="Karen profile" />
        <div class="space-y-0.5 font-medium dark:text-white text-left">
          <div>CryptoWin</div>
          <div class="text-sm font-light text-gray-500 dark:text-gray-400">Mobile | Desktop</div>
        </div>
      </figcaption>
    </figure>




    <figure class="flex flex-col justify-center items-center p-8 text-center bg-white rounded-tr-lg border-b border-gray-200 dark:bg-gray-800 dark:border-gray-700">
      <blockquote class="mx-auto mb-4 max-w-2xl text-gray-500 dark:text-gray-400">
        <h3 class="text-xl lg:text-2xl font-bold text-gray-900 dark:text-white">
            #2 Good Rewards Platform.<br>
            <span class="text-lg font-medium">
                Make Money by Views ads
            </span>
        </h3>
        <p class="my-4 font-light">
            CoinPayu a real platform, reliable with its members, the ideal site with many opportunities for you ...
        </p>
        <Button color="green">
          <a href="https://www.coinpayu.com/?r=d3j1x" target="_blank" rel="noreferrer">CLAIM NOW</a><ArrowRightOutline class="w-3.5 h-3.5 ms-2" />
      </Button>
      </blockquote>
      <figcaption class="flex justify-center items-center space-x-3 rtl:space-x-reverse">
        <img class="w-9 h-9 rounded-full" src={coinpayulg} alt="Robert profile" />
        <div class="space-y-0.5 font-medium dark:text-white text-left">
          <div>CoinPayu</div>
          <div class="text-sm font-light text-gray-500 dark:text-gray-400">Mobile | Desktop</div>
        </div>
      </figcaption>
    </figure>





    <figure class="flex flex-col justify-center items-center p-8 text-center bg-white rounded-bl-lg border-b border-gray-200 md:border-b-0 md:border-e dark:bg-gray-800 dark:border-gray-700">
      <blockquote class="mx-auto mb-4 max-w-2xl text-gray-500 dark:text-gray-400">

        <h3 class="text-xl lg:text-2xl  font-bold text-gray-900 dark:text-white">
            #3 Mixed Platform.<br>
                <span class="text-lg font-medium">
                    Money and Crypto by Views ads
                </span>
        </h3>

        <p class="my-4 font-light">
            Earn bitcoin online by viewing websites. Cheap website promotion with bitcoin payments.
        </p>
        <Button color="green">
          <a href="https://r.adbtc.top/3118297" target="_blank" rel="noreferrer">CLAIM NOW</a><ArrowRightOutline class="w-3.5 h-3.5 ms-2" />
        </Button>
      </blockquote>
      <figcaption class="flex justify-center items-center space-x-3 rtl:space-x-reverse">
        <img class="w-9 h-9 rounded-full" src={adbtclg} alt="adBTC Logo" />
        <div class="space-y-0.5 font-medium dark:text-white text-left">
          <div>adBTC</div>
          <div class="text-sm font-light text-gray-500 dark:text-gray-400">Mobile | Desktop</div>
        </div>
      </figcaption>
    </figure>








    <figure class="flex flex-col justify-center items-center p-8 text-center bg-white rounded-bl-lg border-b border-gray-200 md:border-b-0 md:border-e dark:bg-gray-800 dark:border-gray-700">
      <blockquote class="mx-auto mb-4 max-w-2xl text-gray-500 dark:text-gray-400">
        <h3 class="text-xl lg:text-2xl font-bold text-gray-900 dark:text-white">
            Awesome Btc Faucet.<br>
            <span class="text-lg font-medium">
                Money by BTC Faucet, Ads
            </span>
        </h3>
        <p class="my-4 font-light">
            Exceptional cryptocurrency web system that allows for daily investment returns directly to your balance.
        </p>
        <Button color="green">
          <a href="https://cryptoflare.net/?r=17305" target="_blank" rel="noreferrer">CLAIM NOW</a><ArrowRightOutline class="w-3.5 h-3.5 ms-2" />
        </Button>
      </blockquote>
      <figcaption class="flex justify-center items-center space-x-3 rtl:space-x-reverse">
        <img class="w-9 h-9 rounded-full" src={cryptoflarelg} alt="TraffMonetizer Logo" />
        <div class="space-y-0.5 font-medium dark:text-white text-left">
          <div>CryptoFlare</div>
          <div class="text-sm font-light text-gray-500 dark:text-gray-400">Mobile | Desktop</div>
        </div>
      </figcaption>
    </figure>

  </Card>
  
{/if}

