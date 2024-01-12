<!-- Myname.svelte -->
<script>
  
  import { onMount } from "svelte";
  export let text = '';
  export let delay = 100;
  
  let animatedText = "";
    
  function animateText() {
    
    const letters = text.split("");
    let i = 0;
      
    const intervalId = setInterval(() => {
      if (i >= letters.length) {
        clearInterval(intervalId);
      } else {
        animatedText += letters[i];
        i++;
      }
    }, delay);
  }
    
  // Run the animation when the component is mounted
  onMount(animateText);

</script>
  




<h1 style="font-family: 'Russo One', sans-serif;">{animatedText}</h1>
  