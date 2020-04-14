<template>
  <b-row class="text-left">
    <b-col cols="2"></b-col>
    <b-col cols="8">
      <div id="banner">
        <b-row class="ban-row">
          <b-col cols="4" class="ban-item">
            <h6>Where</h6>
            <b-link>Anywhere in Jordan</b-link>
          </b-col>
          <b-col cols="5" class="ban-item">
            <b-row>
              <b-col cols="6">
                <h6>START DATE</h6>
                <h5>Thu, Feb, 20</h5>
              </b-col>
              <b-col cols="6">
                <h6>END DATE</h6>
                <h5>Fri, Feb, 28</h5>
              </b-col>
            </b-row>
          </b-col>
          <b-col cols="2" class="ban-item">
            <h6>TRAVELLERS</h6>
            <h5>3 travellers</h5>
          </b-col>
          <b-col cols="1"></b-col>
        </b-row>
      </div>
    </b-col>
    <b-col cols="2"></b-col>
  </b-row>
</template>

<style lang="scss">
#banner {
  vertical-align: middle;
  height: 120px;
  background-color: #ffffff;
  margin-top: -60px;
  border: 1px solid #C7B299;
  border-radius: 5px;
  padding: 0px 15px;
  
  .ban-row {
    height: 100%;
  }

  .ban-item {
    border-right: 1px solid #e0e0e0;
    padding: 35px 15px;
  }
}
</style>