<template>
  <section class="pop-dishes">
    <h2>Our Most Popular Dishes</h2>

    <ul>
        <li v-for="(dishe, index) in dishes" :key="index">
            <img :src="'@/assets/images/' + dishe.img" alt="dishe.title">
            <h3>{{dishe.title}}</h3>
            <h4>{{dishe.price}}</h4>
        </li>
    </ul>

    <button class="btn-standard">start your order <span><i class="fa-regular fa-circle-right"></i></span> </button>
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
                    price: '$3.00-$6.00'
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