<template>
  <v-app>
    <v-navigation-drawer
      app
      expand-on-hover
      mobile-breakpoint="md"
      persistent
      width="256"
    >
      <v-list>
        <v-list-item
          prepend-avatar="../assets/perfil.png"
          subtitle="ric.brasiliano@gmail.com"
          title="Ricardo Barbosa"
        />
      </v-list>

      <v-divider />

      <v-list density="compact" nav>
        <v-list-item prepend-icon="mdi-account" title="Sobre mim" to="/about" value="sobre-mim" />
        <v-list-item prepend-icon="mdi-briefcase" title="Projetos" to="/projects" value="projetos" />
        <v-list-item prepend-icon="mdi-email" title="Contato" to="/contact" value="contato" />
      </v-list>
    </v-navigation-drawer>

    <v-main>
      <v-container>
        <slot />
      </v-container>
    </v-main>
  </v-app>
</template>

<script setup>

</script>
