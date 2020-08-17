<template>
  <v-app>
    <v-app-bar app absolute flat dark color="transparent">
      <div class="d-flex align-center font-weight-black" style="font-family: 'Skranji', cursive; font-size: 1.25rem;">
        ~GameSpot~
      </div>

      <v-spacer></v-spacer>

      <v-btn text>
        Xbox 360
      </v-btn>
      <v-btn text>
        PC
      </v-btn>
      <v-btn text>
        PS2
      </v-btn>
      <v-btn text>
        PS3
      </v-btn>
      <v-btn text>
        PS4
      </v-btn>
    </v-app-bar>

    <v-carousel cycle height="850" hide-delimiter-background show-arrows-on-hover>
      <v-carousel-item v-for="(item, i) in items" :key="i" :src="item.src"> </v-carousel-item>
    </v-carousel>

    <section style="background-color: #121212">
      <v-container>
        <v-row>
          <v-col>
            <v-card class="mx-auto" max-width="300" color="#050505">
              <v-img
                class="white--text align-end"
                height="200px"
                :src="require('../src/assets/assassins_creed_assassin.jpg')"
              ></v-img>
              <v-card-text class="grey--text text--darken-2 body-1">
                Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dignissimos doloremque necessitatibus ullam
                neque ipsa voluptates iusto officiis quis architecto provident, nihil nisi at impedit delectus nostrum
                dolor non fuga recusandae!
              </v-card-text>
            </v-card>
          </v-col>
          <v-col>
            <v-card class="mx-auto" max-width="300" color="#050505">
              <v-img
                class="white--text align-end"
                height="200px"
                :src="require('../src/assets/assassins_creed_black_flagjpg.jpg')"
              ></v-img>
              <v-card-text class="grey--text text--darken-2 body-1">
                Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dignissimos doloremque necessitatibus ullam
                neque ipsa voluptates iusto officiis quis architecto provident, nihil nisi at impedit delectus nostrum
                dolor non fuga recusandae!
              </v-card-text>
            </v-card>
          </v-col>
          <v-col>
            <v-card class="mx-auto" max-width="300" color="#050505">
              <v-img
                class="white--text align-end"
                height="200px"
                :src="require('../src/assets/assassins_creed_desmond_21.jpg')"
              ></v-img>
              <v-card-text class="grey--text text--darken-2 body-1">
                Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dignissimos doloremque necessitatibus ullam
                neque ipsa voluptates iusto officiis quis architecto provident, nihil nisi at impedit delectus nostrum
                dolor non fuga recusandae!
              </v-card-text>
            </v-card>
          </v-col>
          <v-col>
            <v-card dark class="mx-auto" max-width="300" color="#050505">
              <v-img
                class="white--text align-end"
                height="200px"
                :src="require('../src/assets/assassins_creed_revelations_de.jpg')"
              ></v-img>
              <v-card-title>Assassins Creed</v-card-title>
              <v-card-text class="grey--text text--darken-2 body-1">
                Some quick example text to build on the card title and make up the bulk of the card's content.
              </v-card-text>
              <v-card-text class="white--text body-1">
                Assassins Creed Revelation
              </v-card-text>
              <v-card-actions>
                <v-btn color="primary" text>
                  Play
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-col>
          <v-col>
            <v-card dark class="mx-auto" max-width="300" color="#050505">
              <v-img
                class="white--text align-end"
                height="200px"
                :src="require('../src/assets/assassins_creed_iv_black_flag.jpg')"
              ></v-img>
              <v-card-title>Assassins Black Flag</v-card-title>
              <v-card-text class="grey--text text--darken-2 body-1">
                Some quick example text to build on the card title and make up the bulk of the card's content.
              </v-card-text>
              <v-card-text class="white--text body-1">
                Assassins Creed Revelation
              </v-card-text>
              <v-card-actions>
                <v-btn color="primary" text>
                  Play
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </section>

    <section class="section-2">
      <v-card dark class="text-center py-5" color="#050505">
        <h2>Upcaming Games</h2>
        <v-card-text class="grey--text text--darken-2 body-1">
          This is a wider card with supporting text below as a natural lead-in to additional content. This content is a
          little bit longer.
        </v-card-text>
        <v-card-text class="white--text">
          Last updated 3 mins ago
        </v-card-text>
      </v-card>
    </section>

    <section class="section-3 parallex"></section>

    <section class="section-4" style="background-color: #050505">
      <v-container>
        <h1 style="color: crimson; font-size: 2rem">Contact Us</h1>
        <v-row>
          <v-col cols="6">
            <v-text-field light solo label="First Name" color="white"></v-text-field>
          </v-col>
          <v-col cols="6">
            <v-text-field light solo label="Last Name" color="white"></v-text-field>
          </v-col>
          <v-col cols="12">
            <v-text-field light solo label="Email" color="white"></v-text-field>
          </v-col>
          <v-col cols="12">
            <v-textarea light solo label="Message" color="white"></v-textarea>
          </v-col>
        </v-row>
      </v-container>
    </section>

    <v-footer dark style="background-color: #050505">
      <v-col class="text-center" cols="12"
        >Copyright &copy; All rights Resevered <strong style="color: crimson;">Kenneth Pineda</strong>
      </v-col>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: "App",

  components: {},

  data: () => ({
    items: [
      {
        src: require("../src/assets/the_elder_scrolls.jpg"),
      },
      {
        src: require("../src/assets/assassins_creed.jpg"),
      },
      {
        src: require("../src/assets/battlefield_4_game_.jpg"),
      },
    ],
  }),
};
</script>

<style>
.parallex {
  background-image: url("./assets/dark_souls_dark_.jpg");
  background-attachment: fixed;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  height: 500px;
}
</style>
