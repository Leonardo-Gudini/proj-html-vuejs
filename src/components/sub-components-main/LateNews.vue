<template>
    <section class="late-news">
            <div class="container">

                <div class="title-section">
                    <h2>Latest News</h2>
                    <button class="btn-standard">read more news <i class="fa-regular fa-circle-right"></i></button>
                </div>
            

                <ul>
                    <li v-for="(news, index) in lateNews" :key="index">
                        <img :src="require(`@/assets/images/${news.img}`)" :alt="news.title">
                        <h2>{{news.title}}</h2>
                        <p>{{news.text}}</p>
                    </li>
                </ul>
            </div>

    </section>
  </template>
  
  <script>
  export default {
      name: "LateNews",
      data(){
          return{

            lateNews:[
                {
                    img: 'pancake-burger-600x450.jpg',
                    title: 'NEW: The Pancake Burger',
                    text: 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Officiis illum deserunt suscipit optio ipsa perspiciatis provident, eum quam excepturi obcaecati eaque similique impedit rem animi praesentium. Vero id quas minus?'
                },
                {
                    img: 'new-milkshake-menu-600x450.jpg',
                    title: 'New Milkshake Menu',
                    text: 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Officiis illum deserunt suscipit optio ipsa perspiciatis provident, eum quam excepturi obcaecati eaque similique impedit rem animi praesentium. Vero id quas minus?'
                },
            ]
  
          }
      }
  
  }
  </script>
  
  <style lang="scss">
  
  </style>