<template>
  <div id="app">
    <transition name="fade" mode="out-in">
      <router-view></router-view>
    </transition>
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style>
#app {
 max-width: 1200px;
 margin: 0 auto;
 padding: 0 20px;
}
.fade-enter-active, .fade-leave-active {
  transition: opacity .5s ease-out;

}

.fade-enter, .fade-leave-to {
  opacity: 0;

}
</style>
