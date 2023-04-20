<template>
    <section class="featured-stories bigger-container">
        <h2 class="block-title featured-stories-title">Featured Stories</h2>
        <div class="featured-stories-desc">
            Did you read read our personal favorites?
        </div>
        <div class="featured-stories-cards">
            <featuredStory
                v-for="(item, index) in posts"
                :key="index"
                :posts="item"
            />
        </div>
        <div class="featured-offer">
            <span class="featured-offer-txt">Want to read all of our stories?</span>
            <a class="article-a" href="#">Read the full blog</a>
        </div>
    </section>
</template>

<script>
import featuredStory from "@/components/featured-story.vue";
export default {
    name: "featured-stories",
    data () {
      return {
          posts: [
              {
                  authorPhoto: '/images/fs-author-1.png',
                  authorName: 'Luke Cage',
                  dateAdd: 'October 11, 2016',
                  cardTitle: 'The 10 most beautiful places you should visit in your life',
                  backgroundArticle:'background-story'
              },
              {
                  authorPhoto: '/images/fs-author-2.png',
                  authorName: 'Jessica Simpson',
                  dateAdd: 'Jun 12, 2016',
                  cardTitle: 'We found the most beautiful place for our party november',
                  backgroundArticle:'background-story-2'

              },
              {
                  authorPhoto: '/images/fs-author-1.png',
                  authorName: 'Luke Cage',
                  dateAdd: 'October 11, 2016',
                  cardTitle: 'Why New York is still our favorite city to visit',
                  backgroundArticle:'background-story-3'

              },
          ],
      }
    },
    components: {
        featuredStory
    }
}
</script>

<style scoped>
.featured-stories {
    padding: 85px 0 90px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-direction: column;
}
.featured-stories-title{
    font-size: 40px;
    margin-bottom: 25px;
}
.featured-stories-desc {
    font-family: "lr";
    font-size: 23px;
    color: #A9AFB3;
    margin-bottom: 50px;
}
.featured-stories-cards{
    display: flex;
    align-items: flex-start;
    justify-content: space-between;
    width: 940px;
    margin-bottom: 56px;
}
.featured-offer-txt{
    font-size: 17px;
    font-family: "lr";
    color: #333333;
    margin-right: 5px;
}
</style>