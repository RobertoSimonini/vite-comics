<script>
import NewSeries from './buttons/NewSeries.vue';
export default {
    name: 'Jumbotron',
    components: {
        NewSeries
    }
}
</script>

<template>
    <section>
        <new-series></new-series>
    </section>
</template>

<style lang="scss" scoped>
    section {
        height: 400px;
        background-image: url(../assets/img/jumbotron.jpg);
        background-size: cover;
        background-repeat: no-repeat;

        position: relative;
        
        button {
            position: absolute;
            bottom: -5%;
            left: 10%;
        }
    }

</style>