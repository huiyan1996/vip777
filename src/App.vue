<template>
  <div id="app">
    <Topbar />
    <div class="container px-0">
      <Transition name="fade" mode="out-in">
        <router-view/>
      </Transition>
    </div>
    <BottomNav />
  </div>
</template>

<script>
import Topbar from '@/views/Topbar.vue'
import BottomNav from '@/views/BottomNav.vue'

export default {
  name: 'App',
  components: {
    Topbar,
    BottomNav,
  },
}
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  background: #000;
}

.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.2s ease;
}

.fade-enter-from,
.fade-leave-to {
  opacity: 0;
}
</style>
