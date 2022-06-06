<template>
  <div>
    <main class="bg-primary">A</main>
    <v-row>
      <v-col>
        <v-container>
          <h1>Daftar Fitur</h1>
          <p>Super App PT Pasoka Sumber Karya.</p>
          <br />
          <hr />
          <br />
          <v-list>
            <v-list-item>
              <NuxtLink to="/">Landing Page is here!</NuxtLink>
              <v-spacer></v-spacer>
              <p>
                Halaman profil perusahaan, dengan fitur / halaman yang dapat
                diakses eksternal.
              </p>
            </v-list-item>
            <v-list-item>
              <NuxtLink to="/login">Login Page</NuxtLink>
              <v-spacer></v-spacer>
              <p>
                Halaman authentikasi untuk dapat masuk ke halaman manajemen
                perusahaan / dashboard.
              </p>
            </v-list-item>
            <v-list-item>
              <NuxtLink to="/forms">Form Page</NuxtLink>
              <v-spacer></v-spacer>
              <p>
                Halaman pengajuan dokumen untuk dapat diakses oleh user / tenaga
                kerja.
              </p>
            </v-list-item>
            <v-list-item>
              <NuxtLink to="/dashboard">Dashboard Page</NuxtLink>
              <v-spacer></v-spacer>
              <p>Halaman manajemen perusahaan.</p>
            </v-list-item>
          </v-list>
        </v-container>
      </v-col>
    </v-row>
  </div>
</template>
<script>
export default {
  name: 'LandingPage',
  layout: 'blank',
}
</script>
