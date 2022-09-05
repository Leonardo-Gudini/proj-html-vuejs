<template>
  <header>
    
    <MyNavbar/>

    <MyJumbo/>

  </header>
</template>

<script>
import MyNavbar from "./sub-components/header-components/MyNavbar.vue";
import MyJumbo from "./sub-components/header-components/MyJumbo.vue";

export default {
    name: "MyHeader",
    components: {
    MyNavbar,
    MyJumbo,
}
}
</script>

<style lang="scss">

header{
    background-image: url("@/assets/images/home-background-hero-scaled.jpg"); // JUMBO IMAGE
    background-position: center;
    background-size: cover;
    height: 1000px;
}
    

</style>