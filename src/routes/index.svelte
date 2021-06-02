<script>
  import { onMount } from 'svelte';
  let x, y;

  onMount(async () => {
		// console.log(x, y)
	});
  
</script>


<svelte:window bind:innerWidth={x} bind:innerHeight={y}/>

<header>
  <img src="hero-1440.webp" 
       srcset="hero-780.webp 780w,
               hero-1024.webp 1024w,
               hero-1440.webp 1440w,
               hero-2400.webp 2400w"

       alt="Mapping the post-human city logo"
       >

</header>


<div class="videoWrapper">

  <!-- <video width="100%" controls>
    <source src="output.mp4" type="video/mp4">
  </video> -->

  <iframe 
    src="https://player.vimeo.com/video/554946488" 
    width="640" 
    height="360" 
    frameborder="0" 
    allow="autoplay; fullscreen; picture-in-picture" 
    allowfullscreen>
</iframe>

</div>

<div class="text">
  <div>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A cum, debitis dolore repellendus dolorem quos pariatur voluptas itaque voluptate doloribus labore tempora voluptatem reprehenderit quam non quibusdam fugiat laudantium quasi! Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusantium nostrum vitae officia a aspernatur pariatur perferendis! Id tempore minima nulla commodi adipisci quas nesciunt consequatur quae, perferendis labore alias hic! <br><br> Lorem, ipsum dolor sit amet consectetur adipisicing elit. A cum, debitis dolore repellendus dolorem quos pariatur voluptas itaque voluptate doloribus labore tempora voluptatem reprehenderit quam non quibusdam fugiat laudantium quasi! Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusantium nostrum vitae officia a aspernatur pariatur perferendis! Id tempore minima nulla commodi adipisci quas nesciunt consequatur quae, perferendis labore alias hic!</div>
  <div>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A cum, debitis dolore repellendus dolorem quos pariatur voluptas itaque voluptate doloribus labore tempora voluptatem reprehenderit quam non quibusdam fugiat laudantium quasi! Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusantium nostrum vitae officia a aspernatur pariatur perferendis! Id tempore minima nulla commodi adipisci quas nesciunt consequatur quae, perferendis labore alias hic! <br><br> Lorem, ipsum dolor sit amet consectetur adipisicing elit. A cum, debitis dolore repellendus dolorem quos pariatur voluptas itaque voluptate doloribus labore tempora voluptatem reprehenderit quam non quibusdam fugiat laudantium quasi! Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusantium nostrum vitae officia a aspernatur pariatur perferendis! Id tempore minima nulla commodi adipisci quas nesciunt consequatur quae, perferendis labore alias hic!</div>
</div>

<footer>

  <div class="credits">
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Architecto voluptatibus odit facilis delectus, consequatur culpa officia dolor laborum cumque, perferendis iste molestiae dolorem doloribus quos aliquid sint ea, modi molestias?
  </div>

  <div class="logos">
    <div>
      <img src="arch+_logo-200.png" 
          srcset="arch+_logo-150.png 780w,
                  arch+_logo-200.png 1024w"
      alt="">
    </div>

    <div>
      <img src="mfn-logo-200-white.png" 
            srcset="mfn-logo-150-white.png 780w,
                    mfn-logo-200-white.png 1024w"
      
      alt="">
    </div>

  </div>

</footer>


<style>


  :global(body){
    margin: 0;
    padding: 0;
  }

  header{
    background-color: #000;
  }

  video {
    width: 100%    !important;
    height: auto   !important;
  }

  
  .videoWrapper {
    position: relative;
    padding-bottom: 56.25%; /* 16:9 */
    height: 0;
  }

  .videoWrapper iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
  }

  .text {
    display: flex;
    flex-direction: row;
    font-family: "Roboto", sans-serif;
    font-weight: 700;
    font-size: 1.5em;
    color: #fff;
    background-color: #000;
    padding: 1em 0;
  }

  .text div {
    padding: 2em;
  }


  footer {
    display: flex;
    flex-direction: row;
    background: rgb(0, 0, 0);
  }

  footer div {
    flex: 1;
    padding: 2em;
  }

  .credits {
    font-family: "Roboto", sans-serif;
    font-weight: 300;
    font-size: 1em;
    color: #fff;
    display: flex;
    align-items: center;
  }

  .logos {
    display: flex;
    flex-direction: row;
    align-items: center;
  }


  @media (max-width: 800px) {

  .text {
    flex-direction: column;
    font-size: 1em;
  }

  .text div {
    padding: 1em;
  }

  footer {
    flex-direction: column;
  }

  footer div {
    padding: 1em;
  }

  /* .logos {
    flex-direction: column;
  } */


}


</style>