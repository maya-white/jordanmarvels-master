<template>
  <div>
    <b-navbar
      toggleable="lg"
      type
      variant
      class="justify-content-md-center justify-content-start p-0 position-relative"
    >
      <div class="brand-left position-absolute">
        <b-navbar-nav class="d-inline-block">
          <b-nav-item-dropdown text="Lang" right class="text-uppercase">
            <b-dropdown-item href="#">EN</b-dropdown-item>
            <b-dropdown-item href="#">ES</b-dropdown-item>
            <b-dropdown-item href="#">RU</b-dropdown-item>
            <b-dropdown-item href="#">FA</b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>
        <b-navbar-brand href="#">
          <b-img src="../../assets/logo.png" fluid alt="Fluid image"></b-img>
        </b-navbar-brand>
      </div>
      <b-navbar-nav class="text-uppercase main-nav">
        <b-nav-item href="#" active>Home</b-nav-item>
        <b-nav-item href="#">Destinations</b-nav-item>
        <b-nav-item href="#">Stores</b-nav-item>
        <b-nav-item href="#">About Us</b-nav-item>
        <b-nav-item href="#">Help</b-nav-item>
      </b-navbar-nav>

      <!-- <b-navbar-nav>
        <b-nav-item-dropdown text="Lang" right>
          <b-dropdown-item href="#">EN</b-dropdown-item>
          <b-dropdown-item href="#">ES</b-dropdown-item>
          <b-dropdown-item href="#">RU</b-dropdown-item>
          <b-dropdown-item href="#">FA</b-dropdown-item>
        </b-nav-item-dropdown> 
      </b-navbar-nav>
      <b-navbar-brand href="#">NavBar</b-navbar-brand>-->

      <!-- <b-navbar-toggle target="nav-collapse"></b-navbar-toggle> -->
      <div class="brand-right position-absolute">
        <b-navbar-nav class="d-inline-block">
          <b-nav-item-dropdown text="USD" right class="text-uppercase">
            <b-dropdown-item href="#">INR</b-dropdown-item>
            <b-dropdown-item href="#">SGD</b-dropdown-item>
            <b-dropdown-item href="#">EURO</b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>
        <b-navbar-nav class="d-inline-block">
          <b-nav-item-dropdown text="SIGN UP" right class="text-uppercase"></b-nav-item-dropdown>
        </b-navbar-nav>
        <b-navbar-nav class="d-inline-block">
          <b-nav-item-dropdown text="GET APP" right class="text-uppercase"></b-nav-item-dropdown>
        </b-navbar-nav>
      </div>
    </b-navbar>
  </div>
</template>
<style lang="scss">
.brand-left {
  left: 0;
  top: 0;
  .navbar-brand {
    margin-left: 20px;
  }
}
.brand-right {
  right: 0;
  top: 0;
}

#nav {
  .navbar-nav {
    &.main-nav {
      .nav-link {
        color: #000;
        padding: 30px 15px;
        border-top: 4px solid transparent;
        &.active {
          border-top: 4px solid #c7b298;
          color: #c7b298;
        }
        &:hover {
          border-top: 4px solid #c7b298;
        }
      }
    }
  }
}
#nav {
  .brand-left,
  .brand-right {
    .navbar-nav {
      .nav-link {
        color: #000;
        padding: 35px 15px;
        font-size: 12px;
        font-weight: bold;
      }
    }
    ul {
      li {
        border-right: 1px solid #e0e0e0;
      }
    }
  }
}
</style>