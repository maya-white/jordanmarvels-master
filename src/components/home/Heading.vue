<template>
  <b-container>
    <b-row class="align-items-center">
      <b-col cols="9"
        ><h1 class="heading text-left">{{ heading }}</h1></b-col
      >
      <b-col cols="3 text-right">
        <a class="btnlink" :href="`${btnLink}`">{{ btnText }} </a>
      </b-col>
    </b-row>
  </b-container>
</template>

<style lang="scss"></style>
<script>
export default {
  name: "Heading",
  props: {
    heading: String,
    btnText: String,
    btnLink: String
  }
};
</script>

<style lang="scss">
.btnlink {
  padding-right: 30px;
  margin-right: 20px;
  display: inline-block;
  color: #50473d;
  font-weight: bold;
  text-decoration: none;
  text-transform: uppercase;
  position: relative;
  font-size: 13px;
  &::after {
    content: ">";
    position: absolute;
    right: 0;
  }
  &:hover {
    text-decoration: none;
  }
}
</style>
