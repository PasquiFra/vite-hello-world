<script>
export default {
    name: "AppJumbotron",
    data: () => ({
        image: "jumbo.jpg"
    }),
    methods: {
        imagePath(image) {
            const url = new URL(`../assets/${image}`, import.meta.url);
            return url.href;
        }
    }
}
</script>

<template>
    <img :src="imagePath(image)" alt="jumbo">
</template>

<style></style>