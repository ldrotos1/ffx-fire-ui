<template>
  <q-layout view="hHh lpR fFf">

    <q-header elevated class="bg-primary text-white" height-hint="98">
      <q-toolbar>
        <q-toolbar-title>
          <q-avatar square>
            <img :src="getImage">
          </q-avatar>
          Fairfax County Fire and Rescue Operations
        </q-toolbar-title>
      </q-toolbar>

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

<script>
import fairfaxFireImg from "../assets/patches/ffx-fire.png"

export default {
  name: "HomePageLayout",
  computed: {
    getImage() {
      return fairfaxFireImg
    }
  }
}
</script>

<style lang="scss" scoped></style>
