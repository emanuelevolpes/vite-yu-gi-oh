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
        .then(response => (this.characters = response.data))
    }
}
</script>

<template>
    <Card />
</template>