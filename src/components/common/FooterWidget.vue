<template>
  <b-col cols="3">
    <h6><slot name="widgettitle"></slot></h6>
    <div>
      <slot name="widgetcontent"></slot>
    </div>
  </b-col>
</template>
<style lang="scss">
#top-footer {
  h6 {
    color: #fff;
    text-transform: uppercase;
    font-weight: 400;
    font-size: 12px;
  }

  a {
    color: #FFFFFF;
    font-size: 11px;
    font-weight: 350;
  }
}
</style>
