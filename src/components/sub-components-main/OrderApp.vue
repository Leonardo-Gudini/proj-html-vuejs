<template>
    <section class="order-app">
        <div class="container">

            <div class="app-text">
                
                <h3>Download Our</h3>
                <h2>Ordering App</h2>

                <div class="mobile-store">
                    <div v-for="(mobile, index) in mobileApp" :key="index">
                        <img :src="require(`../../assets/images/${mobile.img}`)" :alt="mobile.txt">
                    </div>
                </div>
            </div>
        </div>
    </section>
  </template>
  
  <script>
  export default {
      name: "OrderApp",
      data(){
          return{

            mobileApp: [
                {
                    img: 'app-store-badge-200x67.png',
                    txt: 'app-store'
                },
                {
                    img: 'play-store-badge-200x67.png',
                    txt: 'google-play-store'
                }
            ]
  
          }
      }
  
  }
  </script>
  
  <style lang="scss">
  
  </style>