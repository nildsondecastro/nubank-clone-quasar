<template>
  <q-page class="column justify-center items-center">
    <div class="row items-center justify-around q-mt-xl container-logo">
      <q-img src="../assets/logo-white.png" width="55px" />
      <strong>Nildson</strong>
    </div>
    <q-icon name="keyboard_arrow_down" size="28px" class="q-icon-arrow" />

    <q-card class="my-card q-ma-lg" flat bordered>
      <q-icard-section class="q-pa-lg">
        <div class="container-card">
          <q-icon name="payment" size="35px" class="q-icon-card" />
          <div class="info-container q-mt-xl">

            <strong class="text-uppercase">Fatura Atual</strong>
            <h4 class="q-ma-none">R$ 1.258,40</h4>

            <div>
              <span>Limite disponível</span>
              <strong class="q-ml-sm text-uppercase">R$ 4.830,00</strong>
            </div>

          </div>
        </div>
      </q-icard-section>
    </q-card>

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
    color: $white;
    font-size: 22px;
  }
}
.q-icon-arrow {
  color: $white;
}
.my-card {
  width: 100%;
  max-width: 330px;
  height: 340px;
}
.container-card {
  width: 95%;
}
.q-icon-card {
  color: $gray;
}
.info-container {
  height: 100px;
  h4 {
    color: $blue;
    font-weight: bold;
  }
  strong:first-child {
    color: $blue;
  }
  span {
    color: $gray;
  }
  strong {
    color: $green;
  }
}
</style>