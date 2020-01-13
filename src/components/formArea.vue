<template>
    <div>
        <p>Input anything you want in below input: {{inputTxt}}</p>
        <input v-model='inputTxt' placeholder="input anything you want..." />
    </div>
</template>

<script>
export default {
    data() {
        return {
            inputTxt: ''
        }
    }
}
</script>

<style>

</style>