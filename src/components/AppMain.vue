<script>
export default {
    name: 'Main'
}
</script>

<template>
    <main>
        <div class="container">
            <div class="card">
                <div>image</div>
                <h2>Title</h2>
                <p>Type</p>
            </div>
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

        .card {
            text-align: center;
            background-color: pink;
            flex-basis: calc(100% / 5);
        }
    }
}
</style>