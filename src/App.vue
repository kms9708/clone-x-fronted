<template>
  <div class="container">
    
    <router-view />
    <!--/login -> <loginPage />  -->
    <!--/signup -> <signupPage /> -->
  </div>
</template>

<script>

export default {
  name: 'App',
};
</script>

<style>
body{
    background-color:black;
    color:white;
}

.container{
    height:100vh;
    display:flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
</style>