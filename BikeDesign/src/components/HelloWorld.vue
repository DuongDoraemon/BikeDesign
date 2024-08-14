<template>
  <div>
    <HeaderComponent />
    <Content />
    <BannerContent />
    <ContentTwo/>
  </div>
</template>

<script>
import HeaderComponent from "../components/header/header.vue";
import Content from "../components/body/content.vue";
import BannerContent from "../components/body/bannerContent.vue";
import ContentTwo from "../components/body/contentTwo.vue"
export default {
  components: {
    HeaderComponent,
    Content,
    BannerContent,
    ContentTwo
  },
};
//
</script>
