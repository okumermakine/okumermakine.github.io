<template>
  <v-app>
    <v-main>
      <NavigationBar/>
      <HelloWorld class="mt-5"/>
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
