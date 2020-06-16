<template>
  <div id="news-page" class="page-wrapper about-page content-page">
    <site-hero
      title="News"
      image="/uploads/pig4.jpeg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="content">
          <h3>Publications</h3>
		</div>
		<p>
			Pereira de Oliveira R, Hutet E, Paboeuf F, Duhayon M, Boinas F, Perez de Leon A, et al. 
			(2019) Comparative vector competence of the Afrotropical soft tick Ornithodoros 
			moubata and Palearctic species, O. erraticus and O. verrucosus, 
			for African swine fever virus strains circulating in Eurasia. 
			PLoS ONE 14(11): e0225657. 
			<a href="https://doi.org/10.1371/journal.pone.0225657">https://doi.org/10.1371/journal.pone.0225657</a>
			<a href="https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0225657">https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0225657</a>
			</p>
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
