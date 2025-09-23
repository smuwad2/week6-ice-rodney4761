<script>
    export default { 
        data() {
            return {
                // Add code here
                id:"demo1",
                blueBox:true,
                blueBtn:true
            }
        },
        methods: { 
         // Add code here
            changeColour() {
                this.blueBox = !this.blueBox
                this.blueBtn = !this.blueBtn
            }
    }
    }
</script>

<template>
    
    <!-- Modify code here -->
    <div class="container">
        <div v-bind:id="id" :class="{'blueBox': blueBox, 'redBox': !blueBox}" class="m-2">
            div ID : {{id}} 
        </div>
        
        <button type="button" v-on:click="changeColour()" :class="{'btn btn-primary': blueBtn, 'btn btn-danger': !blueBtn}">Change Color</button>
    </div>

</template>

<style scoped>
    .redBox {
        background-color: red;
    }
    .blueBox {
        background-color: blue;
    }
    #demo1 {
        color: white;
    }
</style>