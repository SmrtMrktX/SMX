<script>
    import { Carousel } from 'flowbite-svelte';
    import { images } from '$lib/imagesData/imagesData.js';
</script>



<div class="justify-center items-center self-center  w-full max-w-3xl my-auto ">
  <div class="max-w-4xl">
    <Carousel {images} duration="3900" />
  </div>
</div>