<script>

    import { Breadcrumb, BreadcrumbItem } from 'flowbite-svelte';
    import ComingSoon from "$lib/Components/ComingSoon.svelte";
    import SmxLoader from "$lib/Components/SmxLoader.svelte";
  
    import webappslg from "$lib/img/products/webapps.webp";
  
  
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
      <BreadcrumbItem>BEST OF</BreadcrumbItem>
  </Breadcrumb>
  
  
  
  
  
  
  {#if x}
      
    <SmxLoader />
  
  {:else}
  
    <ComingSoon />
    
  {/if}