<script>
import CardList from './CardList.vue';
export default {
    name: 'Main',
    components: {
        CardList
    }
}
</script>

<template>
    <main>
        <div class="container d-flex">
            <span>Found 39 cards</span>
            <CardList />
        </div>
    </main>
</template>

<style lang="scss" scoped>
main {
    background-color: #d48f38;
    padding: 50px;
    .container {
        background-color: white;
        padding: 30px;
        flex-wrap: wrap;

        span {
            width: 100%;
            background-color: black;
            color: white;
            padding: 20px;
            margin: -10px -10px;
        }
    }
}
</style>