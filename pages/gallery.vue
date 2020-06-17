<template>
  <div id="gallery-page" class="page-wrapper about-page content-page">
    <site-hero
      title="Gallery"
      image="/uploads/pig2.jpeg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="content">
          <h3>Shared Box Folder</h3>
          Feel free to share photos and other documents in our shared Box folder.<br>
          <br><br><iframe src="https://ucdavis.app.box.com/embed/s/4wh25tjih3fzp35l4maal11m5olmcdax?sortColumn=date&view=list" width="900" style="height: 650px !important;" frameborder="0" allowfullscreen webkitallowfullscreen msallowfullscreen></iframe>
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
