<script>
import CardComic from './products/CardComic.vue'
import LoadMore from './buttons/LoadMore.vue'
export default {
        name: 'AppMain',
        components: {CardComic, LoadMore},
        props: {
            cards: Array
        }
}
</script>




<template>
    <main>
        <div class="card-container">
            <card-comic v-for="card in cards" :card="card"></card-comic>
            <load-more></load-more>
        </div>
    </main>
</template>


<style lang="scss" scoped>
    main {
        padding: 0 12.5%;
        background-color: #1C1C1C;
        color: white;
        height: 750px;
        display: flex;
        align-items: center;


        .card-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            margin: 2rem;

            .comic-card {
                flex-basis: calc(100% / 6);         
            }
        }

        

    }
    
</style>