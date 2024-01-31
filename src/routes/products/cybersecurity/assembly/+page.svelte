<script>

    import { Breadcrumb, BreadcrumbItem } from 'flowbite-svelte';
  
    import SmxLoader from "$lib/Components/SmxLoader.svelte";
    import ComingSoon from "$lib/Components/ComingSoon.svelte";


  
  
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
        <BreadcrumbItem href="/products" linkClass='ms-1 text-sm font-medium text-gray-700 hover:text-gray-900 md:ms-2 dark:text-black dark:hover:text-white'>Products</BreadcrumbItem>
        <BreadcrumbItem href="/products/cybersecurity" linkClass='ms-1 text-sm font-medium text-gray-700 hover:text-gray-900 md:ms-2 dark:text-black dark:hover:text-white'>Cybersecurity</BreadcrumbItem>
        <BreadcrumbItem spanClass='ms-1 text-sm font-medium text-gray-500 md:ms-2 dark:text-customColorD'>Assembly</BreadcrumbItem>
    </Breadcrumb>
  
  
  
  
  
  {#if x}
      
    <SmxLoader />
  
  {:else}
  
    <ComingSoon />
  
    
  {/if}
  
  