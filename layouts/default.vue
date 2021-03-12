<template>
  <v-app>
    <v-app-bar app color="indigo" dark flat>
      <v-container class="py-0 fill-height">
        <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
        <v-spacer></v-spacer>
        <v-toolbar-title>SKYCAR</v-toolbar-title>
        <v-spacer></v-spacer>
        <v-avatar class="mr-10" color="white" size="32"></v-avatar>
      </v-container> </v-app-bar
    ><v-navigation-drawer v-model="drawer" absolute temporary>
      <v-list nav dense>
        <v-list-item-group
          v-model="group"
          active-class="deep-purple--text text--accent-4"
        >
          <v-list-item>
            <v-list-item-title>Foo</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title>Bar</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title>Fizz</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title>Buzz</v-list-item-title>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>

    <v-main class="grey lighten-3">
      <v-container> <nuxt /> </v-container
    ></v-main>
  </v-app>
</template>

<script>
export default {
  data: () => ({
    drawer: false,
    group: null,
  }),

  watch: {
    group() {
      this.drawer = false
    },
  },
  title: 'CAR rental',
}
</script>
