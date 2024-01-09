<script>
    import { Breadcrumb, BreadcrumbItem } from 'flowbite-svelte';
    import ComingSoon from "$lib/Components/ComingSoon.svelte";
    import SmxLoader from "$lib/Components/SmxLoader.svelte";

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
    <BreadcrumbItem>Products</BreadcrumbItem>
</Breadcrumb>






{#if x}
    
<SmxLoader />

{:else}
  
<ComingSoon />
  
{/if}
