<script>
export default {
    name: 'Card',
    props: {
        character: Object
    }
}
</script>

<template>
    <article class="card">
        <img :src="character.card_images[0].image_url">
        <h4>{{ character.name }}</h4>
        <p>{{ character.type }}</p>
    </article>
</template>

<style lang="scss" scoped>
.card {
    background-color: #d48f38;
    height: 100%;
    margin: 10px;
    
    h4{
        font-size: 18px;
        color: white;
        text-transform: uppercase;
    }

    img {
        width: 100%;
        margin-bottom: 15px;
    }
}
</style>