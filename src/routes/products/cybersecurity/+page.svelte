<script>

    import { Breadcrumb, BreadcrumbItem, Tabs, TabItem, List, Li } from 'flowbite-svelte';
  
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
        <BreadcrumbItem spanClass='ms-1 text-sm font-medium text-gray-500 md:ms-2 dark:text-customColorD'>Cybersecurity</BreadcrumbItem>
    </Breadcrumb>
  
  
  
  
  
  {#if x}
      
    <SmxLoader />
  
  {:else}
  
  
  <Tabs style="full" defaultClass="flex rounded-lg divide-x rtl:divide-x-reverse divide-gray-200 shadow dark:divide-gray-700 mt-20">
    <TabItem class="w-full" open>
        <span slot="title">Free resources</span>
        <p class="text-sm text-gray-500 dark:text-gray-400">
        <b>Free resources:</b>

        Cybersecurity involves protecting computer systems, networks, and data from unauthorized access, attacks, and damage.
        Free resources in cybersecurity refer to tools, materials, and information that are available at no cost to help individuals or organizations enhance their digital security and defend against cyber threats. 
        These resources may include antivirus software, educational materials, online courses, and practical tips for maintaining a secure online environment.
        </p>

        <List class="my-5">
            <Li>
                <a href="/products/cybersecurity/assembly" class="font-bold">Assembly</a>
            </Li>
            <Li>...</Li>
            <Li>...</Li>
          </List>
    </TabItem>




    <TabItem class="w-full">
      <span slot="title">courses</span>
      <p class="text-sm text-gray-500 dark:text-gray-400">
        <b>courses:</b>
        Coming soon . . .
      </p>
    </TabItem>
    <TabItem class="w-full">
      <span slot="title">Labs</span>
      <p class="text-sm text-gray-500 dark:text-gray-400">
        <b>Labs:</b>
        Coming soon . . .
      </p>
    </TabItem>
    <TabItem class="w-full">
      <span slot="title">Best links</span>
      <p class="text-sm text-gray-500 dark:text-gray-400">
        <b>Best links:</b>
        Coming soon . . .
      </p>
    </TabItem>
  </Tabs>
    
  {/if}
  
  