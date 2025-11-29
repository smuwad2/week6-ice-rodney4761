<script>
    export default { 
        data() {
            return {
                blue: true,
                id: "demo1"
            }
        },
        methods: { 
   			changeColor(){
                this.blue = !this.blue
            }
		}
    }
</script>

<template>
    
    <!-- Modify code here -->
    <div class="container">
        <div v-bind:id="id" class="m-2" :class="{'blueBox': blue, 'redBox': !blue}">
            div ID : {{id}} 
        </div>
        
        <button @click="changeColor()" :class="{'btn btn-primary': blue, 'btn btn-danger': !blue}" type="button">Change Color</button>
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