<template>
  <v-card
    class="py-4 px-6"
    href="https://vuetifyjs.com/"
    rounded="lg"
    target="_blank"
    variant="outlined"
  >
    <v-img
      cover
      height="150px"
      src="../assets/clock.jpg"
    />
    <v-card-title>Rooster Web</v-card-title>
    <v-card-text>Software de gerenciamento de tempo: rastreie, organize e gere planilhas
      para monitorar o tempo gasto em seus projetos.</v-card-text>
    <v-overlay
      contained
      model-value
      opacity=".1"
      persistent
      scrim="primary"
    />
  </v-card>
</template>
