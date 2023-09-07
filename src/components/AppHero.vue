<script >
export default {
    data() {
        return{
            image: 'pexels-riccardo-bertolo-4245826.jpg',
        };
    },

    methods: {
        buidImagePath(imageName) {
            const imageUrl = new URL('../assets/img/' + imageName, import.meta.url);
            return imageUrl.href;
        },
    },
};
</script>

<template>
  <img :src="buidImagePath(image)" alt="">
</template>

<style scoped>

</style>
