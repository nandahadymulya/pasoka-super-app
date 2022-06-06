<template>
  <div>
    <v-container grid-list-xs fluid>
      <v-row>
        <v-col cols="12" md="9">
          <v-layout wrap>
            <h3 class="title grey--text">Perbendaharaan</h3>
            <v-spacer></v-spacer>
            <v-btn icon>
              <v-icon>mdi-arrow-right</v-icon>
            </v-btn>
          </v-layout>
        </v-col>
        <v-col cols="12" md="3"></v-col>
      </v-row>
      <v-row>
        <v-col>
          <CardComponent />
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
import CardComponent from '@/components/Card.vue'

export default {
  name: 'TreasuryPage',
  components: {
    CardComponent,
  },
}
</script>
