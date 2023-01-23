<script>
export default {
    name: 'CardComic',
    props: {
        card: Object
    }
}
</script>

<template>
    <div class="comic-card">
            <img :src="card.thumb" :alt="card.series">
            <h4>{{ card.series }} </h4>
    </div>
</template>


<style lang="scss" scoped>
.comic-card {
    margin: 1.5rem 0;
    transition: transform 0.25s;

    &:hover {
        transform: scale(1.05);
    }

        img {
            display: block;
            height: 200px;
            width: 200px;
            cursor: pointer;         
        }


        h4 {
            text-transform: uppercase;
            font-size: 15px;
            }
}

</style>