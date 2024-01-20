<script>
    import { Breadcrumb, BreadcrumbItem } from 'flowbite-svelte';
    import SmxLoader from "$lib/Components/SmxLoader.svelte";

    let x = true;
    const ToOther = () => {
      setTimeout(() => {
        x = false; 
      }, 900); 
    };

    ToOther();

</script>






<Breadcrumb aria-label="Default breadcrumb example" class="my-4">
    <BreadcrumbItem href="/" home homeClass="inline-flex items-center text-sm font-medium text-gray-700 hover:text-gray-900 dark:text-black dark:hover:text-white">Home</BreadcrumbItem>
    <BreadcrumbItem spanClass='ms-1 text-sm font-medium text-gray-500 md:ms-2 dark:text-customColorD'>Privacy Policy</BreadcrumbItem>
</Breadcrumb>








{#if x}
    
  <SmxLoader />

{:else}
    
    
    <h1 class="text-center tracking-widest text-2xl md:text-3xl font-extrabold m-auto"> Privacy Policy</h1> 

    <h2 class="text-center m-auto tracking-widest text-xl md:text-2xl text-primary-customLime">
    Your privacy is important to us.
    </h2>

    <div class="backdrop-blur-sm justify-center items-center text-center p-2 mb-24">
        <h3 class=" leading-10 tracking-widest md:px-16">
            It is Smrt Mrkt X's policy to respect your privacy regarding any information we may collect from you across our website, and other sites we own and operate.
        </h3>
    </div>
    
  
{/if}






<style>
    h1,h2,h3{
        font-family: 'Russo One', sans-serif;
    }
</style>