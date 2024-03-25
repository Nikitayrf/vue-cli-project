<template>
  <div id="app">
    <div class="top">
      <HeaderComponent />
      <HeroComponent />
      <ProjectComponent />
      <CounterComponent />
      <BlogComponent />
      <FooterComponent />

      <HeaderComponent />
      <BannerComponent />
      <BlogBigComponent />
      <FooterComponent />

      <HeaderComponent />
      <BannerTopComponent />
      <div id="blog-details" class="blog-details">
        <ArticleComponent />
      </div>

      <FooterComponent />

    </div>
  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue'
import HeroComponent from './components/HeroComponent.vue'
import ProjectComponent from './components/ProjectComponent.vue'
import CounterComponent from './components/CounterComponent.vue'
import BlogComponent from './components/BlogComponent.vue'
import BlogBigComponent from './components/BlogBigComponent.vue'
import BannerTopComponent from './components/BannerTopComponent.vue'
import ArticleComponent from './components/ArticleComponent.vue'


import BannerComponent from './components/BannerComponent.vue'
import FooterComponent from './components/FooterComponent.vue'

export default {
  name: 'App',
  components: {
    HeaderComponent,
    HeroComponent,
    ProjectComponent,
    CounterComponent,
    BlogComponent,

    BannerComponent,
    BlogBigComponent,
    BannerTopComponent,
    ArticleComponent,
    FooterComponent
  },
}
</script>