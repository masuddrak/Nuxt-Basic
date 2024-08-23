<script setup>

const inputData = ref(
    {
        inputLabel: "name",
        inputType: "text",
        inputPlaseholder: "Enter Your Name Masud"
    }
)

</script>
<template>
    <div>
        <h2>Addded product list</h2>
        <div class="conatiner">
            <register></register>
            <login></login>
        </div>
        <h1>Vue.js props </h1>
        <!-- common -->

        <h1>Vue.js props </h1>
        <CommonInput :input-data="inputData"></CommonInput>
    </div>

</template>




<style>
.conatiner {
    display: flex;
    gap: 40px;
}
</style>