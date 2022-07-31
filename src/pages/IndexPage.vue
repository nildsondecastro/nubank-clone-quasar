<template>
  <q-page class="column justify-center items-center">
    <div class="row items-center justify-around q-mt-xl container-logo">
      <q-img src="../assets/logo-white.png" width="55px" />
      <strong>Nildson</strong>
    </div>
    <q-icon name="keyboard_arrow_down" size="28px" class="q-icon-arrow" />

    <q-card class="my-card q-ma-lg" flat bordered>
      <q-card-section horizontal class="q-pa-lg">
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

        <q-card-actions vertical class="column justify-center">
          <div class="div-orange"></div>
          <div class="div-blue"></div>
          <div class="div-green"></div>
        </q-card-actions>
      </q-card-section>

      <div class="bottom-container row items-center justify-between q-pa-sm q-mb-md q-mx-sm">
        <q-icon name="fastfood" size="25px" />
        <span class="q-mx-sm">
          Compra mais recente em padaria Av1 no valor de R$ 84,00 hoje
        </span>
        <q-icon name="keyboard_arrow_down" size="20px" />
      </div>
    </q-card>

    <q-scroll-area horizontal class="q-ml-md q-my-md">
      <div class="row no-wrap">

        <q-card class="card-items column justify-between q-ml-sm">
          <q-card-section>
            <q-icon name="person_add" size="35px" />
          </q-card-section>
          <q-card-section class="q-pt-none">
            <strong>Indicar Amigos</strong>
          </q-card-section>
        </q-card>

        <q-card class="card-items column justify-between q-ml-sm">
          <q-card-section>
            <q-icon name="monetization_on" size="35px" />
          </q-card-section>
          <q-card-section class="q-pt-none">
            <strong>Depositar</strong>
          </q-card-section>
        </q-card>

        <q-card class="card-items column justify-between q-ml-sm">
          <q-card-section>
            <q-icon name="request_quote" size="35px" />
          </q-card-section>
          <q-card-section class="q-pt-none">
            <strong>Transferir</strong>
          </q-card-section>
        </q-card>

        <q-card class="card-items column justify-between q-ml-sm">
          <q-card-section>
            <q-icon name="receipt" size="35px" />
          </q-card-section>
          <q-card-section class="q-pt-none">
            <strong>Pagar Boleto</strong>
          </q-card-section>
        </q-card>
        
      </div>
    </q-scroll-area>

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

.div-orange {
  height: 30px;
  width: 7px;
  background-color: $orange;
  border-top-left-radius: 5px;
  border-top-right-radius: 5px;
}
.div-blue {
  height: 70px;
  width: 8px;
  background-color: $blue;
}
.div-green {
  height: 105px;
  width: 7px;
  background-color: $green;
  border-bottom-left-radius: 5px;
  border-bottom-right-radius: 5px;
}
.bottom-container {
  .q-icon {
    color: $gray;
  }
  span {
    color: $gray;
    width: 75%
  }
}
.card-items {
  height: 140px;
  width: 115px;
  background-color: $darkPurple;
  color: $white;
  cursor: pointer;
}
.q-scrollarea {
  width: 95%;
  height: 145px;
}
</style>