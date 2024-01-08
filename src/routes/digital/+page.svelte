<script>
    import { Carousel } from 'flowbite-svelte';
    import { Breadcrumb, BreadcrumbItem } from 'flowbite-svelte';
    import ComingSoon from "$lib/Components/ComingSoon.svelte";
    import { images } from './imagesData/imagesData.js';
</script>
    
<Breadcrumb aria-label="Default breadcrumb example" class="my-4">
    <BreadcrumbItem href="/" home>Home</BreadcrumbItem>
    <BreadcrumbItem>Digital</BreadcrumbItem>
</Breadcrumb>



<div class="justify-center items-center self-center  w-full max-w-3xl my-auto ">
    <Carousel {images} duration={4000} let:Indicators>
      <span slot="slide"  let:Slide let:index>
        <Slide image={images[index]} />
      </span>
      <Indicators />
    </Carousel>
</div>


<ComingSoon />