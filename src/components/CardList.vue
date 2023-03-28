<script>
import Card from './Card.vue';
import axios from 'axios';

export default {
    name: 'CardList',
    components: {
        Card
    },
    data() {
        return {
            characters: []
        }
    },
    created() {
        axios
            .get('https://db.ygoprodeck.com/api/v7/cardinfo.php')
            .then(response => {
                this.characters = response.data.data.slice(0, 39)
                console.log(this.characters)
            })
    }
}
</script>

<template>
    <div class='container-cards' v-for="character in characters">
        <Card :character="character" />
    </div>
</template>

<style lang="scss" scoped>
.container-cards {
    text-align: center;
    flex-basis: calc(100% / 5);
    margin-bottom: 20px;
}
</style>