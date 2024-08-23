<template>
  <v-container class="fill-height d-flex flex-column justify-center align-center">
    <v-responsive class="align-center mx-auto" max-width="900">
      <v-row class="mb-8" justify="center">
        <v-col cols="12" md="6">
          <ProjectCard />
        </v-col>
        <v-col cols="12" md="6">
          <ProjectCard />
        </v-col>
        <v-col cols="12" md="6">
          <ProjectCard />
        </v-col>
        <v-col cols="12" md="6">
          <ProjectCard />
        </v-col>
      </v-row>
    </v-responsive>
  </v-container>
</template>

<script setup lang="ts">
  import ProjectCard from '@/components/ProjectCard.vue'
</script>
