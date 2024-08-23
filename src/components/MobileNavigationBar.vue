<template>
  <v-card>
    <v-tabs
      v-model="tab"
      align-tabs="center"
      color="deep-purple-accent-4"
    >
      <v-tab :to="'/about'">Sobre</v-tab>
      <v-tab :to="'/projects'">Projetos</v-tab>
      <v-tab :to="'/contact'">Contato</v-tab>
    </v-tabs>

    <v-tabs-window v-model="tab">
      <v-tabs-window-item
        v-for="path in ['/about', '/projects', '/contact']"
        :key="path"
        :value="path"
      >
        <router-view :key="path" />
      </v-tabs-window-item>
    </v-tabs-window>
  </v-card>
</template>

<script>
  export default {
    data: () => ({
      tab: null,
    }),
  }
</script>
