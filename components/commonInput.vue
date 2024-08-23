<script setup>
const { inputData } = defineProps(['inputData'])
const { inputType, inputLabel, inputPlaseholder } = inputData
const inputValue = ref('masud')
const getInputValue = (e) => {
    inputValue.value = e
}

</script>
<template>
    <div>
        <p>{{ inputValue }}</p>
        <label>{{ inputLabel }}</label>
        <input :type="inputType" :value="inputValue" @input="getInputValue($event.target.value)" class="input-style"
            :placeholder="inputPlaseholder">
    </div>
</template>

<style scoped>
.input-style {
    border: 2px solid green;
    display: grid;
    grid-template-columns: repeat(3, 1fr);

}
</style>