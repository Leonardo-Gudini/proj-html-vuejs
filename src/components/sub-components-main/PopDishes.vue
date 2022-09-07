<template>
  <section class="pop-dishes">
    <h2>Our Most Popular Dishes</h2>

    <ul>
        <li v-for="(dish, index) in dishes" :key="index">
            <img :src="require(`@/assets/images/${dish.img}`)" :alt="dish.title">
            <h3>{{dish.title}}</h3>
            <h4>{{dish.price}}</h4>
        </li>
    </ul>

    <button class="btn-standard">start your order <span><i class="fa-regular fa-circle-right"></i></span> </button>

    <div class="discount-background">
        <img src="@/assets/images/svg-0.svg" alt="svg">
        <img class="op-30" src="@/assets/images/svg-0.svg" alt="svg">
        <img class="op-25" src="@/assets/images/svg-0.svg" alt="svg">
        <img class="op-20" src="@/assets/images/svg-0.svg" alt="svg">
    </div>
  </section>
</template>

<script>
export default {
    name: "PopDishes",
    data(){
        return{
            dishes: [
                {
                    img: 'skin-on-fries-400x571.jpg',
                    title: 'Skin On Fries',
                    price: '$3.00 - $6.00'
                },
                {
                    img: 'choco-cookie-frappe-400x571.jpg',
                    title: 'Chocco Cookie Frappe',
                    price: '$4.99'
                },
                {
                    img: 'donut-burger-400x571.jpg',
                    title: 'The Donut Burger',
                    price: '$6.99'
                },
            ]
        }
    }

}
</script>

<style lang="scss">
    @import "@/style/main.scss";
</style>