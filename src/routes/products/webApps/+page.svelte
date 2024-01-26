<script>

    import { Breadcrumb, BreadcrumbItem, Card, Button, Badge } from 'flowbite-svelte';
    import { ArrowRightOutline } from 'flowbite-svelte-icons';
  
    import SmxLoader from "$lib/Components/SmxLoader.svelte";


    import webtemplateslg from "$lib/img/products/webApps/webtemplates.webp";
    import arabicwebappslg from "$lib/img/products/webApps/arabicwebappslg.webp";
    import crudapplg from "$lib/img/products/webApps/crudapp.webp";
    import basicwebpagelg from "$lib/img/products/webApps/basicwebpage.webp";
    import blackjacklg from "$lib/img/products/webApps/blackjackwebapp.webp";
    import gridcsslg from "$lib/img/products/webApps/gridcssapp.webp";
  
  
  
  
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
      <BreadcrumbItem spanClass='ms-1 text-sm font-medium text-gray-500 md:ms-2 dark:text-customColorD'>Web Apps</BreadcrumbItem>
  </Breadcrumb>
  
  
  
  
  
  
{#if x}
      
  <SmxLoader />
  
{:else}


  <div class="gap-8 grid  md:grid-cols-2 md:gap-12 lg:grid-cols-3 lg:gap-16 m-auto py-10">


    <div  class="space-y-4 m-auto w-72 max-h-xs">
          
      <Card img={webtemplateslg}>
          
        <div class="justify-end items-end text-end self-end">
            <Badge border color="green" >Free</Badge>
        </div> 
          
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Web Templates.</h5>
          
        <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight">HTML, CSS, JS.</p>
        

        <div class="mx-auto mb-3 text-center rounded border-2">
          <a style="font-family: 'Russo One', sans-serif;" href="https://github.com/smrket/Web-Templates" target="_blank" class="text-purple-600 mx-2">Source code</a>
        </div>
        
        <Button href="https://smrket.github.io/Web-Templates/" target="_blank">
          Live App<ArrowRightOutline class="w-3.5 h-3.5 ms-2 text-white" />
        </Button>

        </Card>
    </div>



    <div  class="space-y-4 m-auto w-72 max-h-xs">
          
      <Card img={arabicwebappslg}>
          
        <div class="justify-end items-end text-end self-end">
            <Badge border color="green" >Free</Badge>
        </div> 
          
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Arabic Web Apps.</h5>
          
        <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight">HTML, CSS, JS.</p>
        

        <div class="mx-auto mb-3 text-center rounded border-2">
          <a style="font-family: 'Russo One', sans-serif;" href="https://github.com/smrket/Arabic-Webapps" target="_blank" class="text-purple-600 mx-2">Source code</a>
        </div>
        
        <Button href="https://smrket.github.io/Arabic-Webapps/" target="_blank">
          Live App<ArrowRightOutline class="w-3.5 h-3.5 ms-2 text-white" />
        </Button>

        </Card>
    </div>



    <div  class="space-y-4 m-auto w-72 max-h-xs">
          
      <Card img={crudapplg}>
          
        <div class="justify-end items-end text-end self-end">
            <Badge border color="green" >Free</Badge>
        </div> 
          
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">CRUD App.</h5>
          
        <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight">HTML, CSS, JS.</p>
        

        <div class="mx-auto mb-3 text-center rounded border-2">
          <a style="font-family: 'Russo One', sans-serif;" href="https://github.com/smrket/CRUDapp" target="_blank" class="text-purple-600 mx-2">Source code</a>
        </div>
        
        <Button href="https://smrket.github.io/CRUDapp/" target="_blank">
          Live App<ArrowRightOutline class="w-3.5 h-3.5 ms-2 text-white" />
        </Button>

        </Card>
    </div>




      <div  class="space-y-4 m-auto w-72 max-h-xs">
            
        <Card img={gridcsslg}>
            
          <div class="justify-end items-end text-end self-end">
              <Badge border color="green" >Free</Badge>
          </div> 
            
          <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Grid Css App.</h5>
            
          <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight">HTML, CSS.</p>
          

          <div class="mx-auto mb-3 text-center rounded border-2">
            <a style="font-family: 'Russo One', sans-serif;" href="https://github.com/smrket/GridCssApp" target="_blank" class="text-purple-600 mx-2">Source code</a>
          </div>
          
          <Button href="https://smrket.github.io/GridCssApp/" target="_blank">
            Live App<ArrowRightOutline class="w-3.5 h-3.5 ms-2 text-white" />
          </Button>

          </Card>
      </div>



      <div  class="space-y-4 m-auto w-72 max-h-xs">
            
          <Card img={blackjacklg}>
              
            <div class="justify-end items-end text-end self-end">
                <Badge border color="green" >Free</Badge>
            </div> 
              
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Blackjack Web App.</h5>
              
            <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight">HTML, CSS, JS.</p>
            

            <div class="mx-auto mb-3 text-center rounded border-2">
              <a style="font-family: 'Russo One', sans-serif;" href="https://github.com/smrket/BlackjackWebApp" target="_blank" class="text-purple-600 mx-2">Source code</a>
            </div>
            
            <Button href="https://smrket.github.io/BlackjackWebApp/" target="_blank">
              Live App<ArrowRightOutline class="w-3.5 h-3.5 ms-2 text-white" />
            </Button>

            </Card>
      </div>

      <div  class="space-y-4 m-auto w-72 max-h-xs">
            
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
              Live App<ArrowRightOutline class="w-3.5 h-3.5 ms-2 text-white" />
            </Button>

            </Card>
      </div>

    </div>
    
{/if}
  