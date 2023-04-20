<template>
    <div class="read-more container">
        <div class="read-more-title block-title">
            Want to read more?
        </div>
        <button class="fiol-button">VISIT BLOG ARCHIVE</button>
    </div>
</template>

<script>
export default {
    name: "read-more-block"
}
</script>

<style scoped>
.read-more {
    background: #F1F1F1;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
}
.read-more-title {
    font-size: 30px;
    margin: 49px 0 21px;;
}
.fiol-button {
    margin-bottom: 60px;
    background-color: #8D4FDB;
    padding: 15px 25px 15px;
    color: white;
    font-family: "mr";
    font-size: 10px;
    border: none;
    border-radius: 3px;
    cursor: pointer;
}

</style>