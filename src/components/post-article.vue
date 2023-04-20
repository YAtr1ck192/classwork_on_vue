<template>
    <article class="container">
        <div :class="post.backgroundArticle">
            <div class="article-button" :class="{'transparent' : !post.buttonContent}">
                <button>{{ post.buttonContent }}</button>
            </div>
            <div class="article-info">
                <div class="article-author">
                    <img class="author-photo" :src="post.authorPhoto" alt="author-photo">
                    <div class="author-desc">
                        <div class="author-name">{{ post.authorName }}</div>
                        <div class="date-add">{{ post.dateAdd }}</div>
                    </div>
                </div>
                <h1 class="article-title">{{ post.postTitle }}</h1>
            </div>
            <div class="article-desc-and-a">
                <div class="article-desc">{{ post.postDesc }} </div>
                <a class="article-a" href="#">{{ linkContent }}</a>
            </div>
        </div>
    </article>
</template>

<script>
export default {
    name: "post-article",
    data () {
        return {
            linkContent: 'Continue Reading →'
        }
    },
    props: ['post'],
}
</script>

<style scoped>
.background-article {
    background: url(../../public/images/article-img-1.png) no-repeat;
}
.second-background-article {
    background: url(../../public/images/article-img-2.png) no-repeat;
}
.third-background-article {
    background: url(../../public/images/article-img-3.png) no-repeat;
}
.article-button {
    display: flex;
    justify-content: flex-end;
}
.article-button button {
    background: rgba(0, 0, 0, 0.2);
    border: none;
    color:white;
    padding: 5px 10px 5px;
    font-size: 8px;
    font-family: "mr";
    border-radius: 30px;
    margin: 21px 20px 115px 0;
    cursor: pointer;
}
.transparent button {
    background:transparent;
    color: transparent;
    cursor: default;
    pointer-events: none;
}
.article-info {
    margin-left: 60px;
}
.article-author {
    display: flex;
    align-items: center;
    margin-bottom: 20px;
}

.article-title {
    max-width: 470px;
    color: white;
    font-size: 18px;
    font-family: "mr";
    margin-bottom: 40px;
}
.article-desc {
    max-width: 660px;
    font-size: 18px;
    line-height: 25px;
    font-family: "lr";
    margin-bottom: 9px;
}

.article-a {
    color: #8D4FDB;
    text-decoration: none;
    font-family: "lr";
    font-size: 17px;
    width: 660px;
}
.article-desc-and-a {
    background: #fff;
    padding: 36px 0 44px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

</style>