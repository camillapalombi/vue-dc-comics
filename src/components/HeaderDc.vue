<template>
  <header>
      <div class="container header-container">
        <div class="container-header-left">
            <img src="../../src/assets/img/dc-logo.png" alt="DC Logo">
        </div>
        <div class="container-header-right">
            <ul>
                <li v-for="(link, index) in headerLinks" :key="index"><a :href="link.href"> {{ link.text }}</a></li>
            </ul>
        </div>
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

<style scoped lang="scss">
@import '../assets/style/partials/variables';

.header-container {
    height: 8rem;
    justify-content: space-between;
    align-items: center;

    .container-header-left {
    width: 20%;
        img {
            width: 70px;
        }
    }
}
.container-header-right {
    width: 80%;

    ul {
        list-style: none;
        display: flex;
        justify-content: flex-end;
        line-height: 7.7em;
        li {
            margin-right: 25px;
            border-bottom: 4px solid transparent;
            &:hover {
                border-bottom: 4px solid $activeColor;
                a {
                    color: $activeColor;
                }
            }
        }
    }
}
a {
    text-decoration: none;
    color: $text_grey;
    font-weight: bold;
}

</style>