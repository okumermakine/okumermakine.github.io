<template>
  <v-app>
    <v-main>
      <NavigationBar/>
      <HelloWorld/>
    </v-main>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import NavigationBar from "@/components/NavigationBar";

export default {
  name: 'App',

  components: {
    HelloWorld,
    NavigationBar,
  },

  data: () => ({
    //
  }),
}
</script>
