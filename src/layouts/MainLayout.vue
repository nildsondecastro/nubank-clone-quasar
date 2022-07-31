<template>
  <q-layout view="lHh Lpr lFf">
    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
export default {
  name: 'MainLayout',
  data() {
    return {};
  },
};
</script>

<style lang="scss">
.q-layout {
  background-color: #82269e;
}
</style>