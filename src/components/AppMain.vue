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
    }
}
</style>