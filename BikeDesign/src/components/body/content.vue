<template>
  <div class="container">
    <v-row>
      <v-col cols="6">
        <v-img
          :aspect-ratio="1"
          class="bg-white"
          src="../../assets/product/pr1.jpg"
          width="700"
          cover
        ></v-img>
      </v-col>
      <v-col cols="6">
        <div class="content">
          <h1>Step into Style: Discover the Ultimate Sneaker Collection</h1>
          <h4>
            Experience the perfect blend of style and comfort with our latest
            sneaker collection, designed for those who step up their game every
            day.
          </h4>
        </div>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.container {
  height: 100vh;
  padding: 160px 40px;
}
.content{
    padding: 200px;
}
</style>
