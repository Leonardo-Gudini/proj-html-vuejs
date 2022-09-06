<template>
    <section class="menu-cat">

        <div class="container">

            <div class="title-section">
                <h2>Menu Categories</h2>
                <button class="btn-standard">view the full menu</button>
            </div>

            <ul>
                <li v-for="(menu, index) in menus" :key="index">
                    <img :src="require(`@/assets/images/${menu.img}`)" :alt="menu.title">
                    <h5>{{menu.title}}</h5>
                </li>
            </ul>

            <ul>
                <li>
                    <div>
                        
                    </div>
                    <h5></h5>
                </li>
            </ul>
        </div>
    </section>
  </template>
  
  <script>
  export default {
      name: "MenuCat",
      data(){
          return{

            menus:[
                {
                    img: 'appetizers-menu-background.jpg',
                    title: 'appetiziers'
                },
                {
                    img: 'burgers-menu-background.jpg',
                    title: 'burgers'
                },
                {
                    img: 'pizza-menu-background.jpg',
                    title: 'pizzas'
                },
                {
                    img: 'fries-menu-background.jpg',
                    title: 'fries'
                },
                {
                    img: 'sides-menu-background.jpg',
                    title: 'sides'
                },
                {
                    img: 'desserts-menu-background.jpg',
                    title: 'desserts'
                },
                {
                    img: 'beverages-menu-background.jpg',
                    title: 'beverages'
                },
                {
                    img: 'specials-menu-background.jpg',
                    title: 'specials'
                },
            ]
  
          }
      }
  
  }
  </script>
  
  <style lang="scss">
  
  </style>