<script>
    export default {
        data () {
            return {
                message: "Choose your favorite fruit: ",
                // fruit1: "apple",
                // fruit2: "orange",
                // fruit3: "peach"
                fruits: ["apple", "orange", "peach"]
            }
        }
    }
</script>

<template>
    <div id="app">
        <!-- {{ message }} </br>
        {{ fruit1 }} <input type="radio" name="fruit">
        {{ fruit2 }} <input type="radio" name="fruit">
        {{ fruit3 }} <input type="radio" name="fruit"> -->

        {{ message }}
        <label v-for="fruit in fruits" :key="fruit">
            {{ fruit }} <input type="radio" name="fruit" :value="fruit">
        </label>
    </div>
</template>

<style scoped>
</style>