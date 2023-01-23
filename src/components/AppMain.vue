<script>
import CardComic from './Products/CardComic.vue'
export default {
        name: 'AppMain',
        components: {CardComic},
        props: {
            cards: Array
        }
}
</script>




<template>
    <main>
        <div class="card-container">
            <card-comic v-for="card in cards" :card="card"></card-comic>
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
            margin: 2rem;

            .comic-card {
                flex-basis: calc(100% / 6);         
            }
        }


    }
    
</style>