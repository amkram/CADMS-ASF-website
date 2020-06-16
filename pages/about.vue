<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="About The Project"
      image="/uploads/hero1.jpeg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="content">
          <h3>About the Project</h3>
          <p>
            
Support for this project is provided by the NSF-USDA-NIH Ecology and Evolution of Infectious Diseases
(EEID) program.
          </p>

          <h3>Overview</h3>
          <p style="float:left">
		  This study will contribute to the understanding of the emergence and complex transmission pathways of
transboundary animal diseases (TADs) at the wildlife-domestic livestock interface. In the last decades
many TADs have been emerging or re-emerging, mostly due to globalization and socio-economic and
environmental changes. This is the case, for example, of African Swine Fever (ASF), a global reemerging
tick-borne hemorrhagic viral disease of swine for which no treatment or vaccine is available. The virus
can result in rapid and widespread mortality, especially in naïve suid populations. Current control
methods are focused on biosecurity and restricting contact with infected and/or wild pigs. When
outbreaks do occur, culling and trade restrictions can result in massive economic losses to producers
and affected countries. The rural poor are often disproportionately affected.
<div class="tile is-ancestor" style="width:50%; float:right; margin-left:10px">
  <div class="tile is-parent">
	<article class="tile is-child box">
	<a href="https://en.wikipedia.org/wiki/Southern_African_Development_Community">
	<img src="@/assets/uploads/SADC.png"></a>
	  <p class="subtitle">
	  Map of Africa indicating SADC (light green) and SADC+SACU (dark green) members.
	  </p>
	</article>
  </div>
</div>

The Southern African Development Community (SADC), an intergovernmental organization, unites 16
southern African countries in an effort to further socio-economic, political and security cooperation. The
community encompassed by the SADC represents the unique area in the world where i) ASFV is believed
to have originated/emerged and continues being an active source of long-distance ASFV spread (e.g., to
Europe in 2007), ii) 23 out of the 24 different ASFV genotypes are present, iii) both the domestic and
sylvatic transmission cycles (involving domestic pigs, wild pigs and ticks) coexist. Moreover, in this
region, more than 80% of the human population is dependent on agriculture, and the presence of ASF
(which causes almost 100% mortality in affected farms) is not only an important cause of poverty and
livelihood deterioration but also a threat to wildlife conservation efforts (i.e., increase of poaching and
bush meat consumption). Despite the importance of this region in ASF viral diversity and local and global
spread, the risk factors and contact networks contributing to ASFV emergence, maintenance and
evolution have been insufficiently studied and ASFV continues spreading to new, previously-free
territories. The characterization of the pig contact networks and the ecologic and socioeconomic factors
contributing to the emergence, maintenance and spread of ASF in the SADC region is an ideal system to
gain understanding about TADs emergence and global spread.

		  </p>


          <h3>Aims</h3>
          <p>The proposed interdisciplinary, multi-institution, research project represents a substantive advance in scope by integrating many scales of research and by linking both ecological and socioeconomic factors influencing disease emergence and transmission. Our approach will be based on intensive field data collection (i.e. wild and domestic pigs and tick sampling, camera traps and surveys conducted in seven study areas of representative SADC countries: Madagascar, South African and Mozambique) and on experimental studies (i.e., ticks competence and variability due to extrinsic and intrinsic factors such as temperature, humidity or tick microbiome).
          </p>

		  <ul>
		  	<li>Assess the pig contact networks within the region</li>
  		  	<li>Collect data on pig management and socio-economic factors characterizing local swine producers</li>
  		  	<li>Explore tick involvement in ASFV transmission</li>
  		  	<li>Assess ASF seroprevalence and viral diversity in the sylvatic and domestic cycles</li>
  		  	<li>Model ASFV transmission dynamics, economic impact and risk of introduction into free areas in different eco-epidemiological settings using multi-scale simulation models</li>
			<li>Integrate genomic-to-population level data and modeling methods into a comprehensive, open-access, user-friendly, long-term, analytical platform referred to as ASF-BioPortal</li>
		  </ul>
<div class="tile is-ancestor" style="width:50%; float:right; margin-left:10px">
  <div class="tile is-parent">
	<article class="tile is-child box">
	<img src="@/assets/uploads/pigs_grass.jpg"></a>
	</article>
  </div>
</div>
		  <h3>Broader Impacts</h3>
<p>It is anticipated that the expected outcomes (better knowledge of factors contributing to disease emergence and transmission dynamics and new modeling, visualization, educational and technology transfer tools) will be directly used by veterinary and public health services in the SADC region to inform the development of more cost-effective preventive and control programs for ASF and other TADs, including those with zoonotic potential, which will lead to a huge positive translational impact in both animal and public health.</p>
<p>The integration of all data, methods and educational materials into the ASFBioPortal will facilitate the analysis and visualization of pig contact networks and ASF-related data. All these will contribute to the vertical advancement in ASF research and will provide a modeling framework and generalizable principles useful for the study of the emergence, prevention and control of many other TADs at a local, continental and global scale.
</p>
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
