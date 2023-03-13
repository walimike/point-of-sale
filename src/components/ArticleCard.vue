<template>
    <v-card>
        <v-card-title>{{ article.title }}</v-card-title>
        <v-card-text>{{ article.content }}</v-card-text>
    </v-card>
</template>

<script>
    export default {
        props: {
            article: Object
        }
    }
</script>
  