<template>
  <footer>

    <div class="footer-container">

      <div class="footer-list">
        <ul>
          <li><h4>order online</h4></li>
          <li v-for="(order, index) in orders" :key="index">{{order.title}}</li>
        </ul>
        
        <ul class="navigate">
          <li><h4>navigate</h4></li>
          <li class="firstGold" v-for="(nav, index) in navs" :key="index">{{nav.title}}</li>
        </ul>

        <div class="information">
          <ul>
            <li><h4>information</h4></li>
            <li v-for="(info, index) in infos" :key="index">{{info.title}}</li>
          </ul>

          <div  v-for="(bedge, index) in bedges" :key="index">
            <img class="bedge" :src="require(`@/assets/images/${bedge.img}`)" :alt="bedge.txt">
          </div>
        </div>

        <ul>
          <li><h4>opening hours</h4></li>
          <li class="openings" v-for="(opening, index) in openings" :key="index">{{`${opening.day} - `}} <span>{{`${opening.time}`}}</span> </li>
        </ul>

        <div class="voucher">
          <h4>vouchers</h4>
          <img src="@/assets/images/footer-coupon-200x200.png" alt="coupon">
          <p>Just Use The Code <br> <span>firstorder</span> <br> At Checkout</p>
        </div>

      </div>

      <div class="footer-form">
        <img src="@/assets/images/takeout-logo-2x-200x43.png" alt="takeout logo">
        <h2>Stay In The Loop</h2>
        <p>Sign up to receive up to date news and offers dirctly in your inbox:</p>
        <input type="email" name="" id="" placeholder="you@email.com">
        <button type="submit" class="btn-large">Subscribe</button>

        <div class="social-container">
          <ul>
            <li v-for="(social, index) in socials" :key="index">
              <i :class="social.icon"></i>
            </li>
          </ul>
        </div>
      </div>
    </div>

  </footer>
</template>

<script>
export default {
    name: "MyFooter",
    data() {
        return {
          orders:[
                {
                    title: 'appetiziers',
                },
                {
                    title: 'burgers'
                },
                {
                    title: 'pizzas'
                },
                {
                    title: 'fries'
                },
                {
                    title: 'sides'
                },
                {
                    title: 'desserts'
                },
                {
                    title: 'beverages'
                },
                {
                    title: 'specials'
                },
          ],
          navs:[
                {
                    title: 'home'
                },
                {
                    title: 'Alternate Home'
                },
                {
                    title: 'Menu'
                },
                {
                    title: 'About'
                },
                {
                    title: 'News'
                },
                {
                    title: 'Contact Us'
                },
                {
                    title: 'Cart'
                },
          ],
          infos:[
            {
              title: 'My Account'
            },
            {
              title: 'Terms Of Service'
            },
            {
              title: 'Privacy Policy'
            },
          ],
          bedges:[
            {
              img: 'app-store-badge-200x67.png',
              txt: 'app store'
            },
            {
              img: 'play-store-badge-200x67.png',
              txt: 'play store'
            }
          ],
          openings:[
            {
              day: 'Mon',
              time: '10AM to 11PM'
            },
            {
              day: 'Tue',
              time: '10AM to 11PM'
            },
            {
              day: 'Wed',
              time: '10AM to 11PM'
            },
            {
              day: 'Thur',
              time: '10AM to 11PM'
            },
            {
              day: 'Fri',
              time: '10AM to 11PM'
            },
            {
              day: 'Sat',
              time: '10AM to 1AM'
            },
            {
              day: 'Sun',
              time: '11AM to 10PM'
            },
          ],
          socials:[
            {
              icon: "fa-brands fa-facebook-f"
            },
            {
              icon: "fa-brands fa-twitter"
            },
            {
              icon:"fa-brands fa-instagram"
            },
            {
              icon: "fa-brands fa-linkedin"
            },
            {
              icon: "fa-solid fa-rss"
            },
            {
              icon: "fa-brands fa-youtube"
            },
            {
              icon: "fa-regular fa-envelope"
            },
          ]
        }
    },
}
</script>

<style lang="scss">

  @import "@/style/footer.scss"

</style>