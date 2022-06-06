<template>
  <div>
    <v-card width="200" color="grey lighten-3" flat>
      <v-list-item>
        <v-list-item-content class="text-left">
          <v-layout>
            <v-icon size="48">mdi-folder-open-outline</v-icon>
            <v-spacer></v-spacer>
            <v-btn icon>
              <v-icon>mdi-dots-vertical</v-icon>
            </v-btn>
          </v-layout>

          <v-list-item-title class="my-2">General</v-list-item-title>
          <v-list-item-subtitle>
            <v-layout wrap>
              <span>Khaira Yasri</span>
              <v-spacer></v-spacer>
              <b>Ka. Bag. Umum</b>
            </v-layout>
          </v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>
    </v-card>
  </div>
</template>
<script>
export default {
  name: 'CardComponent',
}
</script>
