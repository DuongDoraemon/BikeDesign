<template>
  <div class="banner">
     <video autoplay muted loop class="banner-video">
      <source src="../../assets/media/baner2.mp4" type="video/mp4" />
    </video>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.banner {
  position: relative;
  width: 100%;
  /* margin-top: 10vh;  */
  height: 100vh;
  overflow: hidden;
}
.banner-video {
  position: absolute;
  top: 50%;
  left: 50%;
  min-width: 100%;
  min-height: 100%;
  width: auto;
  transform: translate(-50%, -50%);
  z-index: 1;
  object-fit: cover;
}
</style>