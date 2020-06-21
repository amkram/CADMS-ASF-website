<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="Meetings"
      image="/uploads/hero4.jpg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="content">
		<div class="tile is-ancestor" style="width:80%; float:left; margin-left:10px">
		  <div class="tile is-parent">
		   <article class="tile is-child box">
		   <h3>Next Meeting</h3>
			 <p class="subtitle" style="font-size: 12pt">
			 <strong><a href="https://www.ars.usda.gov/GARA/">Global African Swine Fever Research Alliance</a> (GARA) 2020 Scientific Meeting</strong>
			 <br>August 25-27<br>
			 Kampala, Uganda
			 </p>
		   </article>
		  </div>
		</div>
          <h3 style="clear:both">All Meetings</h3>

 <h4 style="clear: both; padding-top:25px">November 2-5, 2019</h4>
<p> <strong><a href="https://crwad.org/crwad2019/"">Conference of Research Workers in Animal Disease</a> (CRWAD)</strong>
<br>Chicago Marriott, Downtown Magnificent Mile, Chicago, Illinois, USA </p>
 <br><br>

		  <h4>March 18-20, 2020</h4>
		  <div class="tile is-ancestor" style="width:40%; float:left; margin-left:10px">
		    <div class="tile is-parent">
		  	<article class="tile is-child box">
		  	<img src="@/assets/uploads/SAkickoff.png">
			<p class="subtitle" style="font-size: 12pt"> Kick-off Meeting in Pretoria, South Africa</p>
		  	</article>
		    </div>
		  </div>
<br><br><br>

		 <h4 style="clear:both">August 25-27, 2020</h4>
		 <strong><a href="https://www.ars.usda.gov/GARA/">Global African Swine Fever Research Alliance</a> (GARA) 2020 Scientific Meeting</strong>
		 <br>Kampala, Uganda
<br><br><br>


		  <h4>December 5-8, 2020</h4>
		 <strong><a href="https://crwad.org/2020-crwad-conference/">Conference for Research Workers in Animal Disease</a> (CRWAD)</strong><br>
		 Chicago Marriott, Downtown Magnificent Mile, Chicago, Illinois, USA
</p>

 <div class="tile is-ancestor" style="width:40%; float:left; margin-left:10px">
   <div class="tile is-parent">
 	<article class="tile is-child box">
 	<a href="https://crwad.org/wp-content/uploads/2019/10/CRWAD-2019-Author-Index-and-Abstracts.FINAL_.pdf">
 	<img src="@/assets/uploads/crwad19.png"></a>
 	  <p class="subtitle" style="font-size: 12pt">
	  Drs. Beatriz Martínez-López and Kathleen O’Hara attended the meeting to present a poster outlining our project goals for the year ahead.
 	  </p>
 	</article>
   </div>
 </div>

 		 <h4 style="clear:both">March 23-26, 2021</h4>
		 <strong><a href="https://wildboarsymposium.com/">International Symposium on Wild Boar and Other Suids </a></strong>
		 <br>Seva, Barcelona
<br><br><br>



  </div>

      </template>

	  <template v-slot:sidebar>
	    <h3 class="subtitle is-4">
	  	News
	    </h3>
	    <posts-grid :per-row="1" :number="2" />
	  </template>
	  </main-section>
	  </div>
	  </template>
<script>
import SadcCard from '~/components/cards/SadcCard'
export default {
  head() {
    return {
      title: `About | ${this.$siteConfig.siteName}`
    }
  },
  components: { SadcCard }
}
</script>
