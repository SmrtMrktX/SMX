<script>
  import { Breadcrumb, BreadcrumbItem, AccordionItem, Accordion, GradientButton } from 'flowbite-svelte';

  import SmxLoader from "$lib/Components/SmxLoader.svelte";

  let x =true;
  const ToOther = () => {
    setTimeout(() => {
      x = false; 
    }, 900); 
  };

  ToOther();
</script>






<Breadcrumb aria-label="Default breadcrumb example" class="my-4">
    <BreadcrumbItem href="/" home homeClass="inline-flex items-center text-sm font-medium text-gray-700 hover:text-gray-900 dark:text-black dark:hover:text-white">Home</BreadcrumbItem>
    <BreadcrumbItem spanClass='ms-1 text-sm font-medium text-gray-500 md:ms-2 dark:text-customColorD'>Bonus</BreadcrumbItem>
</Breadcrumb>






{#if x}
    
  <SmxLoader />

{:else}

  <div class="justify-center items-center my-auto lg:text-center">
    
    <Accordion>
      
      <AccordionItem>
        <span slot="header">Passive Income</span>
        <p class="mb-2 text-gray-500 dark:text-gray-400">
          Passive income is any money earned in a manner that does not require too much effort.<br>
          <span class="flex justify-center items-center pt-5">
            <GradientButton color="greenToBlue">
              <a href="/bonus/passiveIncome" class="">get started</a></GradientButton>
          </span>
        </p>
      </AccordionItem>

      <AccordionItem transitionParams={{ duration: 2000 }}>
        <span slot="header">Direct Income</span>
        <p class="mb-2 text-gray-500 dark:text-gray-400">
          Direct income is the money that is received from doing tasks directly related to your business to make money.<br>
          Like Ads, Manual Faucets ...
          <span class="flex justify-center items-center pt-5">
            <GradientButton color="greenToBlue">
              <a href="/bonus/directIncome" class="">get started</a></GradientButton>
          </span>
        </p>
      </AccordionItem>

      <AccordionItem transitionType="fade" transitionParams={{ duration: 1000 }}>
        <span slot="header">Other</span>
        <p class="mb-2 text-gray-500 dark:text-gray-400">Mining, Trading, Investing.<br>
          Coming Soon ...
        </p>
      </AccordionItem>

    </Accordion>
  </div>
  
{/if}



