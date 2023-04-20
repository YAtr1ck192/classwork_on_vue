<template>
  <div id="app">
    <backgroundBlock id="background"/>
    <headerBlock/>
    <postsSection/>
    <readMoreBlock id="readMoreBlock" />
    <featuredStories />
    <footerBlock />
  </div>
</template>

<script>
import backgroundBlock from "@/components/background-block.vue";
import headerBlock from "@/components/header-block.vue";
import postsSection from "@/components/posts-section.vue";
import readMoreBlock from "@/components/read-more-block.vue";
import featuredStories from "@/components/featured-stories.vue";
import footerBlock from "@/components/footer-block.vue";
export default {
  name: 'App',
  components: {
    backgroundBlock,
    headerBlock,
    postsSection,
    readMoreBlock,
    featuredStories,
    footerBlock
  }
}
</script>

<style>
  #readMoreBlock {
    margin-bottom: 185px;
  }
  @import 'css/global_styles.css';
</style>
