<script>

    import { Breadcrumb, BreadcrumbItem} from 'flowbite-svelte';
    
  
    import SmxLoader from "$lib/Components/SmxLoader.svelte";

    import lg001 from "$lib/img/products/cybersecurity/assembly/microprocessorArchitecture/001.webp";
    import lg002 from "$lib/img/products/cybersecurity/assembly/microprocessorArchitecture/002.webp";
    import lg003 from "$lib/img/products/cybersecurity/assembly/microprocessorArchitecture/003.webp";
    import lg004 from "$lib/img/products/cybersecurity/assembly/microprocessorArchitecture/004.webp";
    import lg005 from "$lib/img/products/cybersecurity/assembly/microprocessorArchitecture/005.webp";
    import lg006 from "$lib/img/products/cybersecurity/assembly/microprocessorArchitecture/006.webp";
    import lg007 from "$lib/img/products/cybersecurity/assembly/microprocessorArchitecture/007.webp";
    import lg008 from "$lib/img/products/cybersecurity/assembly/microprocessorArchitecture/008.webp";
    import lg009 from "$lib/img/products/cybersecurity/assembly/microprocessorArchitecture/009.webp";
    import lg010 from "$lib/img/products/cybersecurity/assembly/microprocessorArchitecture/010.webp";
    import lg011 from "$lib/img/products/cybersecurity/assembly/microprocessorArchitecture/011.webp";
    import lg012 from "$lib/img/products/cybersecurity/assembly/microprocessorArchitecture/012.webp";
    import lg013 from "$lib/img/products/cybersecurity/assembly/microprocessorArchitecture/013.webp";
    




  
  
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


    <h1 class="text-center text-2xl font-extrabold my-4">Microprocessor Architecture</h1>


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
    

  
  
    
  {/if}



  

  
  