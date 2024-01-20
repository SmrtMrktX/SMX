<script>

  import { Breadcrumb, BreadcrumbItem } from 'flowbite-svelte';
  import ComingSoon from "$lib/Components/ComingSoon.svelte";

  import SmxLoader from "$lib/Components/SmxLoader.svelte";
  import penetrationtestingslg from "$lib/img/services/penetrationtesting.webp";


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
    <BreadcrumbItem spanClass='ms-1 text-sm font-medium text-gray-500 md:ms-2 dark:text-customColorD'>Services</BreadcrumbItem>
</Breadcrumb>





{#if x}
    
  <SmxLoader />

{:else}

  <img src={penetrationtestingslg} class="rounded m-auto w-full max-w-3xl shadow-sm shadow-primary-customLime" alt="web apps products"/>

  <ComingSoon />
  
{/if}

