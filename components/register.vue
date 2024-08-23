<script setup>
const handelsubmit=()=>{

    console.log(fristname.value)
}
const fristname=ref("")


</script>



<template>
    <form class="form-control " @submit.prevent="handelsubmit">
        <div class="name-control">
            <input type="text" v-model="fristname" name="fristname" class="input-style" placeholder="Enter Your Frist Name">
            <input type="text" class="input-style" placeholder="Enter Your Last Name">
        </div>
        <br>
        <input type="text" class="input-style" placeholder="Enter Your Email">
        <br>
        <input type="password" class="input-style" placeholder="Enter Your Password">
        <br>
        <button type="submit" class="form-btn">Register</button>
    </form>
</template>
<style scoped>
.name-control{
    display: flex;
    gap: 20px;
}
.input-style{
    border: 2px solid yellow;
    display: grid;
    grid-template-columns: repeat(3,1fr);
    border-radius: 5px;
 
}
.form-btn{
    background-color: green;
    color: white;
    border: none;
    padding: 5px 10px;
    
}
</style>