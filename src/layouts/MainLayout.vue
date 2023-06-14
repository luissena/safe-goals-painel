<template>
  <q-layout >

    <q-header class="row items-end justify-between q-pa-lg " >
      <q-img
        width="225px"
        src="/logo.svg"
        spinner-color="primary"
        spinner-size="82px"

      />

      <div class="col-6 ">
        <ul class="row text-h6 text-center">
          <li class="col-3">HOME</li>
          <li class="col-3">GOALS</li>
          <li class="col-3">NEW GOAL</li>
          <li class="col-3">CONFIGURAÇÕES</li>
        </ul>
      </div>

      <div class="grey-700 row items-center q-py-xs q-px-md" 
      style="border-radius: 10px; gap: 10px;" >
        <q-avatar size="50px"
        class="q-my-sm"
        font-size="50px"
        color="teal"
        text-color="white"
        icon="directions" />
        <span class="text-h5">Luis Sena</span>
        <q-icon name="keyboard_arrow_down"  size="25px"/>

      </div>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'MainLayout',

  setup() {
    return {

    };
  },
});
</script>

<style>
.q-layout__section--marginal{
  background: transparent;
}
</style>
