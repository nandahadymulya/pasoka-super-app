<template>
  <v-app>
    <TheSidebar />

    <v-main>
      <v-system-bar height="30"> News! News! News! </v-system-bar>
      <v-app-bar color="deep-purple accent-4">
        <!-- <v-toolbar-title>{{ items.title }}</v-toolbar-title> -->
      </v-app-bar>

      <v-container>
        <Nuxt />
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
import TheSidebar from '@/components/Sidebar.vue'
export default {
  name: 'DefaultLayout',
  components: {
    TheSidebar,
  },
}
</script>
