<script>
export default {
    name: "AppBlueBar",
    data() {
        return {

        }
    },
    props: {
        thumb: String,
        series: String
    }
}
</script>


<template>
    <div class="card">

        <div class="card-img">
            <img :src="thumb" :alt="series">
        </div>


        <div class="card-text">
            <p>{{ series }}</p>
        </div>

    </div>
</template>


<style lang="scss" scoped>
.card-text {
    color: white;
}

.card {
    width: calc(100% / 6 - 1rem);

}
</style>