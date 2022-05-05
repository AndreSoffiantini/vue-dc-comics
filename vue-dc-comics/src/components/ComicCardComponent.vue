<template>
    <div class="col-2">
        <img :src="comic.thumb" :alt="comic.series">           
        <h4>{{comic.series}}</h4>
    </div>
</template>

<script>
export default {
    name: 'ComicCardComponent',
    props: {
        comic: Object
    }
}
</script>

<style lang="scss" scoped>
    .col-2 {
                width: calc(2*100%/12 - 2rem);
                margin: 1rem;

                img {
                    width: 100%;
                    aspect-ratio: 1 / 1;
                    object-fit: cover;
                    object-position: top;
                }

                h4 {
                    color: white;
                    text-transform: uppercase;
                    margin-top: 1rem;
                }

    }
</style>