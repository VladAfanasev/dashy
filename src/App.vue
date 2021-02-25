<template>
  <v-app id="inspire">
    <v-navigation-drawer
      v-model="drawer"
      app
    >
      <!--  -->
    </v-navigation-drawer>

    <v-app-bar app>
      <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>

      <v-toolbar-title>Dashy</v-toolbar-title>
    </v-app-bar>

    <v-main>
      <!--  -->    
      <v-container>
        <v-calendar-weekly
        start="2021-01-01"
        end="2021-12-31"
        weekdays="[1, 2, 3, 4, 5, 6, 0]"
        > </v-calendar-weekly>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
  export default {
    data: () => ({ drawer: null }),
  }
</script>