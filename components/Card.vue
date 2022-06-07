<template>
  <div>
    <v-card v-bind="$attrs" v-on="$listeners">
      <v-list-item>
        <v-list-item-content class="text-left">
          <v-layout>
            <v-icon size="48">{{ icon }}</v-icon>
            <v-spacer></v-spacer>
            <v-btn icon>
              <v-icon>mdi-dots-vertical</v-icon>
            </v-btn>
          </v-layout>

          <v-list-item-title class="my-2">{{ title }}</v-list-item-title>
          <v-list-item-subtitle>
            <v-layout wrap>
              <span>{{ fieldCount }}</span>
              <v-spacer></v-spacer>
              <b>{{ fieldSize }} MB</b>
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
  inheritAttrs: false,
  props: {
    title: {
      type: String,
      default: 'Title',
    },
    fieldSize: {
      type: String,
      default: '0',
    },
    icon: {
      type: String,
      default: 'mdi-folder-open-outline',
    },
    fieldCount: {
      type: String,
      default: '0 file',
    },
  },
}
</script>
