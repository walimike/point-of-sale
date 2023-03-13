<template>
    <v-container>
        <v-row>
        <v-col v-for="article in articles" :key="article.id" cols="12" sm="6" md="4">
            <article-card :article="article"></article-card>
        </v-col>
        </v-row>
    </v-container>
</template>

<script>
    import ArticleCard from '@/components/ArticleCard.vue'

    export default {
    components: {
        ArticleCard
    },
    data () {
        return {
        articles: []
        }
    },
    created () {
        this.fetchArticles()
    },
    methods: {
        async fetchArticles () {
        const response = await fetch('/api/articles')
        const articles = await response.json()
        this.articles = articles
        }
    }
    }
</script>
  