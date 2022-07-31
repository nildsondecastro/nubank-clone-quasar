<template>
  <q-page class="column justify-center items-center">
    <div class="row items-center justify-around q-mt-xl container-logo">
      <q-img src="../assets/logo-white.png" width="55px" />
      <strong>Nildson</strong>
    </div>
  </q-page>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'IndexPage'
})
</script>

<style lang="scss">
.container-logo {
  width: 40%;
  strong {
    color: #ffe8ff;
    font-size: 22px;
  }
}
</style>