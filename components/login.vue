<template>
    <form class="form-control">
        <input type="text" class="input-style" placeholder="Enter Your Email">
        <br>
        <input type="password" class="input-style" placeholder="Enter Your Password">
        <br>
        <button class="form-btn">Login</button>
    </form>
</template>
<style scoped>

.input-style{
    border: 2px solid green;
    display: grid;
    grid-template-columns: repeat(3,1fr);
 
}
.form-btn{
    background-color: green;
    color: white;
    border: none;
    padding: 5px 10px;
    
}
</style>