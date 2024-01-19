<script>

  import { Breadcrumb, BreadcrumbItem, GradientButton } from 'flowbite-svelte';

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
    <BreadcrumbItem>Products</BreadcrumbItem>
</Breadcrumb>






{#if x}
    
  <SmxLoader />

{:else}

  <img src={webappslg} class="rounded m-auto w-full max-w-3xl shadow-sm shadow-primary-customLime" alt="web apps products"/>

  <GradientButton href="/products/webApps" color="purpleToBlue" class="m-auto font-bold">Web Applications</GradientButton>

  
{/if}
