<template>
  <main>
    <PopDishes/>
    <MenuCat/>
    <OrderApp/>
    <LateNews/>
  </main>
</template>

<script>
import PopDishes from './sub-components-main/PopDishes.vue';
import MenuCat from './sub-components-main/MenuCat.vue';
import OrderApp from './sub-components-main/OrderApp.vue';
import LateNews from './sub-components-main/LateNews.vue';

export default {
    name: "MyMain",
  components: {
    PopDishes,
    MenuCat,
    OrderApp,
    LateNews
}
}
</script>

<style lang="scss">

  @import "@/style/main.scss";

</style>