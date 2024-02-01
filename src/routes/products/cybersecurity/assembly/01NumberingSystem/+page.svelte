<script>

    import { Breadcrumb, BreadcrumbItem} from 'flowbite-svelte';
    
  
    import SmxLoader from "$lib/Components/SmxLoader.svelte";

    import lg001 from "$lib/img/products/cybersecurity/assembly/numberingSystem/001.webp";
    import lg002 from "$lib/img/products/cybersecurity/assembly/numberingSystem/002.webp";
    import lg003 from "$lib/img/products/cybersecurity/assembly/numberingSystem/003.webp";
    import lg004 from "$lib/img/products/cybersecurity/assembly/numberingSystem/004.webp";
    import lg005 from "$lib/img/products/cybersecurity/assembly/numberingSystem/005.webp";
    import lg006 from "$lib/img/products/cybersecurity/assembly/numberingSystem/006.webp";
    import lg007 from "$lib/img/products/cybersecurity/assembly/numberingSystem/007.webp";
    import lg008 from "$lib/img/products/cybersecurity/assembly/numberingSystem/008.webp";
    import lg009 from "$lib/img/products/cybersecurity/assembly/numberingSystem/009.webp";
    import lg010 from "$lib/img/products/cybersecurity/assembly/numberingSystem/010.webp";
    import lg011 from "$lib/img/products/cybersecurity/assembly/numberingSystem/011.webp";
    import lg012 from "$lib/img/products/cybersecurity/assembly/numberingSystem/012.webp";
    import lg013 from "$lib/img/products/cybersecurity/assembly/numberingSystem/013.webp";
    import lg014 from "$lib/img/products/cybersecurity/assembly/numberingSystem/014.webp";
    import lg015 from "$lib/img/products/cybersecurity/assembly/numberingSystem/015.webp";
    import lg016 from "$lib/img/products/cybersecurity/assembly/numberingSystem/016.webp";
    import lg017 from "$lib/img/products/cybersecurity/assembly/numberingSystem/017.webp";
    import lg018 from "$lib/img/products/cybersecurity/assembly/numberingSystem/018.webp";
    import lg019 from "$lib/img/products/cybersecurity/assembly/numberingSystem/019.webp";
    import lg020 from "$lib/img/products/cybersecurity/assembly/numberingSystem/020.webp";
    import lg021 from "$lib/img/products/cybersecurity/assembly/numberingSystem/021.webp";

    import ComingSoon from '$lib/Components/ComingSoon.svelte';


  
  
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
        <BreadcrumbItem href="/products/cybersecurity" linkClass='ms-1 text-sm font-medium text-gray-700 hover:text-gray-900 md:ms-2 dark:text-black dark:hover:text-white'>Cybersecurity</BreadcrumbItem>
        <BreadcrumbItem href="/products/cybersecurity/assembly" linkClass='ms-1 text-sm font-medium text-gray-700 hover:text-gray-900 md:ms-2 dark:text-black dark:hover:text-white'>Assembly</BreadcrumbItem>
    </Breadcrumb>
  
  
  
  
  
  {#if x}
      
    <SmxLoader />
  
  {:else}


    <h1 class="text-center text-2xl font-extrabold my-4">Numbering System</h1>


    <img src={lg001} class="rounded mx-auto my-4 w-full max-w-7xl shadow-sm shadow-primary-customLime" alt="001"/>
    <img src={lg002} class="rounded mx-auto my-4 w-full max-w-7xl shadow-sm shadow-primary-customLime" alt="002"/>
    <img src={lg003} class="rounded mx-auto my-4 w-full max-w-7xl shadow-sm shadow-primary-customLime" alt="003"/>
    <img src={lg004} class="rounded mx-auto my-4 w-full max-w-7xl shadow-sm shadow-primary-customLime" alt="004"/>
    <img src={lg005} class="rounded mx-auto my-4 w-full max-w-7xl shadow-sm shadow-primary-customLime" alt="005"/>
    <img src={lg006} class="rounded mx-auto my-4 w-full max-w-7xl shadow-sm shadow-primary-customLime" alt="006"/>
    <img src={lg007} class="rounded mx-auto my-4 w-full max-w-7xl shadow-sm shadow-primary-customLime" alt="007"/>
    <img src={lg008} class="rounded mx-auto my-4 w-full max-w-7xl shadow-sm shadow-primary-customLime" alt="008"/>
    <img src={lg009} class="rounded mx-auto my-4 w-full max-w-7xl shadow-sm shadow-primary-customLime" alt="009"/>
    <img src={lg010} class="rounded mx-auto my-4 w-full max-w-7xl shadow-sm shadow-primary-customLime" alt="010"/>
    <img src={lg011} class="rounded mx-auto my-4 w-full max-w-7xl shadow-sm shadow-primary-customLime" alt="011"/>
    <img src={lg012} class="rounded mx-auto my-4 w-full max-w-7xl shadow-sm shadow-primary-customLime" alt="012"/>
    <img src={lg013} class="rounded mx-auto my-4 w-full max-w-7xl shadow-sm shadow-primary-customLime" alt="013"/>
    <img src={lg014} class="rounded mx-auto my-4 w-full max-w-7xl shadow-sm shadow-primary-customLime" alt="014"/>
    <img src={lg015} class="rounded mx-auto my-4 w-full max-w-7xl shadow-sm shadow-primary-customLime" alt="015"/>
    <img src={lg016} class="rounded mx-auto my-4 w-full max-w-7xl shadow-sm shadow-primary-customLime" alt="016"/>
    <img src={lg017} class="rounded mx-auto my-4 w-full max-w-7xl shadow-sm shadow-primary-customLime" alt="017"/>
    <img src={lg018} class="rounded mx-auto my-4 w-full max-w-7xl shadow-sm shadow-primary-customLime" alt="018"/>
    <img src={lg019} class="rounded mx-auto my-4 w-full max-w-7xl shadow-sm shadow-primary-customLime" alt="019"/>
    <img src={lg020} class="rounded mx-auto my-4 w-full max-w-7xl shadow-sm shadow-primary-customLime" alt="020"/>
    <img src={lg021} class="rounded mx-auto my-4 w-full max-w-7xl shadow-sm shadow-primary-customLime" alt="021"/>

    <!-- <ComingSoon /> -->
  
  
    
  {/if}



  

  
  