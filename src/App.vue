<template>
  <div id="app">
    <transition name="fade" mode="out-in">
      <router-view></router-view>
    </transition>
  </div>
</template>

<style>
.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.5s ease-out;
}

.fade-enter,
.fade-leave-to {
  opacity: 0;
}

header h1{
    padding: 10px 20px;
}
.app {
  margin: 0 auto;
  max-width: 1200px;
}

.cart {
  padding: 20px 50px;
}
.boxes {
  margin-top: 20px;
}

.verify {
  margin-top: 20px;
}

.submit {
  margin-top:20px;
  float: right;
}

.pagecheckout {
  padding: 20px 50px;
}
.description {
  font-size: 150%;
  margin-top:50px;
}

.inventory-message {
  margin-left: 20px;
  font-weight: bold;
  font-size: 120%;
  display:inline-block;
}


.product {
  margin-top: 30px;
  margin-left: 20px;
  max-height:300px;
  max-width:100%;
}

.rating-active:before {
   content: "\2605";
   position: absolute;
}
.rating {
  display: inline;
  margin-left: 10px;
  margin-top: 10px;
  float:right;
}
.rating > span {
  display: inline-block;
  position: relative;
  width: 1.1em;
}

@media (min-width: 1200px) {
    .container{
        max-width: 970px;
    }
}

</style>
