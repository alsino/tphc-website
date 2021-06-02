<script>
  import { onMount } from 'svelte';
  let x, y;

  onMount(async () => {
		console.log(x, y)
	});
  
</script>


<svelte:window bind:innerWidth={x} bind:innerHeight={y}/>

<header>
  <!-- <img src="https://via.placeholder.com/1440" alt=""> -->
  <img src="hero-1440.webp" 
       srcset="hero-780.webp 780w,
               hero-1024.webp 1024w,
               hero-1440.webp 1440w,
               hero-2400.webp 2400w"

       alt="Mapping the post-human city logo"
       >

   
       <!-- <img src="https://www.mediaevent.de/html/img/needles-1440.jpg" > -->
</header>


<div class="videoWrapper">

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
  <div>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A cum, debitis dolore repellendus dolorem quos pariatur voluptas itaque voluptate doloribus labore tempora voluptatem reprehenderit quam non quibusdam fugiat laudantium quasi! Lorem ipsum dolor sit amet consectetur adipisicing elit. <br><br> Accusantium nostrum vitae officia a aspernatur pariatur perferendis! Id tempore minima nulla commodi adipisci quas nesciunt consequatur quae, perferendis labore alias hic!</div>
  <div>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A cum, debitis dolore repellendus dolorem quos pariatur voluptas itaque voluptate doloribus labore tempora voluptatem reprehenderit quam non quibusdam fugiat laudantium quasi! Lorem ipsum dolor sit amet consectetur adipisicing elit. <br><br>Accusantium nostrum vitae officia a aspernatur pariatur perferendis! Id tempore minima nulla commodi adipisci quas nesciunt consequatur quae, perferendis labore alias hic!</div>
</div>

<!-- <footer>
  <div>Lorem ipsum dolor sit amet consectetur adipisicing elit. Architecto voluptatibus odit facilis delectus, consequatur culpa officia dolor laborum cumque, perferendis iste molestiae dolorem doloribus quos aliquid sint ea, modi molestias?</div>
  <img src="https://via.placeholder.com/150" alt="">

</footer> -->


<style>


  :global(body){
    margin: 0;
    padding: 0;
  }

  header{
    background-color: #000;
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
    font-family: "Roboto", sans-serif;
    font-weight: 700;
    font-size: 2em;
    color: #fff;
    background-color: #000;
  }

  .text div {
    padding: 2em;
  }

  footer {
    display: flex;

  }


</style>