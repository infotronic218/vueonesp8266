<template>
  <v-app>

    <navigation></navigation>
    <v-main>
      <router-view></router-view>
    </v-main>
  </v-app>
</template>

<script>


import Navigation from "@/components/Navigation";
export default {
  name: 'App',

  components: {
    Navigation

  },

  data: () => ({
    //
  }),
};
</script>
