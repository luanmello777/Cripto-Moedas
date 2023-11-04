<template>
  <v-container class="bg-yellow-accent-4">


    <h1 class="font ml-10 mr-10 text-white">Participantes do projeto :</h1>
    <h3 class="font ml-10 mr-10 mt-3" :class="smAndDown ? 'mb-5 mt-5' : ''">
      <v-chip>Fernanda Lira Mateus</v-chip>
      <br>
      <v-chip class="mt-3">Ellen Izabela Ribeiro de Aguiar</v-chip>
      <br>
      <v-chip class="mt-3">Maria Laura Soares Amorim</v-chip>
      <br>
      <v-chip class="mt-3">Luan Cardoso de Mello</v-chip> <v-chip class="mt-3 bg-white">(Programmer)</v-chip>
      <br>
      <v-chip class="mt-3">Carina Rossana Barbosa de Araújo</v-chip>
      <br>
      <v-chip class="mt-3">Carlos Henrique da Silva Batista</v-chip>
      <br>
      <v-chip class="mt-3">Rafael Fracaro de Sena</v-chip>
      <br>
      <v-chip class="mt-3">Victor Andrei da Silva</v-chip>
    </h3>
  </v-container>

  <v-footer class="bg-black align-center justify-center mt-10">
    <v-chip color="white" href="https://github.com/luanmello777" target="_blank>"><svg-icon type="mdi" :path="path"
        class="mr-2"></svg-icon>github.com/Luanmello777
    </v-chip>
  </v-footer>
</template>

<style scoped>
.font {
  font-family: 'Jost', sans-serif;
}
</style>

<script setup>
import SvgIcon from '@jamescoyle/vue-icon';
import { mdiGithub } from '@mdi/js';

const path = mdiGithub;


</script>
