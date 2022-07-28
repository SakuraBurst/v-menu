<template>
  <v-container class="d-flex flex-column width300" >
    <v-menu absolute min-width="100">
      <template v-slot:activator="{ on, attrs }">
        <v-btn v-on="on"  v-bind="attrs">df</v-btn>
      </template>
      <v-card> lorem ipsum </v-card>
    </v-menu>

    <v-menu :attach="'#one'" absolute>
      <template v-slot:activator="{ on, attrs }">
        <v-btn v-on="on" id="one" v-bind="attrs">df</v-btn>
      </template>
      <v-card> lorem ipsum </v-card>
    </v-menu>
  </v-container>
</template>

<script>
  export default {
    name: 'HelloWorld',

    data: () => ({
      ecosystem: [
        {
          text: 'vuetify-loader',
          href: 'https://github.com/vuetifyjs/vuetify-loader',
        },
        {
          text: 'github',
          href: 'https://github.com/vuetifyjs/vuetify',
        },
        {
          text: 'awesome-vuetify',
          href: 'https://github.com/vuetifyjs/awesome-vuetify',
        },
      ],
      importantLinks: [
        {
          text: 'Documentation',
          href: 'https://vuetifyjs.com',
        },
        {
          text: 'Chat',
          href: 'https://community.vuetifyjs.com',
        },
        {
          text: 'Made with Vuetify',
          href: 'https://madewithvuejs.com/vuetify',
        },
        {
          text: 'Twitter',
          href: 'https://twitter.com/vuetifyjs',
        },
        {
          text: 'Articles',
          href: 'https://medium.com/vuetify',
        },
      ],
      whatsNext: [
        {
          text: 'Explore components',
          href: 'https://vuetifyjs.com/components/api-explorer',
        },
        {
          text: 'Select a layout',
          href: 'https://vuetifyjs.com/getting-started/pre-made-layouts',
        },
        {
          text: 'Frequently Asked Questions',
          href: 'https://vuetifyjs.com/getting-started/frequently-asked-questions',
        },
      ],
    }),
  }
</script>
<style>
.width300 {
  width: 300px;
}
</style>