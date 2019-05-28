<template>
  <div id="app">
    <header>
      <figure>
        <img alt="background header" src="./assets/bg.png" />
      </figure>
    </header>
    <main>
      <Home />
    </main>
  </div>
</template>

<script>
import Home from './components/Home.vue'

export default {
  name: 'app',
  components: {
    Home
  }
}
</script>

<style lang="scss">
@import '~@/assets/style/main.scss';

header {
  figure {
    width: 100%;
    margin: auto;
    text-align: center;

    img {
      max-width: 1280px;
      width: 100%;
    }
  }
}

#app {
  padding-bottom: 150px
}

a:not(.nostyle) {
  text-decoration: none;
  color: $palette-blue;
  padding-bottom: 1px;
  border-bottom: 0;

  line-height: 1.4em;

  &:hover {
    cursor: pointer;
    color: $palette-blue;
    border-bottom: 1px solid $palette-blue;
  }
}
</style>
