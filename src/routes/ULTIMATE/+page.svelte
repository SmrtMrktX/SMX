<script>

    import { Breadcrumb, BreadcrumbItem, Tabs, TabItem, List, Li, Button } from 'flowbite-svelte';

    import SmxLoader from "$lib/Components/SmxLoader.svelte";
    
  
    let x =true;
    const ToOther = () => {
      setTimeout(() => {
        x = false; 
      }, 900); 
    };
  
    ToOther();

    let moreTips = false;
    let moreorless = "more";

    const moreLessTips = () => {
      moreTips = !moreTips;
      if (moreTips) {
        moreorless ="less";
      } else {
        moreorless ="more";
      }

    };
  
  </script>
  
  
  
  
  
  
  
  <Breadcrumb aria-label="Default breadcrumb example" class="my-4">
      <BreadcrumbItem href="/" home>Home</BreadcrumbItem>
      <BreadcrumbItem>ULTIMATE</BreadcrumbItem>
  </Breadcrumb>
  
  

  
 
  
  
  
  
{#if x}
      
  <SmxLoader />
  
{:else}

<div class="backdrop-blur-md m-auto text-2xl">

  <Tabs inactiveClasses="text-xl px-2 font-bold mx-4" activeClasses="mx-4 text-2xl text-blue-600 font-extrabold">
    
    <TabItem open title="Tips">

      <p class="mb-4 text-sm text-gray-500 dark:text-gray-400">
        <b>TIPS:</b>
        Succinctly refer to the most effective and intelligent pieces of advice or strategies for optimal results in a given context.      </p>
      <List tag="ol" list="decimal" class="font-bold text-black dark:text-white text-base md:text-lg lg:text-xl">
        <Li>
          Life Hacks:
          <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
            <Li>Include clever life hacks that make daily tasks easier.</Li>
            <Li>Time-saving tips for various activities.</Li>
          </List>
        </Li>

        <Li>
          Productivity Tips:
          <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
            <Li>Techniques for better time management.</Li>
            <Li>Tools and apps that boost productivity.</Li>
          </List>
        </Li>

        <Li>
          Technology Insights:
          <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
            <Li>Updates on the latest tech trends.</Li>
            <Li>How-to guides for using popular gadgets or software.</Li>
          </List>
        </Li>
        
        {#if moreTips}
          <Li>
            Finance and Money Management:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Budgeting tips.</Li>
              <Li>Investment advice or strategies.</Li>
            </List>
          </Li>

          <Li>
            Health and Wellness:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Quick exercises or stretches for desk workers.</Li>
              <Li>Healthy eating tips or recipes.</Li>
            </List>
          </Li>

          <Li>
            Career Development:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Resume writing tips.</Li>
              <Li>Job interview strategies.</Li>
            </List>
          </Li>

          <Li>
            Education and Learning:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Effective study techniques.</Li>
              <Li>Online learning resources.</Li>
            </List>
          </Li>

          <Li>
            Travel Hacks:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Tips for finding the best travel deals.</Li>
              <Li>Packing efficiently for different types of trips.</Li>
            </List>
          </Li>

          <Li>
            Home Improvement:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>DIY home improvement tips.</Li>
              <Li>Energy-saving ideas.</Li>
            </List>
          </Li>

          <Li>
            Communication Skills:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Effective communication strategies.</Li>
              <Li>Networking tips.</Li>
            </List>
          </Li>

          <Li>
            Social Media:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Tips for building an online presence.</Li>
              <Li>Social media etiquette.</Li>
            </List>
          </Li>

          <Li>
            Mindfulness and Stress Reduction:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Meditation or mindfulness exercises.</Li>
              <Li>Stress-relief techniques.</Li>
            </List>
          </Li>

          <Li>
            Environmental Tips:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Eco-friendly practices at home.</Li>
              <Li>Ways to reduce carbon footprint.</Li>
            </List>
          </Li>

          <Li>
            Creativity Boosters:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Tips for sparking creativity.</Li>
              <Li>Exercises to enhance creative thinking.</Li>
            </List>
          </Li>

          <Li>
            Book and Movie Recommendations:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Lists of must-read books or must-watch movies.</Li>
              <Li>Reviews or summaries.              </Li>
            </List>
          </Li>
        {/if}

        <div class="my-4"></div>
        <Button on:click={moreLessTips} color="purple">{moreorless} Tips</Button>
      </List>
    </TabItem>


    <TabItem title="Hints">
      <p class="text-sm text-gray-500 dark:text-gray-400">
        <b>Hints:</b>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
      </p>
    </TabItem>


    <TabItem title="Resources">
      <p class="text-sm text-gray-500 dark:text-gray-400">
        <b>Resources:</b>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
      </p>
    </TabItem>
  </Tabs>
</div>

    

{/if}