<template>
  <div id="news-page" class="page-wrapper about-page content-page">
    <site-hero
      title="Training"
      image="/uploads/about-hero.jpg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="content">
          <h3>Coming Soon</h3>
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
