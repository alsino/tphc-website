<script>
	import { onMount } from 'svelte';
	let lang = "en"

	onMount(async () => {
		// lang = 'en';
	});

	function setLang(){
		console.log("clicked")
	}

</script>

<header>
	<img
		src="hero-1440.webp"
		srcset="hero-780.webp 780w,
               hero-1024.webp 1024w,
               hero-1440.webp 1440w,
               hero-2400.webp 2400w"
		alt="Mapping the post-human city logo"
	/>
</header>

<div class="videoWrapper">
	<!-- <video width="100%" controls>
    <source src="output.mp4" type="video/mp4">
  </video> -->

	<iframe
		src="https://player.vimeo.com/video/687072699?h=bd94c07404&amp;title=0&amp;byline=0&amp;portrait=0&amp;speed=0&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479"
		width="1280"
		height="720"
		frameborder="0"
		allow="autoplay; fullscreen; picture-in-picture"
		allowfullscreen
		title="Mapping The Post-Human City"
	/>
</div>


<div class="switch" >
	<div class="pointer" class:active={lang == "en"} on:click={() => { lang = "en"}}>en</div>
	<div class="pointer" class:active={lang == "de"} on:click={() => { lang = "de"}}>de</div>
</div>

{#if lang === 'de'}
<!-- german version -->
<div class="text">
		<div>
			<h2>Mapping the Post-Human City</h2>
			»Theoretiker*innen wie Donna Haraway und Anna Lowenhaupt Tsing entwickelten in den letzten Jahrzehnten
			ein neues Bewusstsein dafür, dass der Mensch sich nur in interaktiven Beziehungen zu anderen Spezies
			entwickeln konnte. Diese Perspektive macht neue Politik- und Subjektvorstellungen jenseits des
			neoliberalen Individualismus denkbar. Doch was das für die Frage des städtischen Raums bedeuten
			könnte, wurde bisher nur wenig reflektiert. Um diese Blickverschiebung anzustoßen, erzeugt <span class="italic">
			Mapping the Post-Human City</span> neue Visualisierungen für eine Stadt, in der nicht-menschlichen Lebensformen eine bedeutende Rolle zugesprochen wird und ein solidarisches Zusammenleben möglich wird.«
			<br /><br />
			In einer umfassenden Kartierung wird die Präsenz nicht-menschlicher Spezies im Berliner Stadtraum
			untersucht und sichtbar gemacht. Aus unterschiedlichen Datenquellen werden Karten generiert, die
			insbesondere auf neue Beziehungsmuster zwischen Mensch und Tieren hindeuten, jenseits von klassischem
			Naturschutzdenken und der Antithese von Stadt und Land. Kernfragen sind: Wie bedingen sich Stadt
			und Natur gegenseitig? Welche von Menschen erschaffenen städtischen Infrastrukturen bieten neue
			Lebensräume für Tiere? Quellen sind eigene Recherchen, aber auch die Naturblick App (Museum für
			Naturkunde), öffentliche Geoinformationsportale und naturwissenschaftliche Monitorings.
		</div>
		<div>
			Neben diesen Kartierungen helfen Videos die nicht-menschlichen Spezies als städtische Akteure
			ins Bewusstsein zu rücken. Neuronale Netze generieren Videos aus bestehenden Citizen
			Science-Datenarchiven, um eine visuelle Bestandsaufname städtischer Natur zu generieren. Die
			Videos funktionieren als eine Art virtuelles Gedächtnis punktuell ausgewählter Orte der
			Berliner Stadtnatur. Anhand dieser Videos wird aufgezeigt, wie algorithmische Netzwerke die
			Natur ›sehen‹, aber dabei auch neue Realitäten kreieren. Die Videos testen die
			realitätsbildenden Effekte der KI und den Einsatz als künstlerisches Werkzeug, um die
			wachsenden Datenarchive von Citizen-Science-Projekten experimentell auszuwerten und sichtbar
			zu machen.
			<br /><br />
			Für <span class="italic">Mapping the Post-Human City</span> kreiert
			<span class="italic">Pollinations in Blatant Space</span>
			aus dem Tierstimmenarchiv des Museums für Naturkunde eine durch machine learning generierte Klanginstallation,
			die mit den Videos und Karten korrespondiert und von diesen mit Hilfe von Cycle-GANs lernt.
			<br /><br />
			Zu sehen war die Arbeit in der von ARCH+ mitinitiierten Ausstellung
			<a target="_blank" href="https://archplus.net/de/cohabitation/"
				>»Cohabitation: Ein Manifest für Solidarität von Tieren und Menschen im Stadtraum«</a
			>, im silent green Kulturquartier Berlin, Gerichtstraße 35, 13347 Berlin vom 5. Juni bis 4.
			Juli 2021.
			<br /><br />
			Die Arbeit wurde in enger Kooperation mit dem Naturkundemuseum Berlin realisiert.
		</div>
</div>

<footer>
	<div class="credits">
		<h4 class="italic">Mapping the Post-Human City, 2021</h4>
		<br />
		<a target="_blank" href="https://www.moritzahlert.de/">Moritz Ahlert</a> &
		<a target="_blank" href="https://alsino.io">Alsino Skowronnek</a>, 4-Kanal-Videoinstallation, 8
		min, in Kollaboration mit <span class="italic">Pollinations in Blatant Space</span> (Thomas Haferlach),
		Sound 8 min Mit Unterstützung von: Gareth Davies (Übersetzung), Max Pfeffer (Assistenz – Ausstellungsarchitektur),
		Marie Schuster – Bureau Est (Logo), Ludwig Thanhäuser (Assistenz – Karten), Anna-Lena Wenzel (Lektorat).
		<br>
		Fotos: © Alsino Skowronnek & Dotgain.Info, 2021.
	</div>

	<div class="logos">
		<div>
			<img
				src="arch+_logo-150.png"
				srcset="arch+_logo-150.png 1x,
                  arch+_logo-150@2x.png 2x"
				alt=""
			/>
		</div>

		<div>
			<img
				src="mfn-logo-150-white.png"
				srcset="mfn-logo-150-white.png 1x,
                    mfn-logo-150-white@2x.png 2x"
				alt=""
			/>
		</div>
	</div>
</footer>
{:else if lang === "en"}
<!-- english version -->
<div class="text">
	<div>
		<h2>Mapping the Post-Human City</h2>
		»In recent decades, theorists such as Donna Haraway and Anna Lowenhaupt Tsing have developed a new awareness that humans could only develop in interactive relationships with other species. This perspective makes new concepts of politics and subjects beyond neoliberal individualism conceivable. However, what this could mean for the question of urban space has so far received little reflection. In order to initiate this shift in perspective, <span class="italic">Mapping the Post-Human City</span> creates new visualizations for a city in which non-human life forms are given an important role and in which solidarity is made possible.«

		<br /><br />
		In a comprehensive mapping, the presence of non-human species in Berlin's urban space is examined and made visible. Maps are generated from different data sources, which point in particular to new relationship patterns between humans and animals, beyond classic nature conservation thinking and the antithesis of city and country. Key questions are: How do city and nature condition each other? Which man-made urban infrastructures offer new habitats for animals? Sources are our own research, but also the Naturblick app (Museum of Natural History), public geoinformation portals and scientific monitoring.
	</div>
	<div>
		Alongside these maps, videos help to raise awareness of non-human species as urban actors. Neural networks generate videos from existing citizen science data archives to generate a visual inventory of urban nature. The videos function as a kind of virtual memory of selectively selected places in Berlin's urban nature. These videos show how algorithmic networks ›see‹ nature, but also create new realities. The videos test the reality-building effects of AI and its use as an artistic tool to experimentally evaluate and visualize the growing data archives of citizen science projects.
		<br /><br />
		For <span class="italic">Mapping the Post-Human City</span>, <span class="italic">Pollinations in Blatant Space</span> uses the animal sound archive of the Museum für Naturkunde to create a sound installation generated by machine learning that corresponds to the videos and maps and learns from them with the help of Cycle-GANs.

		<br /><br />
		The piece could be seen in the exhibition 	<a target="_blank" href="https://archplus.net/de/cohabitation/"
		> »Cohabitation: A Manifesto for Solidarity of Animals and Humans in Urban Space«</a
		>, co-initiated by ARCH+, in the silent green Kulturquartier Berlin, Gerichtstraße 35, 13347 Berlin from June 5th to July 4th, 2021.
		<br /><br />
		The work was realized in close cooperation with the Natural History Museum Berlin.
	</div>
</div>


<div class="text space-around">

		<div>
			<img
				src="/img/1.jpg"
				srcset="/img/1.jpg 1x, /img/1@2x.jpg 2x"
				alt="Bild 1"
				/>
		</div>
	
		<div>
			<img
			src="/img/2.jpg"
			srcset="/img/2.jpg 1x, /img/2@2x.jpg 2x"
			alt="Bild 2"
			/>
	</div>

</div>

<div class="text space-around">

	<div>
		<img
		src="/img/3.jpg"
		srcset="/img/3.jpg 1x, /img/3@2x.jpg 2x"
		alt="Bild 3"
		/>
	</div>

	<div>
		<img
		src="/img/4.jpg"
		srcset="/img/4.jpg 1x, /img/4@2x.jpg 2x"
		alt="Bild 4"
		/>
	</div>

</div>




<footer>
<div class="credits">
	<h4 class="italic">Mapping the Post-Human City, 2021</h4>
	<br />
	<a target="_blank" href="https://www.moritzahlert.de/">Moritz Ahlert</a> &
	<a target="_blank" href="https://alsino.io">Alsino Skowronnek</a>, 4-channel video installation, 8 min, in collaboration with Pollinations in Blatant Space (Thomas Haferlach, sound). With the support of: Gareth Davies (translation), Max Pfeffer (assistance - exhibition design), Marie Schuster – Bureau Est (Logo design), Ludwig Thanhäuser (Assistant – Maps), Anna-Lena Wenzel (Editing).
	<br>
	Photo credits: © Alsino Skowronnek & Dotgain.Info, 2021.
</div>

<div class="logos">
	<div>
		<img
			src="arch+_logo-150.png"
			srcset="arch+_logo-150.png 1x,
								arch+_logo-150@2x.png 2x"
			alt=""
		/>
	</div>

	<div>
		<img
			src="mfn-logo-150-white.png"
			srcset="mfn-logo-150-white.png 1x,
									mfn-logo-150-white@2x.png 2x"
			alt=""
		/>
	</div>
</div>

</footer>
{/if}

<style>
	:global(body) {
		margin: 0;
		padding: 0;
		font-family: 'tacticregular';
		font-weight: normal;
		font-style: normal;
	}

	:global(#svelte) {
		overflow: hidden;
	}

	header {
		background-color: #000;
	}

	h2 {
		margin: 0 0 1em 0;
	}

	a {
		color: #fff;
		text-decoration: underline;
	}

	img {
		width: 100%;
  	height: auto;
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

	.switch {
		display: flex;
		flex-direction: row;
		font-weight: 700;
		font-size: 1.5em;
		color: #fff;
		background-color: #000;
		padding: 1em 0;
	}

	.switch div {
		padding: 1em 2em;
	}

	.space-around {
		justify-content: space-around;
	}

	

	footer {
		display: flex;
		flex-direction: row;
		background: rgb(0, 0, 0);
		padding-bottom: 2em;
	}

	footer div {
		flex: 1;
		padding: 3em;
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
		font-family: 'tacticitalic';
	}

	.pointer {
		cursor: pointer;
	}

	.active {
		text-decoration: underline;
	}


	@media (max-width: 800px) {
		.text {
			flex-direction: column;
			font-size: 1em;
			padding-top: 0;
		}

		.text div {
			padding: 1em;
		}

		.switch {
			font-size: 1em;
		}

		.switch div {
			padding: 0.5em 1em;
		}

		footer {
			flex-direction: column;
		}

		footer div {
			padding: 1em;
		}

		h2 {
			font-size: 1.2em;
			margin: 1em 0;
		}
	}
</style>
