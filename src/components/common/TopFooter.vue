<template>
  <div id="top-footer" class="text-left">
    <b-container>
      <b-row>
        <footer-widget>
          <template v-slot:widgettitle>
            Destinations
          </template>
          <template v-slot:widgetcontent>
            <div><a href="#">Petra</a></div>
            <div><a href="#">Dead Sea</a></div>
            <div><a href="#">Ammon</a></div>
            <div><a href="#">Magic Bedouin Star</a></div>
          </template>
        </footer-widget>
        <footer-widget>
          <template v-slot:widgettitle>
            ABOUT US
          </template>
          <template v-slot:widgetcontent>
            <div><a href="#">Our agenda</a></div>
            <div><a href="#">Benefits</a></div>
            <div><a href="#">Contact</a></div>
          </template>
        </footer-widget>
        <footer-widget>
          <template v-slot:widgettitle>
            HELP
          </template>
          <template v-slot:widgetcontent>
            <div><a href="#">Payments</a></div>
            <div><a href="#">Frequenty Asked Questions</a></div>
            <div><a href="#">Support Service</a></div>
            <div><a href="#">Guarantee</a></div>
          </template>
        </footer-widget>
        <b-col cols="3">
          <b-img src="../../assets/footer-logo.png" fluid alt="Fluid image"></b-img>
          <b-img src="../../assets/visa.png" fluid alt="Fluid image"></b-img>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
import footerWidget from "./FooterWidget";
export default {
  name: "TopFooter",
  components: {
    "footer-widget": footerWidget
  }
};
</script>

<style lang="scss">
#top-footer {
  background: #4a4642;
  padding: 50px 0;
}
</style>
