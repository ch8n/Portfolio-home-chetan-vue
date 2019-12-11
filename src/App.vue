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
        <!-- my intro -->
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
            <v-icon>mdi-emoticon-happy-outline</v-icon>
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

        <!-- recommendations -->
        <v-card height="500px" width="50%" class="ma-2">
          <v-carousel cycle class="fill-height" hide-delimiter-background show-arrows-on-hover>
            <v-carousel-item>
              <v-card class="pa-10 fill-height" color="#0e76a8" dark>
                <v-card-title>
                  <v-icon large left>mdi-linkedin</v-icon>
                  <span class="display-1 font-weight-bold">LinkedIn</span>
                </v-card-title>

                <v-card-text
                  class="title font-weight-bold"
                >"Chetan is a very hardworking and responsible guy. He can implement and craft very good and detailed user interfaces. He managed to build a great and always changing android application. He is always learning and growing as a developer. Highly recommend working with him."</v-card-text>

                <v-card-actions>
                  <v-list-item class="grow">
                    <a href="https://www.linkedin.com/in/abdulazizalaa/" target="_blank">
                      <v-list-item-avatar color="grey darken-3">
                        <v-img
                          class="elevation-6"
                          src="https://media.licdn.com/dms/image/C5603AQG8BcuwFy2dCg/profile-displayphoto-shrink_100_100/0?e=1581552000&v=beta&t=UJw3osomCGwb_hAGKkzLVCIXE9bQYzQM50-Lm6WQJtI"
                        />
                      </v-list-item-avatar>
                    </a>
                    <v-list-item-content>
                      <v-list-item-title>Abdulaziz Mohamed Alaa</v-list-item-title>
                      <v-list-item-title>Artificial Intelligence Engineer at Mendel.ai</v-list-item-title>
                    </v-list-item-content>
                  </v-list-item>
                </v-card-actions>
              </v-card>
            </v-carousel-item>

            <v-carousel-item>
              <v-card class="pa-10 fill-height" color="#0e76a8" dark>
                <v-card-title>
                  <v-icon large left>mdi-linkedin</v-icon>
                  <span class="display-1 font-weight-bold">LinkedIn</span>
                </v-card-title>

                <v-card-text class="title font-weight-bold">
                  "Chetan is creative, detail-oriented and very hard-working. It is his passion for the task that drives him to perform to his level best. As a techie, I've known him to be committed to his projects while being a perfectionist at what he does.
                  I would like to recommend him as I believe that Chetan would be an asset to any team. "
                </v-card-text>

                <v-card-actions>
                  <v-list-item class="grow">
                    <a href="https://www.linkedin.com/in/siddharthsudhakar/" target="_blank">
                      <v-list-item-avatar color="grey darken-3">
                        <v-img
                          class="elevation-6"
                          src="https://media.licdn.com/dms/image/C4E03AQHaCyCX_Wmf5Q/profile-displayphoto-shrink_100_100/0?e=1581552000&v=beta&t=CG4FOa_NrPrypvH2N86F19UlSZwX5ujAIWvH3jVJQGo"
                        />
                      </v-list-item-avatar>
                    </a>
                    <v-list-item-content>
                      <v-list-item-title>Siddharth Sudhakar</v-list-item-title>
                      <v-list-item-title>CEO, D2K Innovation Labs India Pvt. Ltd.</v-list-item-title>
                    </v-list-item-content>
                  </v-list-item>
                </v-card-actions>
              </v-card>
            </v-carousel-item>
          </v-carousel>
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