<template>
    <div>
        <input type="text" :placeholder="'Email'" v-model="email"/>
        <input type="password" :placeholder="'Password'" v-model="password"/>

        <button @click="login">Login</button>
    <div>
      계정이 없으시나요?
      <span>가입하기</span>  
    </div>

    </div> 
</template>

<script>
export default {
    name : "LoginPage",
    data(){
        return{
            email : "",
            password : "",
        };
    },
    methods : {
        login(){
            console.log(this.email, this.password);
        }
    }
};
</script>

<style>

</style>