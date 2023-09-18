<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <h1>Asho Random Number er square Shikhi :3 </h1>
    <div class="counter">
      {{ $store.state.counter }}
    </div>
    <div class="counter-squared">
      {{ $store.state.counter }}
      <sup>2</sup> =
      {{ $store.getters.counterSquared }}
    </div>
    <div class="buttons">
      <button @click="$store.dispatch ('decreaseCounter')">-</button>
      <button @click="$store.dispatch ('increaseCounter')">+</button>
    </div>
  </div>
</template>

<script>

export default {
  name: 'HomeView'
}

</script>

<style>
div {
  margin-bottom: 10px;
}
.counter {
  font-size: 80px;
}
.buttons button {
  font-size: 40px;
  width: 100px;
  margin: 0 10px;
}
</style>
