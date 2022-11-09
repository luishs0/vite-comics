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
            <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX"
                alt="series">
        </div>


        <div class="card-text">
            <p>hola</p>
        </div>

    </div>
</template>


<style lang="scss" scoped>
.card-text {
    color: white;
}

.card {
    width: calc(100% / 6 - 10px);

}
</style>