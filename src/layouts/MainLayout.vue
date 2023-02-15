<template>
  <q-layout view="hhh Lpr lFf">
    <q-scroll-area style="height: 100vh">
      <q-header>
        <q-toolbar>
          <q-toolbar-title class="text-center"> Header </q-toolbar-title>
        </q-toolbar>
        <q-toolbar class="bg-white">
          <div class="row full-width bg-red q-ma-lg">
            <q-toolbar-title class="text-center text-black">
              toolbar
            </q-toolbar-title>
          </div>
        </q-toolbar>
      </q-header>

      <q-page-container>
        <q-scroll-area :visible="visible" style="width: 90%; min-height: 500px; height: 100px">
          <router-view />
        </q-scroll-area>
      </q-page-container>
    </q-scroll-area>
  </q-layout>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const visible = ref(true);
</script>
<style>
/* *,
*:before,
*:after {
  box-sizing: border-box;
}
main {
  flex: 1 1 auto !important;
  overflow: auto !important;
} */
</style>
