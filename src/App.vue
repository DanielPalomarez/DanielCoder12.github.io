<template>
  <header>
  </header>
  <main>
    <router-view />
  </main>
  
</template>

<script>
import { computed } from 'vue'
import { AppState } from './AppState'
// import Navbar from './components/Navbar.vue'

export default {
  setup() {
    return {
      appState: computed(() => AppState)
    }
  },
  // components: { Navbar }
}
</script>
<style lang="scss">
@import "./assets/scss/main.scss";


:root {
  --main-height: calc(100vh - 32px - 64px);
}

.bebas {
  font-family: 'Bebas Neue', sans-serif;
}

</style>
