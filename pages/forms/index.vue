<template>
  <v-row align="center" class="border">
    <v-col class="p-2">
      <h2>Daftar Form</h2>
      <v-card elevation="2" height="500">
        <v-list>
          <v-list-item
            v-for="(item, i) in items"
            :key="i"
            :to="item.to"
            router
            exact
          >
            <v-list-item-action class="white--text">
              <v-icon>{{ item.icon }}</v-icon>
            </v-list-item-action>
            <v-list-item-content class="white--text">
              <v-list-item-title v-text="item.title" />
            </v-list-item-content>
          </v-list-item>
        </v-list>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: 'FormsPage',
  layout: 'blank',
}
</script>
