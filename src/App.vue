<template>
  <div id="app">

    <!-- Header -->
    <HeaderComponent />

    <!-- Main -->
    <MainComponent />

    <!-- Footer -->
    <FooterComponent />
  </div>
</template>

<script>
import HeaderComponent from "./components/HeaderComponent";
import  MainComponent  from "./components/MainComponent";
import  FooterComponent  from "./components/FooterComponent";

export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainComponent,
    FooterComponent
  }
}
</script>

<style lang="scss">
@import "./style/common.scss";

</style>
