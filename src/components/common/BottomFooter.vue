<template>
  <div>
    <b-container>
      <b-row id="bottom-footer">
        <b-col cols="3">
          <b-img src="../../assets/footer_1.png" fluid alt="Fluid image"></b-img>
        </b-col>
        <b-col cols="3">
          <b-img src="../../assets/footer_2.png" fluid alt="Fluid image"></b-img>
        </b-col>
        <b-col cols="3">
          <b-img src="../../assets/footer_3.png" fluid alt="Fluid image"></b-img>
        </b-col>
        <b-col cols="3">
          <b-img src="../../assets/footer_4.png" fluid alt="Fluid image"></b-img>
        </b-col>
      </b-row>
      <b-row>
        <b-col cols="6" class="text-left">Copyright 2020. All Rights Reserved.</b-col>
        <b-col cols="6" class="text-right bt-footer-term">
          <a href="#">TERMS OF USE</a>
          <a href="#">PRIVACY POLICY</a>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {
  name: "BottomFooter"
};
</script>

<style lang="scss">
#bottom-footer {
  background: #FFFFFF;
  padding: 50px 0;
}
.bt-footer-term {
  a {
    margin-left: 15px;
    color: #000000;
    font-size: 11px;
    font-weight: 350;
  }
}
</style>
