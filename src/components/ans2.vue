<script>
    export default { 
        data() {
            return {
                width: '200',
                height: '200',
                myImg: '/assets/me.png'
            }
        },
    }
</script>

<template>
    <!-- : is a short-hand notation for v-bind -->
    <!-- <img v-bind:src="myImg" v-bind:width="width" v-bind:height="height"/> -->
    <img :src="myImg" :width="width" :height="height"/>
   
</template>
