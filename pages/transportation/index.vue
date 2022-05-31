<template>
  <v-row align="center" class="border">
    <v-col class="p-2">
      <h2>Bagian Transportasi & Pemeliharaan</h2>

      <div>
        <v-card
          v-for="(item, index) in items"
          :key="index"
          class="d-flex flex-row mb-6 pa-4"
          outline
          tile
          width="200"
          height="auto"
        >
          <div>
            <div>
              <img :src="item.icon" alt="icon" width="40" />
            </div>
            <div>
              <NuxtLink :to="item.link"> {{ item.name }} </NuxtLink>
            </div>
          </div>
        </v-card>
      </div>
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: 'TransportationPage',
  data() {
    return {
      items: [
        {
          name: 'Data Truk',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Data Supir',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Data Pemeliharaan Ban',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
      ],
    }
  },
}
</script>
