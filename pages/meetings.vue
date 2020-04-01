<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="Meetings"
      image="/uploads/about-hero.jpg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="content">
          <h3>Meetings</h3>
 <h2>November 2-5, 2019, Chicago Marriott</h2>
<p> <strong>Conference of Research Workers in Animal Disease (CRWAD)</strong><br>
Chicago Marriott, Downtown Magnificent Mile, <strong>Chicago, Illinois, USA</strong> </p>
 https://crwad.org/crwad2019/


 Drs. Beatriz Martínez-López and Kathleen O’Hara attended the meeting to present a poster outlining our project goals for the year ahead.

 •	March 18-20, 2020
 Kick-off Meeting in Pretoria, South Africa



 •	August 25-27, 2020
 Global African Swine Fever Research Alliance (GARA) 2020 Scientific Meeting in Kampala, Uganda
 https://www.ars.usda.gov/GARA/

 •	December 5-8, 2020
 Conference for Research Workers in Animal Disease, Chicago Marriott, Downtown Magnificent Mile, Chicago, Illinois, USA

 https://crwad.org/2020-crwad-conference/

  </div>

      </template>

      <template v-slot:sidebar>
        <h3 class="subtitle is-4">
          Latest Posts
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
