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
    <BreadcrumbItem spanClass='ms-1 text-sm font-medium text-gray-500 md:ms-2 dark:text-customColorD'>Licensing</BreadcrumbItem>
</Breadcrumb>









{#if x}
    
  <SmxLoader />

{:else}



  <div class="backdrop-blur-sm flex justify-center items-center m-auto border shadow-2xl rounded  border-lime-400 md:border-2 p-2 lg:text-xl leading-relaxed tracking-wider max-w-4xl">
    <span class="p-2">
      <h1 style="font-family: 'Russo One', sans-serif;" class="font-bold text-purple-600 "> MIT License</h1>
 
      <h2 class="font-mono font-extrabold">Copyright (c) 2023 SMRT MRKT X السوق الذكية</h2>

      <br>
      <h3 class="p-2 font-bold text-customColorD dark:text-customColorW">
        Permission is hereby granted, free of charge, to any person obtaining a copy
        of this software and associated documentation files (the "Software"), to deal
        in the Software without restriction, including without limitation the rights
        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
        copies of the Software, and to permit persons to whom the Software is
        furnished to do so, subject to the following conditions:
        <br>
        <br>
        <span style="font-family: 'Russo One', sans-serif;" class="text-primary-customLime ">
          The above copyright notice and this permission notice shall be included in all
          copies or substantial portions of the Software.
        </span>
        <br>
        <br>

        <h2 class="p-2 font-extrabold text-customColorD dark:text-customColorW">
          THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
          IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
          FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
          AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
          LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
          OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
          SOFTWARE.
        </h2>
      </h3>
    </span>
  </div>



{/if}

