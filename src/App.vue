<template>
  <v-app>
    <v-navigation-drawer
            app
            v-model="drawer">
      <!-- -->
    </v-navigation-drawer>

      <v-app-bar
              app
              color="white"
              elevate-on-scroll
              scroll-target="#scrolling-techniques-7"
      >
        <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>

        <v-toolbar-title>Title</v-toolbar-title>

        <v-spacer></v-spacer>

        <v-btn icon>
          <v-icon>mdi-magnify</v-icon>
        </v-btn>

        <v-btn icon>
          <v-icon>mdi-heart</v-icon>
        </v-btn>

        <v-btn icon>
          <v-icon>mdi-dots-vertical</v-icon>
        </v-btn>
      </v-app-bar>
<!--      <v-sheet
              id="scrolling-techniques-7"
              class="overflow-y-auto purple"
              max-height="950"
      >
        <v-container app style="height: 1500px;">
          <div>
            <h1 class="text&#45;&#45;white">Hola Mundo</h1>
          </div>
        </v-container>
      </v-sheet>-->
    <v-content
            id="scrolling-techniques-7"
            class="overflow-auto"

    >

      <!-- Provides the application the proper gutter -->
      <v-container fluid>
        <h1>Hola Mundo</h1>
        <!-- If using vue-router -->
      </v-container>
    </v-content>

    <v-footer app>
      <!-- -->
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: 'App',
  data(){
    if (screen.width<1024){
      return{
        drawer: false
      }
    }else{
      return{
        drawer: true
      }
    }

  }
};
</script>
