<template>
  <header>
    
    <div class="container">
      <MyNavbar/>
      <MyJumbo/>
    </div>

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

  @import "@/style/header.scss";
  @import "@/style/general.scss"

</style>