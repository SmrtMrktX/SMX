<script>

    import { Breadcrumb, BreadcrumbItem, Timeline, TimelineItem, Button } from 'flowbite-svelte';
    import { ArrowRightOutline } from 'flowbite-svelte-icons';
  
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
        <BreadcrumbItem href="/products" linkClass='ms-1 text-sm font-medium text-gray-700 hover:text-gray-900 md:ms-2 dark:text-black dark:hover:text-white'>Products</BreadcrumbItem>
        <BreadcrumbItem href="/products/cybersecurity" linkClass='ms-1 text-sm font-medium text-gray-700 hover:text-gray-900 md:ms-2 dark:text-black dark:hover:text-white'>Cybersecurity</BreadcrumbItem>
        <BreadcrumbItem spanClass='ms-1 text-sm font-medium text-gray-500 md:ms-2 dark:text-customColorD'>Assembly</BreadcrumbItem>
    </Breadcrumb>
  
  
  
  
  
  {#if x}
      
    <SmxLoader />
  
  {:else}


    <Timeline class="m-auto">

      <TimelineItem title="01 Numbering System">
        <p class="mb-4 text-base font-normal text-gray-500 dark:text-gray-400">Numbering System.</p>
        <Button href="/products/cybersecurity/assembly/01NumberingSystem" color="alternative">Learn more<ArrowRightOutline class="ms-2 w-3 h-3" /></Button>
      </TimelineItem>

    </Timeline>
  
  
    
  {/if}



  

  
  