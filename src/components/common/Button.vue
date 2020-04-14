<template>
  <b-link class="book-now"><slot></slot></b-link>
</template>

<style lang="scss">
a {
  &.book-now {
    background: #f1ece5;
    display: inline-block;
    color: #000;
    font-weight: bold;
    text-decoration: none;
    border-radius: 5px;
    padding: 12px 40px 12px 20px;
    text-transform: uppercase;
    font-size: 14px;
    position: relative;
    &::after {
      content: ">";
      position: absolute;
      right: 20px;
      font-size: 16px;
      line-height: 16px;
    }
    &:hover {
      background: #f3c01b;
    }
  }
}
</style>
