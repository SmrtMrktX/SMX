<script>

</script>



<section class="font-extrabold text-2xl ">
	
    <div id="loading">
        <div class="waviy">
 <span style="--i:1">C</span>&nbsp
 <span style="--i:2">O</span>&nbsp
 <span style="--i:3">M</span>&nbsp
 <span style="--i:4">I</span>&nbsp
 <span style="--i:5">N</span>&nbsp
 <span style="--i:6">G</span>&nbsp
 <span style="--i:7">&nbsp</span>&nbsp
 <span style="--i:9">S</span>&nbsp
 <span style="--i:10">O</span>&nbsp
 <span style="--i:11">O</span>&nbsp
 <span style="--i:12">N</span>
        </div>
    </div>

</section>



<style>



section{
  /* font-family: 'Ubuntu', sans-serif; */
  font-family: 'Russo One', sans-serif;
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

@keyframes flip {
  0%,80% {
    transform: rotateY(360deg) 
  }
}
@keyframes invertColor {
  0% {
    filter: invert(0); /* Initial color */
  }
  100% {
    filter: invert(1); /* Inverted color */
  }
}

.waviy {
  position: relative;
}

.waviy span {
  position: relative;
  display: inline-block;
  animation: invertColor 2s linear 60, flip 1s linear 60; /* Adjust durations and iterations as needed */
  animation-delay: calc(.1s * var(--i));
}

/* .waviy span {
  position: relative;
  display: inline-block;
  animation: flip 1s 60;
  animation-delay: calc(.1s * var(--i))
} */



</style>