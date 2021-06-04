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
  
  <div>
    <h2>Mapping the Post-Human City</h2>
    Theoretiker*innen wie Donna Haraway und Anna Lowenhaupt Tsing entwickelten in den letzten Jahrzehnten ein neues Bewusstsein dafür, dass der Mensch sich nur in interaktiven Beziehungen zu anderen Spezies entwickeln konnte. Diese Perspektive macht neue Politik- und Subjektvorstellungen jenseits des neoliberalen Individualismus denkbar. Doch was das für die Frage des städtischen Raums bedeuten könnte, wurde bisher nur wenig reflektiert. Um diese Blickverschiebung anzustoßen, erzeugt <span class="italic">Mapping the Post-Human City</span> neue Visualisierungen für eine Stadt, in der nicht-menschlichen Lebensformen eine bedeutende Rolle zugesprochen wird und ein solidarisches Zusammenleben möglich wird. 
    <br><br> 
    In einer umfassenden Kartierung wird die Präsenz nicht-menschlicher Spezies im Berliner Stadtraum untersucht und sichtbar gemacht. Aus unterschiedlichen Datenquellen werden Karten generiert, die insbesondere auf neue Beziehungsmuster zwischen Mensch und Tieren hindeuten, jenseits von klassischem Naturschutzdenken und der Antithese von Stadt und Land. Kernfragen sind: Wie bedingen sich Stadt und Natur gegenseitig? Welche von Menschen erschaffenen städtischen Infrastrukturen bieten neue Lebensräume für Tiere? Quellen sind eigene Recherchen, aber auch die Naturblick App (Museum für Naturkunde), öffentliche Geoinformationsportale und naturwissenschaftliche Monitorings.
  </div>
  <div>
    Neben diesen Kartierungen helfen Videos die nicht-menschlichen Spezies als städtische Akteure ins Bewusstsein zu rücken. Neuronale Netze generieren Videos aus bestehenden Citizen Science-Datenarchiven, um eine visuelle Bestandsaufname städtischer Natur zu generieren. Die Videos funktionieren als eine Art virtuelles Gedächtnis punktuell ausgewählter Orte der Berliner Stadtnatur. Anhand dieser Videos wird aufgezeigt, wie algorithmische Netzwerke die Natur ›sehen‹, aber dabei auch neue Realitäten kreieren. Die Videos testen die realitätsbildenden Effekte der KI und den Einsatz als künstlerisches Werkzeug, um die wachsenden Datenarchive von Citizen-Science-Projekten experimentell auszuwerten und sichtbar zu machen.
    <br><br> 
    Für <span class="italic">Mapping the Post-Human City</span> kreiert <span class="italic">Pollinations in Blatant Space</span> aus dem Tierstimmenarchiv des Museums für Naturkunde eine durch maschine-learning-generierte Klanginstallation, die mit den Videos und Karten korrespondiert und von diesen mit Hilfe von Cycle-GANs lernt.
    <br><br>
    Zu sehen ist die Arbeit in der von ARCH+ mitinitiierten Ausstellung »Cohabitation: Ein Manifest für Solidarität von Tieren und Menschen im Stadtraum«, im silent green Kulturquartier Berlin, Gerichtstraße 35, 13347 Berlin vom 5. Juni bis 4. Juli 2021.
    <br><br> 
    Die Arbeit ist in enger Kooperation mit dem Naturkundemuseum Berlin realisiert.
  </div>
</div>

<footer>

  <div class="credits">
    Mapping the Post-Human City, 2021 <br>
    Moritz Ahlert & Alsino Skowronnek, 4-Kanal-Videoinstallation, 8 min,
    in Kollaboration mit <span class="italic">Pollinations in Blatant Space</span> (Thomas Haferlach, Adrien Bitton & Niels Warnecke), Sound 8 min
    Mit Unterstützung von: Gareth Davies (Übersetzung), Max Pfeffer (Assistenz – Ausstellungsarchitektur), Marie Schuster – Bureau Est (Logo), Ludwig Thanhäuser (Assistenz – Karten), Anna-Lena Wenzel (Lektorat).
  </div>

  <div class="logos">
    <div>
      <img src="arch+_logo-150.png" 
          srcset="arch+_logo-150.png 1x,
                  arch+_logo-150@2x.png 2x"
      alt="">
    </div>

    <div>
      <img src="mfn-logo-150-white.png" 
            srcset="mfn-logo-150-white.png 1x,
                    mfn-logo-150-white@2x.png 2x"
      
      alt="">
    </div>

  </div>

</footer>


<style>


  :global(body){
    margin: 0;
    padding: 0;
    font-family: "tacticregular";
    font-weight: normal; 
    font-style: normal;
  }

  :global(#svelte){
    overflow: hidden;
  }

  header{
    background-color: #000;
  }

  video {
    width: 100%    !important;
    height: auto   !important;
  }

  h2 {
    margin: 0 0 1em 0;
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
    padding-bottom: 2em;
  }

  footer div {
    flex: 1;
    padding: 2em;
  }

  .credits {
    font-weight: 300;
    font-size: 1em;
    color: #fff;
    align-items: center;
  }

  .logos {
    display: flex;
    flex-direction: row;
    align-items: center;
  }

  .italic {
    font-family: "tacticitalic";
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

  h2 {
    font-size: 1.4em;
    margin: 1em 0;
  }

}


</style>