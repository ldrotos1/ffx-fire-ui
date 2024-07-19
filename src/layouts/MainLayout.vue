<template>
  <q-layout view="hHh lpR fFf">

    <q-header elevated class="bg-primary text-white" height-hint="98">
      <HeaderToolbar />

      <q-tabs align="left">
        <q-route-tab to="/stations" label="Stations" />
        <q-route-tab to="/apparatus" label="Apparatus" />
      </q-tabs>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>

  </q-layout>
</template>

<script setup>
import HeaderToolbar from "components/header/HeaderToolbar.vue";
</script>

<style lang="scss" scoped></style>
