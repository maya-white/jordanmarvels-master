<template>
  <div id="featured-in">
    <div class="position-relative top-heading">
      <h6>Jordan Marvels Has Been Fetures In</h6>
    </div>
    <b-container class="jordan-featured-wrap">
      <b-row>
        <b-col>
          <carousel :items="4" :nav="false" :dots="false" :margin="20">
            <img src="../../assets/freatured-1.jpg" />

            <img src="../../assets/freatured-2.jpg" />

            <img src="../../assets/freatured-3.jpg" />

            <img src="../../assets/freatured-4.jpg" />
          </carousel>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>
<script>
import carousel from "vue-owl-carousel2";
export default {
  components: { carousel }
};
</script>
<style lang="scss">
#featured-in {
  .top-heading {
    position: relative;
    &::after {
      content: "";
      width: 100%;
      border-top: 1px solid #c7b298;
      position: absolute;
      left: 0;
      top: 11px;
    }
  }
  h6 {
    position: relative;
    text-transform: uppercase;
    color: #c7b298;
    font-weight: bold;
    padding: 0 20px;
    background: #fff;
    display: inline-block;
    z-index: 2;
  }
}
.jordan-featured-wrap {
  padding: 40px 0;
}
</style>
