<template>
    <div class="background">
    </div>
</template>

<script>
export default {
    name: "background-block"
}
</script>

<style scoped>
    .background {
        width: 100%;
        height: 2080px;
        background:  linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('../../public/images/background.png') no-repeat;
        background-size: cover;
        z-index: -100;
        position: absolute;
    }
</style>