<script>
    import { Breadcrumb, BreadcrumbItem } from 'flowbite-svelte';
    import SmxLoader from "$lib/Components/SmxLoader.svelte";
    import PoweredBy from "$lib/Components/PoweredBy.svelte";

    import opensourcelg from '$lib/img/poweredBy/opensourcelg.webp';
    import githublg from '$lib/img/poweredBy/githublg.webp';
    import sveltekitlg from '$lib/img/poweredBy/sveltekitlg.webp';
    import vercellg from '$lib/img/poweredBy/vercellg.webp';
    import flowbitelg from '$lib/img/poweredBy/flowbitelg.webp';
    import openailg from '$lib/img/poweredBy/openailg.webp';
    
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
    <BreadcrumbItem spanClass='ms-1 text-sm font-medium text-gray-500 md:ms-2 dark:text-customColorD'>About</BreadcrumbItem>
</Breadcrumb>






{#if x}
    
  <SmxLoader />

{:else}



    <div style="background-color: lime;" class=" rounded-full my-10 mx-auto px-2 text-3xl md:text-4xl font-bold tracking-widest justify-center items-center text-center">
        <!-- <h1 class="my-10 text-3xl md:text-4xl font-bold tracking-widest text-primary-customLime underline">POWERED BY</h1> -->
        <PoweredBy  text="POWERED BY" delay={250} />
    </div>



    <div class="grid gap-10 md:grid-cols-2  md:gap-10 lg:gap-20 justify-center items-center text-center mb-10 mx-auto px-10 lg:px-20 text-xl lg:text-2xl ">

        <figure class="grid md:col-span-1 max-w-xl rounded-lg transition duration-700 ease-in-out p-1 hover:backdrop-blur-sm hover:scale-105 hover:shadow-md hover:shadow-customColorD  dark:hover:shadow-customColorW">
            <img class="dark:invert h-auto max-w-full rounded-lg mb-0" src={opensourcelg} alt="Opensource Logo">
            <figcaption class="my-0 text-center "><a href="https://opensource.org/" target="_blank">®</a></figcaption>
        </figure>

        <figure class="grid md:col-span-1 max-w-xl rounded-lg transition duration-700 ease-in-out p-1 hover:backdrop-blur-sm hover:scale-105 hover:shadow-md hover:shadow-customColorD  dark:hover:shadow-customColorW">
            <img class="dark:invert h-auto max-w-full rounded-lg" src={githublg} alt="Github Logo">
            <figcaption class="mb-0  text-center "><a href="https://github.com/" target="_blank">®</a></figcaption>
        </figure>

        <figure class="grid md:col-span-1 max-w-xl rounded-lg transition duration-700 ease-in-out p-1 hover:backdrop-blur-sm hover:scale-105 hover:shadow-md hover:shadow-customColorD  dark:hover:shadow-customColorW">
            <img class="dark:invert h-auto max-w-full rounded-lg" src={sveltekitlg} alt="Sveltekit LOGO">
            <figcaption class="mb-0 text-center "><a href="https://kit.svelte.dev/" target="_blank">®</a></figcaption>
        </figure>

        <figure class="grid md:col-span-1 max-w-xl rounded-lg transition duration-700 ease-in-out p-1 hover:backdrop-blur-sm hover:scale-105 hover:shadow-md hover:shadow-customColorD  dark:hover:shadow-customColorW">
            <img class="dark:invert h-auto max-w-full rounded-lg" src={vercellg} alt="Vercel Logo">
            <figcaption class="mb-0 text-center "><a href="https://vercel.com/" target="_blank">®</a></figcaption>
        </figure>

        <figure class="grid md:col-span-1 max-w-xl rounded-lg transition duration-700 ease-in-out p-1 hover:backdrop-blur-sm hover:scale-105 hover:shadow-md hover:shadow-customColorD  dark:hover:shadow-customColorW">
            <img class="dark:invert h-auto max-w-full rounded-lg" src={flowbitelg} alt="Flowbite Logo">
            <figcaption class="mb-0 text-center "><a href="https://flowbite.com/" target="_blank">®</a></figcaption>
        </figure>

        <figure class="grid md:col-span-1 max-w-xl rounded-lg transition duration-700 ease-in-out p-1 hover:backdrop-blur-sm hover:scale-105 hover:shadow-md hover:shadow-customColorD  dark:hover:shadow-customColorW">
            <img class="dark:invert h-auto max-w-full rounded-lg" src={openailg} alt="OpenAI Logo">
            <figcaption class="text-center"><a href="https://openai.com/" target="_blank">®</a></figcaption>
        </figure>

    </div>



{/if}









<style>



    a {
        font-family: 'Russo One', sans-serif;
    }



    @keyframes colorChange {
        0% {
            color: #32CD32; /* Start color */
        }
        50% {
            color: purple; /* Middle color */

        }
        100% {
            color: #32CD32; /* End color (back to the start) */
        }
    }

        

    /* Apply the animation to the text */

    figure:hover {
        animation: colorChange 2s infinite;
        font-weight:800;
    }


</style>