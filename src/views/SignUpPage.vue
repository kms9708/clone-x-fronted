<template>
    <div>
        <div class="logo-container">
            <img src="@/assets/x-logo.png" class="logo" />
        </div>
    <div class = "title">계정을 생성하세요</div>
    <InputField :type="'text'" :placeholder="'Email'" :modelValue="email" v-model="email"/>
    <InputField :type="'text'" :placeholder="'Name'" :modelValue="name" v-model="name"/>
    <InputField :type="'password'" :placeholder="'Password'" :modelValue="password" v-model="password"/>
    <InputField :type="'password'" :placeholder="'Confirm Password'" :modelValue="confirmPassword" v-model="confirmPassword"/>


    <button class="button" @click="signup"> 회원가입</button>
    </div>

</template>

<script>
import InputField from "@/components/inputField.vue";
export default {
    name: "SignUpPage",
    components: {InputField  },
    data(){
        return{
            email:"",
            name:"",
            password:"",
            confirmPassword:""
        };
    },
}
</script>

<style scoped>
.title{
    margin-top:10px;
    margin-bottom:10px; 
    font-size: large;
    padding:1%;
}

</style>