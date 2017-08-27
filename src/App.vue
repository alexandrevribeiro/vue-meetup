<template>
  <v-app light>

    <v-navigation-drawer v-model="showSideNav">
       <v-list>
        <v-list-tile>
          <v-list-tile-action>
            <v-icon>supervisor_account</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>View Meetups</v-list-tile-content>
        </v-list-tile>
      </v-list> 
    </v-navigation-drawer>

    <v-toolbar dark class="primary">
      <v-toolbar-side-icon 
        @click.stop="showSideNav = !showSideNav"
        class="hidden-sm-and-up"></v-toolbar-side-icon>
      <v-toolbar-title>Meetup</v-toolbar-title>      
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-xl-only">
        <v-btn flat>
          <v-icon left>supervisor_account</v-icon>
          View Meetups
          </v-btn>
      </v-toolbar-items>
    </v-toolbar>
    <main>

    </main>
  </v-app>
</template>

<script>
  export default {
    data () {
      return {
        showSideNav: false
      }
    }
  }
</script>

<style lang="stylus">
  @require './stylus/main'
</style>
