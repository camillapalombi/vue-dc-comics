<template>
  <div class="single-box-series">
    <img class="series-img" :src="srcImage" :alt="serieTitle">
    <p class="series-title">{{ serieTitle }}</p>
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

<style>

</style>