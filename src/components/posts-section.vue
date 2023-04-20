<template>
    <section class="posts">
        <postArticle
                v-for="(item, index) in items"
                :key="index"
                :post="item"
        />
    </section>
</template>

<script>
import postArticle from "@/components/post-article.vue";
export default {
    name: "posts-section",
    data () {
        return {
            items: [
                {
                    buttonContent: 'TRAVEL',
                    authorPhoto:'/images/author-1.png',
                    authorName: 'Luke Cage',
                    dateAdd: 'October 11, 2016',
                    postTitle: 'The 10 most beautiful places you should visit in your life',
                    postDesc: 'Vestibulum ut placerat nisl. Cras sed purus tellus. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Duis posuere nisi sit amet neque finibus vestibulum. Vivamus at leo ut turpis posuere molestie. Nullam',
                    backgroundArticle: 'background-article'
                },
                {
                    buttonContent: '',
                    authorPhoto:'/images/author-2.png',
                    authorName: 'Luke Cage',
                    dateAdd: 'October 11, 2016',
                    postTitle: 'The 10 most beautiful places you should visit in your life',
                    postDesc: 'Vestibulum ut placerat nisl. Cras sed purus tellus. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Duis posuere nisi sit amet neque finibus vestibulum. Vivamus at leo ut turpis posuere molestie. Nullam',
                    backgroundArticle: 'second-background-article'
                },
                {
                    buttonContent: 'PHOTOGRAPHY',
                    authorPhoto:'/images/author-1.png',
                    authorName: 'Luke Cage',
                    dateAdd: 'October 11, 2016',
                    postTitle: 'The 10 most beautiful places you should visit in your life',
                    postDesc: 'Vestibulum ut placerat nisl. Cras sed purus tellus. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Duis posuere nisi sit amet neque finibus vestibulum. Vivamus at leo ut turpis posuere molestie. Nullam',
                    backgroundArticle:'third-background-article'
                },
            ]
        }
    },
    components: {
        postArticle
    }
}
</script>

<style scoped>

</style>