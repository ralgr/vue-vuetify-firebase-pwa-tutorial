<template>
  <v-app>
    <v-toolbar app>

      <v-btn icon
             v-if="$route.name !== 'home'"
             @click="$router.go(-1)">
             <v-icon>arrow_back</v-icon>
      </v-btn>

      <v-toolbar-title class="headline">
        <span>Dogschat</span>
      </v-toolbar-title>

      <v-spacer></v-spacer>

    </v-toolbar>

    <v-content>
      <router-view></router-view>
    </v-content>
  </v-app>
</template>

<script>
export default {
  name: 'App',
  components: {
  },
  data () {
    return {
      //
    }
  }
}
</script>
