<script>
    import { Breadcrumb, BreadcrumbItem } from 'flowbite-svelte';
    import SmxLoader from "$lib/Components/SmxLoader.svelte";
    import PoweredBy from "$lib/Components/PoweredBy.svelte";
    import opensourcelg from '$lib/img/poweredBy/opensourcelg.png';
    import githublg from '$lib/img/poweredBy/githublg.png';
    import sveltekitlg from '$lib/img/poweredBy/sveltekitlg.png';
    import vercellg from '$lib/img/poweredBy/vercellg.png';
    
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
    <BreadcrumbItem>About</BreadcrumbItem>
</Breadcrumb>

{#if x}
    
  <SmxLoader />

{:else}

  <div class="m-10 text-3xl md:text-4xl font-bold tracking-widest text-primary-customLime justify-center items-center text-center">
    <!-- <h1 class="my-10 text-3xl md:text-4xl font-bold tracking-widest text-primary-customLime underline">POWERED BY</h1> -->
    <PoweredBy  text="POWERED BY" delay={250} />
</div>



<div class="grid gap-10 md:grid-cols-2  md:gap-10 justify-center items-center m-auto px-10 text-2xl ">

    <figure class="grid md:col-span-1 max-w-xl lg:max-w-2xl">
        <img class="dark:invert h-auto max-w-full rounded-lg" src={opensourcelg} alt="">
        <figcaption class="mb-10 mt-2 text-center "><a href="https://opensource.org/" target="_blank">®</a></figcaption>
    </figure>

    <figure class="grid md:col-span-1 max-w-xl">
        <img class="dark:invert h-auto max-w-full rounded-lg" src={githublg} alt="">
        <figcaption class="mb-10 mt-2  text-center "><a href="https://github.com/" target="_blank">®</a></figcaption>
    </figure>

    <figure class="grid md:col-span-1 max-w-xl">
        <img class="dark:invert h-auto max-w-full rounded-lg" src={sveltekitlg} alt="hi">
        <figcaption class="mb-10 mt-2 text-center "><a href="https://kit.svelte.dev/" target="_blank">®</a></figcaption>
    </figure>

    <figure class="grid md:col-span-1 max-w-xl">
        <img class="dark:invert h-auto max-w-full rounded-lg" src={vercellg} alt="">
        <figcaption class="mb-10 mt-2 text-center "><a href="https://vercel.com/" target="_blank">®</a></figcaption>
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

        a:hover {
            animation: colorChange 2s infinite;
            font-weight:800;
        }


</style>