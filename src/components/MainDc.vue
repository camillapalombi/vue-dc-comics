<template>
  <main>
      <div class="container main-container">
          <p>--> Content Goes Here --> </p>
      </div>
    </main>
</template>

<script>
export default {
name: 'MainDc'
}
</script>

<style scoped lang="scss">
main {
    background-color: #1c1c1c;
    .main-container {
        height: 8rem;
        align-items: center;
        p {
            font-size: 23px;
            color: white;
            font-weight: bold;
        }
    }
}
</style>