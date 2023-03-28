<script>
export default {
    name: 'Card'
}
</script>

<template>
    <div class="card">
        <div>image</div>
        <h2>Title</h2>
        <p>Type</p>
    </div>
</template>

<style lang="scss" scoped>
.card {
    text-align: center;
    background-color: pink;
    flex-basis: calc(100% / 5);
}
</style>