<script>

    import { Breadcrumb, BreadcrumbItem, Timeline, TimelineItem, Button } from 'flowbite-svelte';
    import { ArrowRightOutline } from 'flowbite-svelte-icons';
  
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
        <BreadcrumbItem href="/products" linkClass='ms-1 text-sm font-medium text-gray-700 hover:text-gray-900 md:ms-2 dark:text-black dark:hover:text-white'>Products</BreadcrumbItem>
        <BreadcrumbItem href="/products/cybersecurity" linkClass='ms-1 text-sm font-medium text-gray-700 hover:text-gray-900 md:ms-2 dark:text-black dark:hover:text-white'>Cybersecurity</BreadcrumbItem>
        <BreadcrumbItem spanClass='ms-1 text-sm font-medium text-gray-500 md:ms-2 dark:text-customColorD'>Assembly</BreadcrumbItem>
    </Breadcrumb>
  
  
  
  
  
  {#if x}
      
    <SmxLoader />
  
  {:else}

    <div class="mt-10">
    </div>

    <Timeline class="m-auto">

      <TimelineItem title="01 Numbering System">
        <p class="mb-4 text-base font-normal text-gray-500 dark:text-gray-400">The assembly numbering system refers to the method of assigning and organizing part numbers or codes to components in a product or assembly.</p>
        <Button href="/products/cybersecurity/assembly/01NumberingSystem" color="alternative">Learn more<ArrowRightOutline class="ms-2 w-3 h-3" /></Button>
      </TimelineItem>

      <TimelineItem title="02 Data Formats">
        <p class="mb-4 text-base font-normal text-gray-500 dark:text-gray-400">"Data Formats Assembly" typically refers to the process of organizing and structuring data in a specific way, often using a standardized format.</p>
        <Button href="/products/cybersecurity/assembly/02DataFormats" color="alternative">Learn more<ArrowRightOutline class="ms-2 w-3 h-3" /></Button>
      </TimelineItem>

      <TimelineItem title="03 Computer System">
        <p class="mb-4 text-base font-normal text-gray-500 dark:text-gray-400">A computer system's primary functions include input, processing, storage, output, and communication. Input devices collect data, the CPU processes it, and the results are stored in memory or on storage devices.</p>
        <Button href="/products/cybersecurity/assembly/03ComputerSystem" color="alternative">Learn more<ArrowRightOutline class="ms-2 w-3 h-3" /></Button>
      </TimelineItem>

      
      <TimelineItem title="04 Memory System">
        <p class="mb-4 text-base font-normal text-gray-500 dark:text-gray-400">"memory system" refers to the organization and management of memory in a computer. Memory is a crucial component in a computer system where data and instructions are stored for processing.</p>
        <Button href="/products/cybersecurity/assembly/04MemorySystem" color="alternative">Learn more<ArrowRightOutline class="ms-2 w-3 h-3" /></Button>
      </TimelineItem>


      <TimelineItem title="05 Microprocessor Architecture">
        <p class="mb-4 text-base font-normal text-gray-500 dark:text-gray-400">"Microprocessor architecture" refers to the set of rules and conventions governing the design and functioning of a microprocessor, which is a central processing unit (CPU) contained on a single integrated circuit (IC).</p>
        <Button href="/products/cybersecurity/assembly/05MicroprocessorArchitecture" color="alternative">Learn more<ArrowRightOutline class="ms-2 w-3 h-3" /></Button>
      </TimelineItem>

      <TimelineItem title="06 Real Mode Operation">
        <p class="mb-4 text-base font-normal text-gray-500 dark:text-gray-400">"Real mode" is an operation mode of x86 architecture processors, where the processor behaves as a 16-bit processor. In real mode, the processor uses a segmented memory model, where memory addresses are formed by combining a 16-bit segment value and a 16-bit offset value.</p>
        <Button href="/products/cybersecurity/assembly/06RealModeOperation" color="alternative">Learn more<ArrowRightOutline class="ms-2 w-3 h-3" /></Button>
      </TimelineItem>

      <TimelineItem title="07 Data Addressing Modes">
        <p class="mb-4 text-base font-normal text-gray-500 dark:text-gray-400">"addressing modes define how the processor calculates the memory address of operands for instructions. </p>
        <Button href="/products/cybersecurity/assembly/07DataAddressingModes" color="alternative">Learn more<ArrowRightOutline class="ms-2 w-3 h-3" /></Button>
      </TimelineItem>

      

    </Timeline>
  
  
    
  {/if}



  

  
  