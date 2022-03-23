<template>
  <div class="single-box-series">
    <img class="series-img" :src="srcImage" :alt="serieTitle">
    <p class="series-title">{{ serieTitle.toUpperCase() }}</p>
</div>
</template>

<script>
export default {
name: 'BoxSeries',
props: {
    srcImage: String,
    serieTitle: String
}
}
</script>

<style scoped lang="scss">
.single-box-series {
    flex-basis: calc(16.66% - 15px);
    margin-left: 15px;
    margin-bottom: 55px;
    height: 190px;
    img {
        width: 100%;
        height: 100%;
    }
}
.series-title {
    color: white;
    margin-top: 10px;
}
</style>