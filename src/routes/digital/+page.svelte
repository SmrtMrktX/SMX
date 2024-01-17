<script>

  import { Breadcrumb, BreadcrumbItem } from 'flowbite-svelte';


  import ExploreBtn from "$lib/Components/ExploreBtn.svelte";
  import SliderComponent from "$lib/Components/SliderComponent.svelte";
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
    <BreadcrumbItem href="/" home>Home</BreadcrumbItem>
    <BreadcrumbItem>Digital</BreadcrumbItem>
</Breadcrumb>








{#if x}
    
  <SmxLoader />

{:else}

  <SliderComponent />
  <ExploreBtn />
  
{/if}

