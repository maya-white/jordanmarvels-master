<template>
  <div>
    <div>
      <b-carousel
        id="carousel-1"
        :interval="4000"
        indicators
        background="#ababab"
        img-width="1024"
        img-height="300"
        style="text-shadow: 1px 1px 2px #333;"
      >
        <!-- Slide with blank fluid image to maintain slide aspect ratio -->
        <b-carousel-slide img-blank img-alt="Blank image">
          <template v-slot:img>
            <img
              class="d-block img-fluid w-100"
              width="1024"
              height="480"
              src="../assets/banner.jpg"
              alt="image slot"
            />
          </template>
        </b-carousel-slide>
        <b-carousel-slide img-blank img-alt="Blank image">
          <template v-slot:img>
            <img
              class="d-block img-fluid w-100"
              width="1024"
              height="480"
              src="../assets/banner.jpg"
              alt="image slot"
            />
          </template>
        </b-carousel-slide>
      </b-carousel>
    </div>
    <div id="slide_title">
      <p>Book your authentic trip,</p>
      <p>get the unique experience</p>
    </div>
    <div id="slide_img">
      <b-img src="../assets/slide_img.png" fluid alt="slide img"></b-img>
    </div>
    <div id="slide_img_title">
      <p class="mpp">MOST POPULAR</p>
      <p class="alkp">Al- Khaznoh, Petra</p>
      <p class="disc">DISCOVER DESTINATION ></p>
    </div>
    <banner></banner>
    <section>
      <b-container class="pt-4">
        <b-row>
          <mood></mood>
          <traveling></traveling>
        </b-row>
      </b-container>
    </section>
    <featured></featured>
    <section>
      <premium-experience></premium-experience>
    </section>
    <section>
      <travellers-use></travellers-use>
    </section>
    <section>
      <featured-in></featured-in>
    </section>
  </div>
</template>

<script>
import Banner from "../components/home/Banner";
import Mood from "../components/home/Mood.vue";
import Traveling from "../components/home/Traveling.vue";
import Featured from "../components/home/Featured";
import PremiumExperience from "../components/home/PremiumExperience";
import TravellersUse from "../components/home/TravellersUse";
import FeaturedIn from "../components/home/FeaturedIn";
export default {
  name: "Home",
  components: {
    banner: Banner,
    mood: Mood,
    traveling: Traveling,
    featured: Featured,
    "premium-experience": PremiumExperience,
    "travellers-use": TravellersUse,
    "featured-in": FeaturedIn
  }
};
</script>
<style lang="scss">
#slide_title {
  position: absolute;
  left: 150px;
  top: 220px;
  text-align: left;
  font-family: Poppins;
  font-style: normal;
  font-weight: bold;
  font-size: 58px;
  line-height: 87px;

  margin-top: -30px;
  color: #ffffff;
}
#slide_img {
  position: absolute;
  left: 900px;
  top: 420px;
}
#slide_img_title {
  position: absolute;
  left: 1000px;
  top: 420px;
  text-align: left;

  color: #ffffff;

  .mpp {
    font-size: 12px;
  }

  .alkp {
    font-size: 17px;
  }

  .disc {
    font-size: 10px;
  }
}
</style>
