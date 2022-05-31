<template>
  <v-row align="center" class="border">
    <v-col class="p-2">
      <h2>Tambah Dokumen Baru</h2>
      <v-card elevation="2" height="500">
        <v-btn>
          <NuxtLink to="/general"> Back </NuxtLink>
        </v-btn>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: 'CreateDocumentPage',
}
</script>
