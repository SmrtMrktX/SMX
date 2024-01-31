<script>

  import { Breadcrumb, BreadcrumbItem, GradientButton } from 'flowbite-svelte';

  import SmxLoader from "$lib/Components/SmxLoader.svelte";

  import webappslg from "$lib/img/products/webapps.webp";
  import cybersecuritylg from "$lib/img/products/cybersecurity.webp";


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
    <BreadcrumbItem spanClass='ms-1 text-sm font-medium text-gray-500 md:ms-2 dark:text-customColorD'>Products</BreadcrumbItem>
</Breadcrumb>






{#if x}
    
  <SmxLoader />

{:else}

  <img src={webappslg} class="rounded m-auto w-full max-w-3xl shadow-sm shadow-primary-customLime" alt="web apps products"/>

  <GradientButton href="/products/webApps" color="purpleToBlue" class="mx-auto my-10 font-bold">Web Applications</GradientButton>



  <img src={cybersecuritylg} class="rounded m-auto w-full max-w-3xl shadow-sm shadow-primary-customLime" alt="cybersecurity resources"/>

  <GradientButton href="/products/cybersecurity" color="greenToBlue" class="mx-auto my-10 font-bold">Cybersecurity</GradientButton>

  
{/if}
