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
    <BreadcrumbItem href="/" home homeClass="inline-flex items-center text-sm font-medium text-gray-700 hover:text-gray-900 dark:text-black dark:hover:text-white">Home</BreadcrumbItem>
    <BreadcrumbItem spanClass='ms-1 text-sm font-medium text-gray-500 md:ms-2 dark:text-customColorD'>Digital</BreadcrumbItem>
</Breadcrumb>








{#if x}
    
  <SmxLoader />

{:else}

  <SliderComponent />
  <ExploreBtn />
  
{/if}

