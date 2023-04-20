<template>
    <footer>
        <div>Copyright © Explorer - Images used for demonstration purpose only (<a class="footer-a" href="#">Licenses</a>)</div>
        <div>Copyright © <a class="footer-a" href="#">Studio Corvus</a> Powered by <a class="footer-a" href="#">Webflow</a></div>
    </footer>
</template>

<script>
export default {
    name: "footer-block"
}
</script>

<style scoped>
footer {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    padding: 55px 0 45px;
    background: #000;
}
footer div{
    color: #8B8B8B;
    font-size: 14px;
    font-family: "lr";
}
footer div a {
    color: #8D4FDB;
    text-decoration: none;
    font-family: "lr";
    font-size: 13px;
}
footer div:last-child {
    margin-top: 10px;
}
</style>