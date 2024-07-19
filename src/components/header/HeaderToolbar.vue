<template>
  <q-toolbar>
    <q-toolbar-title>
      <q-avatar square>
        <img v-bind:src="img" class="pointer" :onclick="gotoHomePage">
      </q-avatar>
      <span class="q-ml-sm pointer" :onclick="gotoHomePage">Fairfax County Fire and Rescue Operations</span>
    </q-toolbar-title>
  </q-toolbar>
</template>

<script setup>
import img from 'assets/patches/ffx-fire.png'
import { useRouter } from 'vue-router';

const router = useRouter()

function gotoHomePage() {
  router.push({ path: "/" })
}
</script>

<style lang="scss" scoped>
.pointer {
  cursor: pointer;
}
</style>
