<template>
  <div class="jumbo">
    <div>
        <h1>great food delivered</h1>
        
        <MyButton/>
    </div>
  </div>
</template>

<script>
import MyButton from '../MyButton.vue';
export default {
    name: "MyJumbo",
    components: { 
      MyButton, 
    }
}
</script>

<style lang="scss">
  .jumbo{
        color: white;
    }
</style>