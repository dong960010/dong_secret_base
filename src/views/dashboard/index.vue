<template>
  <div class="dashboard-container">
    <div class="dashboard-text">name: {{ name }}</div>
    <section class="icon-list">
      <i class="nes-mario" />
      <i class="nes-ash" />
      <i class="nes-pokeball" />
      <i class="nes-bulbasaur" />
      <i class="nes-charmander" />
      <i class="nes-squirtle" />
      <i class="nes-kirby" />
    </section>
  </div>
</template>

<script>
import { mapGetters } from 'vuex'

export default {
  name: 'Dashboard',
  computed: {
    ...mapGetters([
      'name'
    ])
  }
}
</script>

<style lang="scss" scoped>
.dashboard {
  &-container {
    margin: 30px;
  }
  &-text {
    font-size: 30px;
    line-height: 46px;
  }
}
</style>
