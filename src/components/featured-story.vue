<template>
    <article class="featured-stories-card">
        <div :class="posts.backgroundArticle">
            <div class="card-story-author">
                <img class="card-story-photo" :src="posts.authorPhoto" alt="author-photo">
                <div class="author-desc">
                    <div class="author-name">{{ posts.authorName }}</div>
                    <div class="date-add">{{ posts.dateAdd }}</div>
                </div>
            </div>
        </div>
        <div class="featured-stories-card-title">
            {{ posts.cardTitle }}
        </div>
    </article>
</template>

<script>
export default {
    name: "featured-story",
    props:['posts'],
}
</script>

<style scoped>

.background-story {
    background: url("../../public/images/featured-bg.png");
    display: flex;
    align-items: flex-end;
    justify-content: flex-start;
    width: 300px;
    height: 190px;
}
.background-story-2 {
    background: url("../../public/images/featured-bg-2.png");
    display: flex;
    align-items: flex-end;
    justify-content: flex-start;
    width: 300px;
    height: 190px;
}
.background-story-3 {
    background: url("../../public/images/featured-bg-3.png");
    display: flex;
    align-items: flex-end;
    justify-content: flex-start;
    width: 300px;
    height: 190px;
}
.card-story-author {
    display: flex;
    align-items: center;
    margin: 0 0 24px 24px;
}
.featured-stories-card-title {
    font-family: "mr";
    font-size: 18px;
    max-width: 272px;
    margin-top: 23px;
}

</style>