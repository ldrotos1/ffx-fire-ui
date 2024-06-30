<template>
  <div class="fullscreen bg-red-10 text-white text-center q-pa-md flex flex-center">
    <div>
      <div style="font-size: 30vh">
        404
      </div>

      <div class="text-h2" style="opacity:.8">
        Page does not exist
      </div>

      <q-btn class="q-mt-xl" color="white" text-color="red" unelevated to="/" label="Go Home" no-caps />
    </div>
  </div>
</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'ErrorNotFound'
});
</script>
