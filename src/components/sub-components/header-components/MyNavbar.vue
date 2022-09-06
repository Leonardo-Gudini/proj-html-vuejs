<template>
  <nav>
        <img src="@/assets/images/takeout-logo-2x.png" alt="logo">

        <ul>
            <li v-for="(list, index) in menu" :key="index" v-html="list.txt"></li>
        </ul>
    </nav>
</template>

<script>
export default {
    name: "MyNavbar",
    data() {
        return {
            menu: [
                    {
                        "txt": "Home"
                    },
                    {
                        "txt": "Order Online"
                    },
                    {
                        "txt": "About"
                    },
                    {
                        "txt": "News"
                    },
                    {
                        "txt": "Contact Us"
                    },
                    {
                        "txt": '<i class="fa-solid fa-cart-shopping"></i>'
                    },
                ]
        }
    },
}
</script>

<style lang="scss">

</style>