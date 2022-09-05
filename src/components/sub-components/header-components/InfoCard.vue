<template>

    <div class="info-card">
        <ul>
            <li v-for="(info, index) in infocard" :key="index">
                <span class="info-icon" v-html="info.icon"></span>
                <span class="info-text">{{info.text}}</span>
            </li>
        </ul>
    </div>
  
</template>

<script>
export default {
    name: "InfoCard",
    data(){
        return{
            infocard: [
                {
                    icon: '<i class="fa-regular fa-clock"></i>',
                    text: "24/7 delivery"
                },
                {
                    icon: '<i class="fa-solid fa-burger"></i>',
                    text: "over 100 dishes"
                },
                {
                    icon: '<i class="fa-solid fa-mobile"></i>',
                    text: "in app orders"
                },
                {
                    icon: '<i class="fa-solid fa-car"></i>',
                    text: "fast delivery"
                },
            ]
        }
    }

}
</script>

<style>

</style>