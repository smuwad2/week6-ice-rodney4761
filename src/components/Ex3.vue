<script>
    export default { 
        data () {
            return {
                loginType: "Username login"
            }
        }
    }
</script>

<template>
    <h1>Please select your login option</h1>
    <!-- Add/modify code in the following to have a dropdown list 
        which lets the user to select either to login with username or email -->
    <select v-model="loginType">
        <option selected>Username login</option>
        <option>Email login</option>
    </select>
    
    <div v-if = "loginType == 'Username login'">
        <label>Username:&nbsp;</label>
        <input placeholder="Enter your username">
    </div>

    <div v-else>
        <label>Email:&nbsp;</label>
        <input placeholder="Enter your email">
    </div>
</template>