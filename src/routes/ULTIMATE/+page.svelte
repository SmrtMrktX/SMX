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
    let moreorlessT = "more";

    const moreLessTips = () => {
      moreTips = !moreTips;
      if (moreTips) {
        moreorlessT ="less";
      } else {
        moreorlessT ="more";
      }

    };


    let moreHints = false;
    let moreorlessH = "more";

    const moreLessHints = () => {
      moreHints = !moreHints;
      if (moreHints) {
        moreorlessH ="less";
      } else {
        moreorlessH ="more";
      }

    };


    let moreResources = false;
    let moreorlessR = "more";

    const moreLessResources = () => {
      moreResources = !moreResources;
      if (moreResources) {
        moreorlessR ="less";
      } else {
        moreorlessR ="more";
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
      <List tag="ol" list="decimal" class="text-pretty font-bold text-black dark:text-white text-base md:text-lg lg:text-xl">
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
        <Button on:click={moreLessTips} outline color="purple">{moreorlessT}</Button>
      </List>
    </TabItem>


    <TabItem title="Hints">
      <p class="mb-4 text-sm text-gray-500 dark:text-gray-400">
        <b>Hints:</b>
        likely refers to highly advanced and intelligent suggestions or clues provided in a context, often with the goal of assisting or guiding users in a smart and effective way.
      </p>
      <List tag="ol" list="decimal" class="text-pretty font-bold text-black dark:text-white text-base md:text-lg lg:text-xl">
        <Li>
          Quick Fixes:
          <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
            <Li>Instant solutions for common problems or challenges.</Li>
          </List>
        </Li>

        <Li>
          Time-Saving Hints:
          <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
            <Li>Tips to save time in daily activities.</Li>
          </List>
        </Li>

        <Li>
          Memory Boosters:
          <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
            <Li>Techniques to enhance memory and recall.</Li>
          </List>
        </Li>
        
        {#if moreHints}
          <Li>
            Tech Shortcuts:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Keyboard shortcuts for popular software or apps.</Li>
              <Li>Quick tech troubleshooting tips.</Li>
            </List>
          </Li>

          <Li>
            Money-Saving Hacks:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Budget-friendly shopping tips.</Li>
              <Li>Ways to cut costs without sacrificing quality.</Li>
            </List>
          </Li>

          <Li>
            Health Quickies:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Brief exercises for a quick energy boost.</Li>
              <Li>Healthy snacks on the go.</Li>
            </List>
          </Li>

          <Li>
            Career Nuggets:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Bite-sized career advice.</Li>
              <Li>Strategies for a more productive workday.</Li>
            </List>
          </Li>

          <Li>
            Study Snippets:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Memorization techniques for quick learning.</Li>
              <Li>Study hacks for better retention.</Li>
            </List>
          </Li>

          <Li>
            Communication Brevities:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Concise tips for effective communication.</Li>
              <Li>Email etiquette shortcuts.</Li>
            </List>
          </Li>

          <Li>
            Travel Snapshots:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Rapid travel planning tips.</Li>
              <Li>Packing essentials in a nutshell.</Li>
            </List>
          </Li>

          <Li>
            DIY Rapid Fire:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Quick and easy do-it-yourself projects.</Li>
              <Li>Home improvement shortcuts.</Li>
            </List>
          </Li>

          <Li>
            Mindfulness Bites:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Micro-meditations for busy schedules.</Li>
              <Li>Stress-relief techniques in a nutshell.</Li>
            </List>
          </Li>

          <Li>
            Green Living Blurbs:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Easy ways to live more sustainably.</Li>
              <Li>Eco-friendly habits for a quick positive impact.</Li>
            </List>
          </Li>

          <Li>
            Creativity Sparks:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Rapid creativity exercises.</Li>
              <Li>Creative prompts for a quick inspiration boost.</Li>
            </List>
          </Li>

          <Li>
            Media Sips:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Bite-sized book or movie recommendations.</Li>
              <Li>Quick reviews or highlights.</Li>
            </List>
          </Li>
        {/if}

        <div class="my-4"></div>
        <Button on:click={moreLessHints} outline color="purple">{moreorlessH}</Button>
      </List>
    </TabItem>


    <TabItem title="Resources">
      <p class="mb-4 text-sm text-gray-500 dark:text-gray-400">
        <b>Resources:</b>
        refers to the most advanced and efficient tool or system that provides intelligent solutions and comprehensive support across various tasks or challenges.
      </p>
      <List tag="ol" list="decimal" class="text-pretty font-bold text-black dark:text-white text-base md:text-lg lg:text-xl">
        <Li>
          Educational Platforms:
          <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
            <Li>Online courses and certifications.</Li>
            <Li>Learning platforms for various subjects.</Li>
          </List>
        </Li>

        <Li>
          Productivity Tools:
          <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
            <Li>Task management apps.</Li>
            <Li>Collaboration tools for teams.</Li>
          </List>
        </Li>

        <Li>
          Tech Resources:
          <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
            <Li>Coding tutorials and documentation.</Li>
            <Li>Software development tools.</Li>
          </List>
        </Li>
        
        {#if moreResources}
          <Li>
            Financial Resources:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Budgeting apps.</Li>
              <Li>Investment calculators.</Li>
            </List>
          </Li>

          <Li>
            Health and Wellness Apps:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Fitness tracking apps.</Li>
              <Li>Meditation and mindfulness apps.</Li>
            </List>
          </Li>

          <Li>
            Career Development Platforms:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Job search websites.</Li>
              <Li>Resume-building tools.</Li>
            </List>
          </Li>

          <Li>
            Language Learning Resources:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Language learning apps.</Li>
              <Li>Online language exchange platforms.</Li>
            </List>
          </Li>

          <Li>
            Research Databases:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Academic journals and databases.</Li>
              <Li>Research tools for students and professionals.</Li>
            </List>
          </Li>

          <Li>
            Design and Creativity Tools:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Graphic design software.</Li>
              <Li>Creative content creation platforms.</Li>
            </List>
          </Li>

          <Li>
            Travel Planning Websites:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Flight and hotel comparison websites.</Li>
              <Li>Travel itinerary planning tools.</Li>
            </List>
          </Li>

          <Li>
            Environmental and Sustainability Resources:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Eco-friendly product directories.</Li>
              <Li>Environmental awareness campaigns.</Li>
            </List>
          </Li>

          <Li>
            Coding and Development Resources:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Code repositories and version control.</Li>
              <Li>API documentation and tutorials.</Li>
            </List>
          </Li>

          <Li>
            Social Media Marketing Tools:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Analytics platforms.</Li>
              <Li>Social media scheduling tools.</Li>
            </List>
          </Li>

          <Li>
            Science and Technology News Outlets:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Websites for staying updated on the latest scientific discoveries.</Li>
              <Li>Technology news platforms.</Li>
            </List>
          </Li>

          <Li>
            Open Source Software Repositories:
            <List tag="ul" class="ps-5 my-2 space-y-1 text-gray-500 dark:text-gray-400">
              <Li>Platforms for discovering and contributing to open-source projects.</Li>
              <Li>Version control systems</Li>
            </List>
          </Li>
        {/if}

        <div class="my-4"></div>
        <Button on:click={moreLessResources} outline color="purple">{moreorlessR}</Button>
      </List>
    </TabItem>
  </Tabs>
</div>

    

{/if}