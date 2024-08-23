<template>
  <v-container class="pa-4" max-width="1200">
    <v-expansion-panels
      v-model="panel"
      class="modern-expansion-panels"
      flat
      multiple
    >
      <v-expansion-panel>
        <v-expansion-panel-title class="modern-title">
          <v-icon>mdi-video</v-icon>
          <span>Vídeo de Apresentação</span>
        </v-expansion-panel-title>
        <v-expansion-panel-text class="modern-text">
          <div class="video-container">
            <v-responsive max-width="950">
              <iframe
                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                allowfullscreen
                frameborder="0"
                height="500"
                src="https://www.youtube.com/embed/rtPNp-FSAJg"
                title="YouTube video player"
                width="100%"
              />
            </v-responsive>
          </div>
        </v-expansion-panel-text>
      </v-expansion-panel>

      <v-expansion-panel>
        <v-expansion-panel-title class="modern-title">
          <v-icon>mdi-account</v-icon>
          <span>Sobre Mim</span>
        </v-expansion-panel-title>
        <v-expansion-panel-text class="modern-text">
          <v-sheet
            class="modern-sheet mt-4 pa-4 d-flex align-center justify-center"
            elevation="6"
            rounded="lg"
          >
            <div class="d-flex align-center">
              <v-img
                class="rounded-circle"
                height="150"
                src="../assets/linkedin.png"
                width="150"
              />
              <div class="ml-4">
                <h2 class="text-h6">Sobre Mim</h2>
                <p class="text-body-1">
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque
                  ut risus at nisi condimentum scelerisque. Fusce nec arcu in purus
                  ullamcorper sodales.
                </p>
              </div>
            </div>
          </v-sheet>
        </v-expansion-panel-text>
      </v-expansion-panel>
    </v-expansion-panels>
  </v-container>
</template>

<script setup>
  import { ref } from 'vue'

  const panel = ref([1])
</script>
