<script>
  import { Blockquote, Card } from "flowbite-svelte";

  import { QuoteSolid, GiftBoxSolid, ArrowUpRightFromSquareOutline } from 'flowbite-svelte-icons';

  import UltimateExplore from "$lib/Components/UltimateExplore.svelte";
</script>



<svelte:head>
  <title>SMX © SMRT MRKT X : Simple Life  السوق الذكية : حياة بسيطة</title>
  <meta name="description" content="Discover the secrets to earning passive and direct income through cryptocurrency at SMX © SMRT MRKT X | السوق الذكية
  Access expert tips, strategies, and real-time insights on lucrative crypto opportunities. Join our community to stay ahead in the dynamic world of digital assets and unlock your path to financial freedom."/>
</svelte:head>





<div class=" spec  flex flex-col justify-center items-center text-center mt-24">

  <Blockquote alignment="center" size="lg" class="opacity-90">
    <QuoteSolid class="w-8 h-8 text-gray-800 dark:text-gray-200" />
      <span style="font-family: 'Russo One', sans-serif;" 
      class="font-medium tracking-wider text-gray-800 dark:text-gray-200  leading-relaxed md:leading-loose ">
        Awesome opensource
        <a style="font-family: 'Russo One', sans-serif;" href="https://github.com/SmrtMrktX/SMX" target="_blank" 
        class="text-black dark:text-white rounded hover:font-extrabold ">
        ©</a>
      </span>
  </Blockquote>

  <h1 class="backdrop-blur-sm text-black dark:text-white py-2 px-4 rounded-full shadow-2xl dark:shadow-inner dark:shadow-blue-800 welcome font-extrabold leading-10  text-2xl md:text-3xl lg:text-4xl m-auto">
    Welcome to our 
    <a style="font-family: 'Russo One', sans-serif;" href="/digital" 
    class="rounded-md px-1 text-blue-600  hover:no-underline hover:text-blue-700 shadow-inner dark:shadow-blue-900 shadow-blue-600 hover:shadow-none ">
      digital
    </a>
    home!
  </h1>

  
  <Card class="hover:scale-105 bg-transparent backdrop-blur-sm dark:bg-transparent dark:backdrop-blur-sm">
    <GiftBoxSolid class="w-7 h-7  text-gray-500 dark:text-gray-400" />
    <a href="/bonus/passiveIncome">
      <h5 class="mb-2 text-2xl font-semibold tracking-tight text-primary-customBlack dark:text-primary-customSmoke hover:font-bold hover:text-primary-customLime">
        Passive Income Bonus</h5>
    </a>
    <p class="mb-3 font-normal text-gray-500 dark:text-gray-400">Go to this step by step guideline process on how to certify for your benefits:</p>
    <a href="/bonus" class="inline-flex items-center text-primary-customLime hover:underline">
      See our guideline
      <ArrowUpRightFromSquareOutline class="w-3 h-3 ms-2.5" />
    </a>
  </Card>  

</div>



<UltimateExplore />



<div style="font-weight:700;" class="rounded-md py-10 my-10 flex-col justify-center items-center text-center leading-loose tracking-wide font-extralight shadow-md border-t-4 dark:border-none dark:shadow-inner dark:shadow-customColorW">
  
   
  <h1 class="pb-10 text-2xl md:text-3xl lg:text-4xl font-extrabold">
    We're thrilled to have
    <span style="font-family: 'Russo One', sans-serif;" class="font-normal text-primary-customLime">
      you
    </span>
    here,
  </h1>

  <div  class="my-20 text-lg md:text-xl lg:text-2xl max-w-4xl justify-center items-center mx-auto">
    <h2 class="my-20">where curiosity meets discovery and every click unveils a world of possibilities.</h2>

    <h2 class="my-20"> Whether you're a seasoned explorer or a newcomer seeking inspiration, our site is designed with you in mind.</h2>

    <h2 class="my-20"> Dive into our collection of articles, resources, and insights crafted to ignite your imagination and satisfy your thirst for knowledge.</h2>

    <h2 class="my-20"> From informative guides to thought-provoking content, embark on a journey where learning knows no bounds.</h2>
  </div>


  <div  class="backdrop-blur-sm  font-mono my-32 px-0 mx-2 md:mx-auto max-w-3xl text-lg md:text-xl lg:text-2xl border-2 border-primary-customLime rounded-xl shadow-lg dark:shadow-black">
      
    <h3 class="p-1"><span style="font-family: 'Russo One', sans-serif;color:lime;">#Join us</span> as we traverse the digital realm together, exploring, learning, and growing.</h3>
  
    <h3 class="p-1"><span class="text-purple-600">#Your presence</span> enriches our virtual haven, and we're excited to share this digital adventure with you.</h3>
    
  </div>


  <h1 class="px-2 my-10 font-extrabold text-lg md:text-xl lg:text-2xl hover:underline">
    Welcome, fellow seeker, to our corner of the web!
  </h1>




</div>

<h1 style="font-family: 'Russo One', sans-serif;color:lime;"
class="flex justify-center items-center text-center font-extrabold backdrop-blur-md  rounded-full w-44 mx-auto  text-xs italic tracking-widest leading-loose">
  SMX™ Simple Life
</h1>



<style>



  .spec {
    height: 70vh;
    max-height: 777px;

  }


  @media screen and (max-width: 320px) {
      /* Your CSS styles here */
      .spec {
        margin-top:50px;
        height: 90vh;
      }
      .welcome {
        font-size:1.4rem;
      }
  }

  @media screen and (max-height: 375px) {
      /* Your CSS styles here */
      .spec {
        margin-top:40px;
        height: 120vh;
      }
  }


</style>