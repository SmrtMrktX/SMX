<head>
    <!-- Other meta tags and styles -->
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css" rel="stylesheet">
</head>







<script>
    import { Breadcrumb, BreadcrumbItem } from 'flowbite-svelte';

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
  <BreadcrumbItem spanClass='ms-1 text-sm font-medium text-gray-500 md:ms-2 dark:text-customColorD'>Contact</BreadcrumbItem>
</Breadcrumb>








{#if x}
    
  <SmxLoader />

{:else}

  <div style="font-family: 'Russo One', sans-serif;" class="shadow-sm dark:shadow-black justify-center items-center text-center text-4xl my-10">
    <h1 class="text-6xl text-purple-500">Social</h1>
    
    <div class="grid grid-cols-2 gap-10 md:grid-cols-3 md:gap-20 justify-center items-center text-center space-x-4 my-20 mx-10">
      <a href="https://www.facebook.com/smrtmrktx" target="_blank" class="text-black dark:text-white hover:text-blue-700"><i class="fab fa-facebook text-6xl md:text-8xl"></i></a>
      <a href="https://twitter.com/SmrtMrket" target="_blank" class="text-black dark:text-white hover:text-white hover:bg-black dark:hover:text-black dark:hover:bg-white rounded-full"><i class="fas fa-times text-6xl md:text-8xl"></i></a>
      <a href="https://www.linkedin.com/in/smrtmrktx/" target="_blank" class="text-black dark:text-white hover:text-blue-700"><i class="fab fa-linkedin text-6xl md:text-8xl"></i></a>
      <a href="https://www.github.com/SmrtMrktX" target="_blank" class="text-black dark:text-white hover:text-gray-700"><i class="fab fa-github text-6xl md:text-8xl"></i></a>
      <a href="https://www.tiktok.com/@smrtmrktx" target="_blank" class="text-black dark:text-white hover:text-pink-500"><i class="fab fa-tiktok text-6xl md:text-8xl"></i></a>
      <a href="https://www.instagram.com/smrtmrket/" target="_blank" class="text-black dark:text-white hover:text-pink-500"><i class="fab fa-instagram text-6xl md:text-8xl"></i></a>
    </div>
    
    <h1 class="text-6xl text-purple-500">Mail</h1>
    
    <div class="m-20 flex justify-center space-x-4">
        <a href="mailto:smrtmrket@gmail.com" class="text-black dark:text-white hover:text-blue-500"><i class="fas fa-envelope text-9xl"></i></a>
        <!-- Other social links -->
    </div>

    <h1 class="text-6xl  text-purple-500">Whatsapp</h1>
    
    <div class="mx-20 mt-20 mb-10 flex justify-center space-x-4">
        <a href="/Contact" class="text-black dark:text-white hover:text-green-500"><i class="fab fa-whatsapp text-8xl"></i></a>
        <!-- Other social links -->
    </div>
  </div>
  
{/if}

