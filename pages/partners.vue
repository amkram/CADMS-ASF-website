<template>
  <div id="partners-page" class="page-wrapper about-page content-page">
    <site-hero
      title="Partners"
      image="/uploads/about-hero.jpg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="content">
          <h3>Directors</h3>
		  <div class="tile is-ancestor" style="width:45%; float:left; margin-left:10px">
		    <div class="tile is-parent">
		  	<article class="tile is-child box">

		  	<img src="@/assets/uploads/contact-person.png">
		  	  <p class="subtitle">
			  <strong>Project Director</strong><br>
		  	   Beatriz Martínez López<br>
			   University of California, Davis (UCD)
		  	  </p>
		  	</article>
		    </div>
		  </div>
		  <div class="tile is-ancestor" style="width:50%; float:left; margin-left:10px">
		    <div class="tile is-parent">
		  	<article class="tile is-child box">

		  	<img src="@/assets/uploads/etter.png">
		  	  <p class="subtitle" style="float:right">
			  <strong>Co-Project Director</strong><br>
		  	  Eric Etter<br>
			   Centre de coopération internationale en recherche agronomique pour le développement (CIRAD)
		  	  </p>
		  	</article>
		    </div>
			</div>
			<br>
			<h3>Partners</h3>
			<div class="tile is-ancestor" style="width:45%; float:left; margin-left:10px">
  		    <div class="tile is-parent">
  		  	<article class="tile is-child box">

  		  	<img src="@/assets/uploads/logo.png">
  		  	  <p class="subtitle">
  			   University of California, Davis (UCD)<br>
			   Led by Beatriz Martínez López
  		  	  </p>
  		  	</article>
  		    </div>
  		  </div>
  		  <div class="tile is-ancestor" style="width:55%; float:right; margin-left:10px">
  		    <div class="tile is-parent">
  		  	<article class="tile is-child box">

  		  	<img src="@/assets/uploads/cirad.jpg">
  		  	  <p class="subtitle" style="float:left">
  			   Centre de coopération internationale en recherche agronomique pour le développement (CIRAD)
			   <br>Led by Eric Etter
			  </p>
  		  	</article>
  		    </div>
  			</div>

			<div class="tile is-ancestor" style="width:45%; float:left; margin-left:10px">
  		    <div class="tile is-parent">
  		  	<article class="tile is-child box">

  		  	<img src="@/assets/uploads/UP.png">
  		  	  <p class="subtitle">
  			   University of Pretoria, South Africa (UP)<br>
			   Led by Armanda Bastos
  		  	  </p>
  		  	</article>
  		    </div>
  		  </div>

  		  <div class="tile is-ancestor" style="width:45%; float:left; margin-left:10px">
  		    <div class="tile is-parent">
  		  	<article class="tile is-child box">

  		  	<img src="@/assets/uploads/iiam.jpg">
  		  	  <p class="subtitle" style="float:right">
  			   Instituto de Investigação Agrária de Moçambique (IIAM)
			   <br>Led by Carlos Quembo
			  </p>
  		  	</article>
  		    </div>
  			</div>


			<div class="tile is-ancestor" style="width:45%; float:left; margin-left:10px">
  		    <div class="tile is-parent">
  		  	<article class="tile is-child box">

  		  	<img src="@/assets/uploads/UCM.png">
  		  	  <p class="subtitle">
  			   Universidad Complutense de Madrid (UCM)<br>
			   Led by José Manuel Sànchez Vizcaíno
  		  	  </p>
  		  	</article>
  		    </div>
  		  </div>

  		  <div class="tile is-ancestor" style="width:45%; float:left; margin-left:10px">
  		    <div class="tile is-parent">
  		  	<article class="tile is-child box">

  		  	<img src="@/assets/uploads/uem.jpg">
  		  	  <p class="subtitle" style="float:right">
  			   Eduardo Mondlane Unversity, Mozambique (EUM)
			   <br>Led by Jose Fafetine
			  </p>
  		  	</article>
  		    </div>
  			</div>

			<div class="tile is-ancestor" style="width:45%; float:left; margin-left:10px">
  		    <div class="tile is-parent">
  		  	<article class="tile is-child box">

  		  	<img src="@/assets/uploads/ovi.jpg">
  		  	  <p class="subtitle">
  			   Onderstepoort Veterinary Institute, Agricultural Research Council (OVI)<br>
			   Led by Juanita van Heerden
  		  	  </p>
  		  	</article>
  		    </div>
  		  </div>


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
