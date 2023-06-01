<script>

export default {
    name: 'Appfumetti',
    props: {
        details: Object
    }
}

</script>

<template>
    <!-- fumetto -->
    <div class="card-fumetto">
        <img :src="details.thumb" :alt="details.series">
        <h5>{{ details.series }}</h5>
    </div>
</template>

<style lang="scss" scoped>
.card-fumetto {
    width: 15%;
    margin-bottom: 2rem;
}
</style>