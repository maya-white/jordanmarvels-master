<template>
  <b-col cols="4" class="traveling">
    <div class="travel-wrap">
      <h1 class="heading text-left">Traveling with us</h1>
      <div class="home-beniffit">
        <ul>
          <li>
            Discover Genuine
            <br />Experiences
          </li>
          <li>
            Secure and
            <br />Safe Payments
          </li>
          <li>
            Give back and
            <br />Have Fun
          </li>
        </ul>
      </div>
      <book-now-btn>All Benefits</book-now-btn>
    </div>
  </b-col>
</template>
<script>
import Button from "../common/Button";
export default {
  components: {
    "book-now-btn": Button
  }
};
</script>
<style lang="scss">
.travel-wrap {
  position: relative;
  a {
    position: absolute;
    bottom: -10px;
    right: 30px;
  }
}
.home-beniffit {
  background: #c7b298;
  padding: 40px 40px 100px 40px;
  clip-path: polygon(0 0, 100% 0, 100% 100%, 0 90%);
  ul {
    margin: 0;
    padding: 0;
    list-style: none;
    li {
      padding-left: 90px;
      color: #3b352d;
      font-size: 20px;
      font-weight: bold;
      text-align: left;
      margin-bottom: 30px;
      &:nth-child(1) {
        background: url(../../assets/discover.png) no-repeat -12px;
        background-size: 30%;
      }
      &:nth-child(2) {
        background: url(../../assets/secure.png) no-repeat center left;
        background-size: 20%;
      }
      &:nth-child(3) {
        background: url(../../assets/havefun.png) no-repeat center left;
        background-size: 21%;
      }
    }
  }
}
</style>
