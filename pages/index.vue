<template>
  <div>
    <VAppBar>
      <VAppBarTitle>
        <v-img
          :width="30"
          cover
          alt="Logo Blasco"
          src="../assets/logo_blasco.png"
        ></v-img>
      </VAppBarTitle>

      <v-tabs v-model="tab" bg-color="white" color="#5b1216">
        <v-tab value="one">Sobre</v-tab>
        <v-tab value="two">Equipe</v-tab>
        <v-tab value="three">Publicações</v-tab>
        <v-tab value="four">Contato</v-tab>
      </v-tabs>
    </VAppBar>
    <VContainer>
      <v-tabs-window v-model="tab">
        <v-tabs-window-item value="one">
          <p>
            Precisa de um advogado especializado em isenção de imposto de renda
            para pessoas com doença grave?
          </p>
        </v-tabs-window-item>
        <v-tabs-window-item value="two"> Two </v-tabs-window-item>
        <v-tabs-window-item value="three"> Three </v-tabs-window-item>
        <v-tabs-window-item value="four"> Four </v-tabs-window-item>
      </v-tabs-window>
    </VContainer>
  </div>
</template>

<script setup>
import { ref } from "vue";

const tab = ref(null);
</script>

<style></style>
