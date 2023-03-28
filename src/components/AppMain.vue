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
    <main class="d-flex flex-column">
        <div class="container-sm dropdown mb-5">
            <button class="btn dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false">
                Select type
            </button>
            <ul class="dropdown-menu">
                <li><a class="dropdown-item" href="#">Action</a></li>
                <li><a class="dropdown-item" href="#">Another action</a></li>
                <li><a class="dropdown-item" href="#">Something else here</a></li>
            </ul>
        </div>
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

    button {
        background-color: white;
    }

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