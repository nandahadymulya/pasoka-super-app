<template>
  <v-row>
    <v-col cols="8">
      <h2 class="text-center">Bagian Umum & Sistem Manajemen</h2>
      <p>Struktur Organisasi</p>
      <p>Kepala Bagian</p>
      <p>Kepala Seksi</p>
      <p>Anggota</p>
    </v-col>

    <v-col cols="4">
      Daftar Menu
      <v-container>
        <v-row>
          <v-col v-for="(item, index) in items" :key="index">
            <v-card
              class="rounded justify-center"
              outline
              tile
              width="140"
              height="100"
            >
              <div>
                <img :src="item.icon" alt="icon" width="36" />
              </div>
              <div>
                <NuxtLink :to="item.link"> {{ item.name }} </NuxtLink>
              </div>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: 'GeneralPage',
  data() {
    return {
      items: [
        {
          name: 'Dokumen',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Daftar Permohonan',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Daftar Lelang',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Dokumen',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Daftar Permohonan',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Daftar Lelang',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Dokumen',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Daftar Permohonan',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Daftar Lelang',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Dokumen',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Daftar Permohonan',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Daftar Lelang',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Dokumen',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Daftar Permohonan',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Daftar Lelang',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Dokumen',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Daftar Permohonan',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Daftar Lelang',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Dokumen',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Daftar Permohonan',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Daftar Lelang',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Daftar Lelang',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Daftar Lelang',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Daftar Lelang',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Daftar Lelang',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Daftar Lelang',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Daftar Lelang',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Daftar Lelang',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Daftar Lelang',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
        {
          name: 'Daftar Lelang',
          icon: 'assets/icons/document.svg',
          link: '/general/documents',
        },
      ],
    }
  },
}
</script>
