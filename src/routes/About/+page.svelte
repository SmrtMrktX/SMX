<script>
    import { Breadcrumb, BreadcrumbItem } from 'flowbite-svelte';
    import PoweredBy from "$lib/Components/PoweredBy.svelte";
    import opensourcelg from '$lib/img/poweredBy/opensourcelg.png';
    import githublg from '$lib/img/poweredBy/githublg.png';
    import sveltekitlg from '$lib/img/poweredBy/sveltekitlg.png';
    import vercellg from '$lib/img/poweredBy/vercellg.png';
</script>
    
<Breadcrumb aria-label="Default breadcrumb example" class="my-4">
    <BreadcrumbItem href="/" home>Home</BreadcrumbItem>
    <BreadcrumbItem>About</BreadcrumbItem>
</Breadcrumb>


<div class="m-10 text-3xl md:text-4xl font-bold tracking-widest text-primary-customLime justify-center items-center text-center">
    <!-- <h1 class="my-10 text-3xl md:text-4xl font-bold tracking-widest text-primary-customLime underline">POWERED BY</h1> -->
    <PoweredBy  text="POWERED &nbsp BY" delay={250} />
</div>



<div class="grid gap-10 md:grid-cols-2  md:gap-10 justify-center items-center m-auto px-10">

    <figure class="grid md:col-span-1 max-w-xl lg:max-w-2xl">
        <img class="dark:invert h-auto max-w-full rounded-lg" src={opensourcelg} alt="">
        <figcaption class="mb-10 mt-2 text-base text-center ">©</figcaption>
    </figure>

    <figure class="grid md:col-span-1 max-w-xl">
        <img class="dark:invert h-auto max-w-full rounded-lg" src={githublg} alt="">
        <figcaption class="mb-10 mt-2 text-base text-center ">©</figcaption>
    </figure>

    <figure class="grid md:col-span-1 max-w-xl">
        <img class="dark:invert h-auto max-w-full rounded-lg" src={sveltekitlg} alt="hi">
        <figcaption class="mb-10 mt-2 text-base text-center ">©</figcaption>
    </figure>

    <figure class="grid md:col-span-1 max-w-xl">
        <img class="dark:invert h-auto max-w-full rounded-lg" src={vercellg} alt="">
        <figcaption class="mb-10 mt-2 text-base text-center ">©</figcaption>
    </figure>

</div>