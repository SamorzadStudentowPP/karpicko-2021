<template>
  <div id="hero">
    <v-parallax dark src="@/assets/1.png" height="750" style="top:2px;">
      <v-row align="center" justify="center" class="mt-n12">
        <v-col class="text-center" cols="12">
          <v-img
            src="@/assets/other/Karpicko_White_Logo_2021.png"
            contain
            max-height="400"
          ></v-img>
          <h2 class="display-0">
            Zapisy rozpoczęte!
          </h2>
        </v-col>
      </v-row>
    </v-parallax>
  </div>
</template>

<script>
export default {
  name: 'HomeHero',
};
</script>

<style scoped>
#hero {
  margin-top: -80px;
}
</style>
