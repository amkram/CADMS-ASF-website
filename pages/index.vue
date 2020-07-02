<template>
  <div id="home-page" class="page-wrapper home-page">
    <site-hero :title="title" :subtitle="subtitle" :image="featureImage">

      
    </site-hero>
    <main-section theme="one-column">
     
      <template v-slot:default>
      <div class="content">
        <div class="tile is-ancestor" style="width:70%; margin: 0 auto">
  <div class="tile is-parent">
	<article class="tile is-child box">
	<img src="@/assets/uploads/logo_all.png" style="width:100%"></a>

	</article>
  </div>
</div>
<hr>

        <br>
<div class="tile is-ancestor" style="width:50%; float:right; margin-left:10px">
  <div class="tile is-parent">
	<article class="tile is-child box">
	<img src="@/assets/uploads/pig2.jpeg"></a>

	</article>
  </div>
</div>
          <p>African swine fever (ASF) virus is a viral hemorrhagic disease of domestic and wild pigs.  
            Its introduction to naïve populations can result in outbreaks causing up to 100% mortality. 
             Among commercial swine this can result in massive economic losses via high mortality, 
             culling and trade restrictions.  
             Among subsistence farmers, loss of domestic swine can lead to devastating financial hardships and food insecurity. 
              Currently, there is no treatment and no vaccine available.
</p>


<p>
ASF was detected for the first time in China in August 2018.  
Since then the disease has rapidly spread throughout southeast Asia, 
resulting in billions in economic losses and the death of millions of swine.  
Since its reintroduction to Europe through Georgia in 2007, 
the disease has spread north into Russia and has more recently been moving westward through Europe via migration of wild boar reservoir and maintenance in Ornithodoros ticks. 

</p>
<p>
Current control protocols are based on biosecurity, barrier protection, surveillance, 
and stamping out protocols when the disease is discovered. 
 A better understanding of the disease ecology and epidemiology is needed to optimize prevention and control programs.  Our group therefore aims to explore the origins of ASF in the Southern African Development Community (SADC).  Defining the risk factors contributing to the virus’ disease emergence, maintenance and evolution at the wildlife-domestic interface may provide key insights for transboundary animal diseases worldwide.
</p><hr>
      </div>
        
        <!-- All Posts -->
        <posts-grid />
      </template>
      <template v-slot:sidebar>
        Nothing here
      </template>
    </main-section>
    <news-letter-form-modal />
  </div>
</template>

<script>
import { mapState } from 'vuex'
import { setPageData } from '../helper'
import NewsLetterFormModal from '~/components/NewsLetterFormModal'

export default {
  name: 'HomePage',
  head() {
    return {
      title: `Home | ${this.$siteConfig.siteName}`
    }
  },
  components: {
    NewsLetterFormModal
  },
  computed: {
    ...mapState(['title', 'subtitle', 'featureImage'])
  },
  fetch({ store, params }) {
    setPageData(store, { slug: 'home' })
  }
}
</script>

<style>
.home-page .under-subtitle {
  border-top: none;
}
</style>
