<script>
    export default {
        name: 'AppMain',
        props: {
            cards: Array
        }
}
</script>




<template>
    <main>
        <div class="card-container container">

        </div>
    </main>
</template>


<style lang="scss" scoped>
    main {
        padding: 0 12.5%;
        background-color: #1C1C1C;
        color: white;
        height: 500px;
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