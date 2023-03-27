<script>
import Card from './Card.vue';

export default {
    name: 'Main',
    components: {
        Card
    }
}
</script>

<template>
    <main>
        <div class="container">
            <Card />
        </div>
    </main>
</template>

<style lang="scss" scoped>
main {
    background-color: #d48f38;
    .container {
        background-color: white;
        display: flex;
        flex-wrap: wrap;
    }
}
</style>