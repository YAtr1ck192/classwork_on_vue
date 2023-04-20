<template>
    <header>
        <div class="header-logo">
            <img src="/images/logo.png" alt="header-logo">
        </div>
        <nav>
            <a
                v-for="(item, index) in items"
                :key="index"
                class="nav-item"
                href="#"
            >{{ item.linkContent }}</a>
        </nav>
    </header>
</template>

<script>
export default {
    name: "header-block",
    data () {
        return {
            items:[
                {linkContent:'HOME'},
                {linkContent:'BLOG'},
                {linkContent:'CATEGORIES'},
                {linkContent:'PICK CATEGORY'},
                {linkContent:'ABOUT US'},
                {linkContent:'CONTACT US'},
            ],
        }
    }
}
</script>

<style scoped>
header {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
}
.header-logo {
    margin: 60px 0 52px;
}
nav {
    display: flex;
    align-items: center;
    width: 560px;
    justify-content: space-between;
    margin-bottom: 58px;
}
.nav-item {
    text-decoration: none;
    color: white;
    font-size: 11px;
    font-family: "mr";
    padding-bottom: 14px;
    border-bottom: 2px solid transparent;
}
.nav-item:hover {
    border-bottom: 2px solid #dfdede73;
}

</style>