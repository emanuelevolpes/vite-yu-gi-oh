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
        <!-- <div class="container d-flex">
            <Card />
        </div> -->
        <div class="dropdown">
  <button class="btn btn-secondary dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false">
    Dropdown button
  </button>
  <ul class="dropdown-menu">
    <li><a class="dropdown-item" href="#">Action</a></li>
    <li><a class="dropdown-item" href="#">Another action</a></li>
    <li><a class="dropdown-item" href="#">Something else here</a></li>
  </ul>
</div>
    </main>
</template>

<style lang="scss" scoped>
main {
    background-color: #d48f38;
    .container {
        background-color: white;
    }
}
</style>