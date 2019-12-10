<template>
  <v-app>
    <!-- app drawer-->
    <v-card>
      <v-navigation-drawer
        app
        class="nav-drawer"
        v-model="drawer"
        :mini-variant="true"
        permanent
        height="700px"
      >
        <v-divider></v-divider>

        <v-list-item link>
          <v-list-item-icon>
            <v-tooltip right>
              <template v-slot:activator="{ on }">
                <v-avatar v-on="on" size="48">
                  <img src="https://avatars1.githubusercontent.com/u/11576342?v=3" alt="CG" />
                </v-avatar>
              </template>
              <span>Hello! ~(^_^)~</span>
            </v-tooltip>
          </v-list-item-icon>
        </v-list-item>

        <v-divider></v-divider>

        <v-list-item link>
          <v-list-item-icon>
            <v-tooltip right>
              <template v-slot:activator="{ on }">
                <v-icon v-on="on">mdi-coffee</v-icon>
              </template>
              <span>Work experience</span>
            </v-tooltip>
          </v-list-item-icon>
        </v-list-item>

        <v-list-item link>
          <v-list-item-icon>
            <v-tooltip right>
              <template v-slot:activator="{ on }">
                <v-icon v-on="on">mdi-book-open-page-variant</v-icon>
              </template>
              <span>Blogs and Tutorials</span>
            </v-tooltip>
          </v-list-item-icon>
        </v-list-item>

        <v-list-item link>
          <v-list-item-icon>
            <v-tooltip right>
              <template v-slot:activator="{ on }">
                <v-icon v-on="on">mdi-google-play</v-icon>
              </template>
              <span>My PlayStore Apps</span>
            </v-tooltip>
          </v-list-item-icon>
        </v-list-item>

        <v-list-item link>
          <v-list-item-icon>
            <v-tooltip right>
              <template v-slot:activator="{ on }">
                <v-icon v-on="on">mdi-android</v-icon>
              </template>
              <span>My Android Apps</span>
            </v-tooltip>
          </v-list-item-icon>
        </v-list-item>

        <v-list-item link>
          <v-list-item-icon>
            <v-tooltip right>
              <template v-slot:activator="{ on }">
                <v-icon v-on="on">mdi-code-braces-box</v-icon>
              </template>
              <span>Other Projects</span>
            </v-tooltip>
          </v-list-item-icon>
        </v-list-item>

        <v-list-item link>
          <v-list-item-icon>
            <v-tooltip right>
              <template v-slot:activator="{ on }">
                <v-icon v-on="on">mdi-face</v-icon>
              </template>
              <span>Contact me</span>
            </v-tooltip>
          </v-list-item-icon>
        </v-list-item>
      </v-navigation-drawer>
    </v-card>

    <!-- app toolbar -->
    <v-app-bar app>
      <v-toolbar-title class="toolbar-brand">Home</v-toolbar-title>
      <v-spacer />

      <v-toolbar-items>
        <v-btn text>Blogs</v-btn>
        <v-btn text>Chetan Gupta</v-btn>
      </v-toolbar-items>
    </v-app-bar>

    <!-- app body/content -->
    <v-content>
      <v-container class="d-flex flex-row">
        <v-card height="500px" width="50%" class="d-flex flex-column ma-2">
          <p class="mt-6 ml-6 display-2">Chetan Gupta</p>
          <blockquote class="blockquote mt-n4">
            Hello there! I go in community with the name Ch8n.
            I'm a mobile technology enthusiast! love Android
            <code>#kotlinAlltheWay</code>, want to explore all opportunity around it!
            <br />
            <code class="mt-2">CodingMantra: #cleanCoder, #TDD, #SOLID, #designpatterns</code>
          </blockquote>

          <p class="ml-7 mt-10 font-weight-light">
            Have a look around my website, don't forget to see my tech blogs
            you will absolutly find something interesting, feel free to leave comments
            and feedbacks.
            <br />
            <v-icon >mdi-emoticon-happy-outline</v-icon>
          </p>

          <v-spacer />
          <div class="d-flex flex-row ml-6 mt-n4" width="100px">
            <v-icon class="ml-2 display-1">mdi-github-circle</v-icon>
            <v-icon class="ml-3 display-1">mdi-twitter</v-icon>
            <v-icon class="ml-3 display-1">mdi-facebook-box</v-icon>
            <v-icon class="ml-3 display-1">mdi-instagram</v-icon>
            <v-icon class="ml-3 display-1">mdi-linkedin-box</v-icon>
          </div>
          <p class="ml-7 headline">
            Android Developer
            <v-icon class="display-1">mdi-android-head</v-icon>
          </p>
        </v-card>

        <v-card height="500px" width="50%" class="ma-2">
          <v-card-title class="headline">Unlimited music now</v-card-title>

          <v-card-subtitle>Listen to your favorite artists and albums whenever and wherever, online and offline.</v-card-subtitle>

          <v-card-actions>
            <v-btn text>Listen Now</v-btn>
          </v-card-actions>
        </v-card>
      </v-container>
    </v-content>
  </v-app>
</template>

<script>
export default {
  name: "App",
  data: () => ({
    drawer: true
  })
};
</script>

<style scoped>
.nav-drawer {
  padding-top: 80px;
}
.nav-drawer-avatar {
  padding-top: 16px;
  padding-bottom: 16px;
}
.toolbar-brand {
  margin-left: 32px;
}
</style>