<script>

</script>



<section class="font-extrabold text-2xl ">
	
  <div id="loading">
    <div class="waviy">
      <span style="--i:1">L</span>&nbsp
      <span style="--i:2">O</span>&nbsp
      <span style="--i:3">A</span>&nbsp
      <span style="--i:4">D</span>&nbsp
      <span style="--i:5">I</span>&nbsp
      <span style="--i:6">N</span>&nbsp
      <span style="--i:7">G</span>&nbsp
      <span style="--i:9">&nbsp</span>&nbsp
      <span style="--i:10">.</span>&nbsp
      <span style="--i:11">.</span>&nbsp
      <span style="--i:12">.</span>
    </div>
  </div>

</section>



<!-- <h6 class="text-xl text-purple-700 dark:text-primary-customYellow">Coming soon.</h6> -->




<style>


  section{
    font-family: 'Ubuntu', sans-serif;
    justify-content:center;
    align-content:center;
    align-items:center;
    text-align:center;
    margin:auto;
  }




  #loading {
    
    display: flex;
    justify-content: center;
    align-items: center;
    /* min-height: 50vh; */
  }



  .waviy {
    position: relative;
  }



  .waviy span {
    position: relative;
    display: inline-block;
    animation: flip 3s infinite;
    animation-delay: calc(.3s * var(--i))
  }



  

  @keyframes flip {
    0%,80% {
      transform: rotateY(360deg) 
    }
  }




  h6{
    
    font-family: 'Russo One', sans-serif;;
    
    
    /* color: #CFC547; */
    text-align: center;
    letter-spacing: 5px;
    
  }



</style>