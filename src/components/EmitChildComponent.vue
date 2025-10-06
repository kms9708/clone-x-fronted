<template>
    <button @click="clickButton">"자식이 만든 버튼 입니다."</button>
  
</template>

<script>
export default {
    name: "EmitChildComponent",
    emits:["click-child-button"],
    methods:{
        clickButton(){
            this.$emit("click-child-button","what's up");
        },
    },

};
</script>

<style>

</style>