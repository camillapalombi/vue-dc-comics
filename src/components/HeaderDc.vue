<template>
  <header>
      <div class="container-header-left">
        <img src="../../src/assets/img/dc-logo.png" alt="DC Logo">
      </div>
      <div class="container-header-right">
          <ul>
              <li v-for="(link, index) in headerLinks" :key="index"><a :href="link.href"> {{ link.text }}</a></li>
          </ul>
      </div>
  </header>
</template>

<script>
export default {
name: 'HeaderDc',
data () {
    return {
        headerLinks: [
            {
            text: 'CHARACTERS',
            href: '#!'
            },
            {
            text: 'COMICS',
            href: '#!'
            },
            {
            text: 'MOVIES',
            href: '#!'
            },
            {
            text: 'TV',
            href: '#!'
            },
            {
            text: 'GAMES',
            href: '#!'
            },
            {
            text: 'COLLECTIBLES',
            href: '#!'
            },
            {
            text: 'VIDEOS',
            href: '#!'
            },
            {
            text: 'FANS',
            href: '#!'
            },
            {
            text: 'NEWS',
            href: '#!'
            },
            {
            text: 'SHOP',
            href: '#!'
            }
        ]
    }
}
}
</script>

<style>

</style>