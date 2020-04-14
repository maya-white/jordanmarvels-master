<template>
  <b-col cols="8" class="mood">
    <h1 class="heading text-left">What's your mood?</h1>
    <b-row>
      <b-col cols="6">
        <figure>
          <b-img src="../../assets/0011.png" fluid alt="Responsive image"></b-img>
          <figcaption>
            <h1>Gateway with friends</h1>
            <b-link>86 Destinations</b-link>
          </figcaption>
        </figure>
      </b-col>
      <b-col cols="6">
        <figure>
          <b-img src="../../assets/0012.png" fluid alt="Responsive image"></b-img>
          <figcaption>
            <h1>Gateway with friends</h1>
            <b-link>86 Destinations</b-link>
          </figcaption>
        </figure>
      </b-col>
      <b-col cols="6">
        <figure>
          <b-img src="../../assets/0013.png" fluid alt="Responsive image"></b-img>
          <figcaption>
            <h1>Gateway with friends</h1>
            <b-link>86 Destinations</b-link>
          </figcaption>
        </figure>
      </b-col>
      <b-col cols="6">
        <figure>
          <b-img src="../../assets/0014.png" fluid alt="Responsive image"></b-img>
          <figcaption>
            <h1>Gateway with friends</h1>
            <b-link>86 Destinations</b-link>
          </figcaption>
        </figure>
      </b-col>
    </b-row>
  </b-col>
</template>

<style lang="scss">
.mood {
  .row {
    margin-left: -10px;
    margin-right: -10px;
  }
  .col-6 {
    padding-left: 10px;
    padding-right: 10px;
    figure {
      margin-bottom: 20px;
      position: relative;
      figcaption {
        position: absolute;
        text-align: right;
        bottom: 0;
        width: 100%;
        padding: 20px;
        h1 {
          color: #fff;
          font-size: 24px;
          font-weight: bold;
        }
        a {
          color: #fff;
          text-decoration: none;
          text-transform: uppercase;
          display: inline-block;
          position: relative;
          padding-right: 15px;
          &::before {
            content: "";
            position: absolute;
            width: 30px;
            left: -40px;
            border-top: 1px solid #d5d5d5;
            top: 50%;
          }
          &::after {
            content: ">";
            position: absolute;

            right: 0px;
          }
        }
      }
    }
  }
}
</style>