<template>
  <div>
    <v-navigation-drawer
      v-model="drawer"
      class="grey"
      :mini-variant="miniVariant"
      :clipped="clipped"
      fixed
      app
    >
      <v-row>
        <v-col>
          <v-list-item height="300 purple">
            <v-list-item-content>
              <v-list-item-title class="text-h4"> PASOKA </v-list-item-title>
              <v-list-item-subtitle> Everything is here! </v-list-item-subtitle>
            </v-list-item-content>
          </v-list-item>
        </v-col>
        <v-divider></v-divider>
        <v-col>
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
        </v-col>
      </v-row>
      <v-spacer></v-spacer>
      <v-row>
        <v-col>
          <v-avatar color="indigo">
            <v-icon dark> mdi-account-circle </v-icon>
          </v-avatar>
        </v-col>
      </v-row>
    </v-navigation-drawer>
  </div>
</template>
<script>
export default {
  name: 'SidebarComponent',
  data() {
    return {
      clipped: false,
      drawer: true,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Dashboard',
          to: '/dashboard',
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Akuntansi',
          to: '/accounting',
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Kontruksi',
          to: '/construction',
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'SDM',
          to: '/human-resources',
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Transportasi',
          to: '/transportation',
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Umum',
          to: '/general',
        },
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
    }
  },
}
</script>
