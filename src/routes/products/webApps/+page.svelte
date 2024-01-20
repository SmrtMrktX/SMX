<script>

    import { Breadcrumb, BreadcrumbItem, Card, Button, Badge } from 'flowbite-svelte';
    import { ArrowRightOutline } from 'flowbite-svelte-icons';
  
    import SmxLoader from "$lib/Components/SmxLoader.svelte";
    import ComingSoon from '$lib/Components/ComingSoon.svelte';

    import basicwebpagelg from "$lib/img/products/webApps/basicwebpage.webp";
  
  
  
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
      <BreadcrumbItem href="/products">Products</BreadcrumbItem>
      <BreadcrumbItem>Web Apps</BreadcrumbItem>
  </Breadcrumb>
  
  
  
  
  
  
  {#if x}
      
    <SmxLoader />
  
  {:else}
  
    <div class="gap-4 grid  md:grid-cols-2 lg:grid-cols-3 m-auto">
        
        <div  class="space-y-4 m-auto max-w-60 max-h-xs">
            
          <Card img={basicwebpagelg}>
              
            <div class="justify-end items-end text-end self-end">
                <Badge border color="green" >Free</Badge>
            </div> 
              
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Basic Web Page.</h5>
              
            <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight">HTML5, CSS3.</p>
            

            <div class="mx-auto mb-3 text-center rounded border-2">
              <a style="font-family: 'Russo One', sans-serif;" href="https://github.com/smrket/BasicWebPage" target="_blank" class="text-purple-600 mx-2">Source code</a>
            </div>
            
            <Button href="https://smrket.github.io/BasicWebPage/" target="_blank">
              Watch The App<ArrowRightOutline class="w-3.5 h-3.5 ms-2 text-white" />
            </Button>

            </Card>
        </div>
    </div>
    
    
  {/if}
  