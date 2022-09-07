<template>
  <div class="jumbo">
    <div class="jumbo-text">
        <h1>
          <span class="txt-sm">Hungry?</span> <br>
          <span class="jumbo-colored">Great Food</span><br>
          Delivered<br>
        </h1>
        
        <button class="btn-standard">view our menu <span><i class="fa-regular fa-circle-right"></i></span></button>
    </div>

    <InfoCard/>
  </div>
</template>

<script>
import InfoCard from './InfoCard.vue';
export default {
    name: "MyJumbo",
    components: {
    InfoCard
}
}
</script>

<style lang="scss">
  
</style>