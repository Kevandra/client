<template>
  <v-container>
    <!-- <v-row align="center">
    <v-date-picker
      v-model="date"
      full-width
      class="mt-4"
    ></v-date-picker>
    </v-row> -->

    <v-row>
      <v-col>
        <v-card>
          <!-- <v-card-actions> -->
            <!-- <v-col>Bagaimana kegiatan hari ini?
              <template>
                <div class="text-center">
                  <v-dialog
                    v-model="dialog"
                    width="500"
                  >
                    <template v-slot:activator="{ on, attrs }">
                      <v-btn
                        v-bind="attrs"
                        v-on="on"
                      >
                        <v-icon large>
                          mdi-plus
                        </v-icon>
                      </v-btn>
                    </template>

                    <v-card>
                      <v-card-title class="text-h5 grey lighten-2">
                        Pertanyaan
                      </v-card-title>

                      <v-card-text>
                        <v-text-field
                          v-model="title"
                          :rules="rules"
                          counter="25"
                          hint="Jawaban"
                          label="Jawaban"
                        ></v-text-field>
                      </v-card-text>

                      <v-divider></v-divider>

                      <v-card-actions>
                        <v-spacer></v-spacer>
                        <v-btn
                          color="primary"
                          text
                          @click="onsubmit"
                        >
                          Submit
                        </v-btn>
                      </v-card-actions>
                    </v-card>
                  </v-dialog>
                </div>
              </template>
            </v-col>
          </v-card-actions>
        </v-card>
      </v-col>
      <v-col>
        <v-card>
          <v-card-actions>
            <v-col>Bagaimana perasaan mu hari ini?
              <template>
                <div class="text-center">
                  <v-dialog
                    v-model="dialog"
                    width="500"
                  >
                    <template v-slot:activator="{ on, attrs }">
                      <v-btn
                        v-bind="attrs"
                        v-on="on"
                      >
                        <v-icon large>
                          mdi-plus
                        </v-icon>
                      </v-btn>
                    </template>

                    <v-card>
                      <v-card-title class="text-h5 grey lighten-2">
                        Pertanyaan
                      </v-card-title>

                      <v-card-text>
                        <v-text-field
                          v-model="title"
                          :rules="rules"
                          counter="25"
                          hint="Jawaban"
                          label="Jawaban"
                        ></v-text-field>
                      </v-card-text>

                      <v-divider></v-divider>

                      <v-card-actions>
                        <v-spacer></v-spacer>
                        <v-btn
                          color="primary"
                          text
                          @click="dialog = false"
                        >
                          Submit
                        </v-btn>
                      </v-card-actions>
                    </v-card>
                  </v-dialog>
                </div>
              </template>
            </v-col>
          </v-card-actions>
        </v-card>
      </v-col>
      <v-col>
        <v-card>
          <v-card-actions>
            <v-col>Apa saja yang akan dilakukan untuk hari ini?
              <template>
                <div class="text-center">
                  <v-dialog
                    v-model="dialog"
                    width="500"
                  >
                    <template v-slot:activator="{ on, attrs }">
                      <v-btn
                        v-bind="attrs"
                        v-on="on"
                      >
                        <v-icon large>
                          mdi-plus
                        </v-icon>
                      </v-btn>
                    </template>

                    <v-card>
                      <v-card-title class="text-h5 grey lighten-2">
                        Pertanyaan
                      </v-card-title>

                      <v-card-text>
                        <v-text-field
                          v-model="title"
                          :rules="rules"
                          counter="25"
                          hint="Jawaban"
                          label="Jawaban"
                        ></v-text-field>
                      </v-card-text>

                      <v-divider></v-divider>

                      <v-card-actions>
                        <v-spacer></v-spacer>
                        <v-btn
                          color="primary"
                          text
                          @click="dialog = false"
                        >
                          Submit
                        </v-btn>
                      </v-card-actions>
                    </v-card>
                  </v-dialog>
                </div>
              </template>
            </v-col>
          </v-card-actions>
        </v-card>
      </v-col>
      <v-col>
        <v-card>
          <v-card-actions>
            <v-col>Apakah ada hal yang membuat mu senang?
              <template>
                <div class="text-center">
                  <v-dialog
                    v-model="dialog"
                    width="500"
                  >
                    <template v-slot:activator="{ on, attrs }">
                      <v-btn
                        v-bind="attrs"
                        v-on="on"
                      >
                        <v-icon large>
                          mdi-plus
                        </v-icon>
                      </v-btn>
                    </template>

                    <v-card>
                      <v-card-title class="text-h5 grey lighten-2">
                        Pertanyaan
                      </v-card-title>

                      <v-card-text>
                        <v-text-field
                          v-model="title"
                          :rules="rules"
                          counter="25"
                          hint="Jawaban"
                          label="Jawaban"
                        ></v-text-field>
                      </v-card-text>

                      <v-divider></v-divider>

                      <v-card-actions>
                        <v-spacer></v-spacer>
                        <v-btn
                          color="primary"
                          text
                          @click="dialog = false"
                        >
                          Submit
                        </v-btn>
                      </v-card-actions>
                    </v-card>
                  </v-dialog>
                </div>
              </template>
            </v-col>
          </v-card-actions>
        </v-card>
      </v-col>
      <v-col>
        <v-card>
          <v-card-actions>
            <v-col>Bagaimana jika cuaca hari ini buruk?
              <template>
                <div class="text-center">
                  <v-dialog
                    v-model="dialog"
                    width="500"
                  >
                    <template v-slot:activator="{ on, attrs }">
                      <v-btn
                        v-bind="attrs"
                        v-on="on"
                      >
                        <v-icon large>
                          mdi-plus
                        </v-icon>
                      </v-btn>
                    </template>

                    <v-card>
                      <v-card-title class="text-h5 grey lighten-2">
                        Pertanyaan
                      </v-card-title>

                      <v-card-text>
                        <v-text-field
                          v-model="title"
                          :rules="rules"
                          counter="25"
                          hint="Jawaban"
                          label="Jawaban"
                        ></v-text-field>
                      </v-card-text>

                      <v-divider></v-divider>

                      <v-card-actions>
                        <v-spacer></v-spacer>
                        <v-btn
                          color="primary"
                          text
                          @click="dialog = false"
                        >
                          Submit
                        </v-btn>
                      </v-card-actions>
                    </v-card>
                  </v-dialog>
                </div>
              </template>
            </v-col>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
    <v-row>
      <v-col>
        <v-card>
          <v-card-actions>
            <v-col>Tugas apa yang biasa kamu kerjakan?
              <template>
                <div class="text-center">
                  <v-dialog
                    v-model="dialog"
                    width="500"
                  >
                    <template v-slot:activator="{ on, attrs }">
                      <v-btn
                        v-bind="attrs"
                        v-on="on"
                      >
                        <v-icon large>
                          mdi-plus
                        </v-icon>
                      </v-btn>
                    </template>

                    <v-card>
                      <v-card-title class="text-h5 grey lighten-2">
                        Pertanyaan
                      </v-card-title>

                      <v-card-text>
                        <v-text-field
                          v-model="title"
                          :rules="rules"
                          counter="25"
                          hint="Jawaban"
                          label="Jawaban"
                        ></v-text-field>
                      </v-card-text>

                      <v-divider></v-divider>

                      <v-card-actions>
                        <v-spacer></v-spacer>
                        <v-btn
                          color="primary"
                          text
                          @click="dialog = false"
                        >
                          Submit
                        </v-btn>
                      </v-card-actions>
                    </v-card>
                  </v-dialog>
                </div>
              </template>
            </v-col>
          </v-card-actions>
        </v-card>
      </v-col>
      <v-col>
        <v-card>
          <v-card-actions>
            <v-col>Makananan favorit mu apa?
              <template>
                <div class="text-center">
                  <v-dialog
                    v-model="dialog"
                    width="500"
                  >
                    <template v-slot:activator="{ on, attrs }">
                      <v-btn
                        v-bind="attrs"
                        v-on="on"
                      >
                        <v-icon large>
                          mdi-plus
                        </v-icon>
                      </v-btn>
                    </template>

                    <v-card>
                      <v-card-title class="text-h5 grey lighten-2">
                        Pertanyaan
                      </v-card-title>

                      <v-card-text>
                        <v-text-field
                          v-model="title"
                          :rules="rules"
                          counter="25"
                          hint="Jawaban"
                          label="Jawaban"
                        ></v-text-field>
                      </v-card-text>

                      <v-divider></v-divider>

                      <v-card-actions>
                        <v-spacer></v-spacer>
                        <v-btn
                          color="primary"
                          text
                          @click="dialog = false"
                        >
                          Submit
                        </v-btn>
                      </v-card-actions>
                    </v-card>
                  </v-dialog>
                </div>
              </template>
            </v-col>
          </v-card-actions>
        </v-card>
      </v-col>
      <v-col>
        <v-card>
          <v-card-actions>
            <v-col>Buku favorit mu bercerita tentang apa?
              <template>
                <div class="text-center">
                  <v-dialog
                    v-model="dialog"
                    width="500"
                  >
                    <template v-slot:activator="{ on, attrs }">
                      <v-btn
                        v-bind="attrs"
                        v-on="on"
                      >
                        <v-icon large>
                          mdi-plus
                        </v-icon>
                      </v-btn>
                    </template>

                    <v-card>
                      <v-card-title class="text-h5 grey lighten-2">
                        Pertanyaan
                      </v-card-title>

                      <v-card-text>
                        <v-text-field
                          v-model="title"
                          :rules="rules"
                          counter="25"
                          hint="Jawaban"
                          label="Jawaban"
                        ></v-text-field>
                      </v-card-text>

                      <v-divider></v-divider>

                      <v-card-actions>
                        <v-spacer></v-spacer>
                        <v-btn
                          color="primary"
                          text
                          @click="dialog = false"
                        >
                          Submit
                        </v-btn>
                      </v-card-actions>
                    </v-card>
                  </v-dialog>
                </div>
              </template>
            </v-col>
          </v-card-actions>
        </v-card>
      </v-col>
      <v-col>
        <v-card>
          <v-card-actions>
            <v-col>Jika merasa senang kamu melakukan apa?
              <template>
                <div class="text-center">
                  <v-dialog
                    v-model="dialog"
                    width="500"
                  >
                    <template v-slot:activator="{ on, attrs }">
                      <v-btn
                        v-bind="attrs"
                        v-on="on"
                      >
                        <v-icon large>
                          mdi-plus
                        </v-icon>
                      </v-btn>
                    </template>

                    <v-card>
                      <v-card-title class="text-h5 grey lighten-2">
                        Pertanyaan
                      </v-card-title>

                      <v-card-text>
                        <v-text-field
                          v-model="title"
                          :rules="rules"
                          counter="25"
                          hint="Jawaban"
                          label="Jawaban"
                        ></v-text-field>
                      </v-card-text>

                      <v-divider></v-divider>

                      <v-card-actions>
                        <v-spacer></v-spacer>
                        <v-btn
                          color="primary"
                          text
                          @click="dialog = false"
                        >
                          Submit
                        </v-btn>
                      </v-card-actions>
                    </v-card>
                  </v-dialog>
                </div>
              </template>
            </v-col>
          </v-card-actions>
        </v-card>
      </v-col>
      <v-col>
        <v-card>
          <v-card-actions>
            <v-col>Apakah kamu sering keluar rumah?
              <template>
                <div class="text-center">
                  <v-dialog
                    v-model="dialog"
                    width="500"
                  >
                    <template v-slot:activator="{ on, attrs }">
                      <v-btn
                        v-bind="attrs"
                        v-on="on"
                      >
                        <v-icon large>
                          mdi-plus
                        </v-icon>
                      </v-btn>
                    </template>

                    <v-card>
                      <v-card-title class="text-h5 grey lighten-2">
                        Pertanyaan
                      </v-card-title>

                      <v-card-text>
                        <v-text-field
                          v-model="title"
                          :rules="rules"
                          counter="25"
                          hint="Jawaban"
                          label="Jawaban"
                        ></v-text-field>
                      </v-card-text>

                      <v-divider></v-divider>

                      <v-card-actions>
                        <v-spacer></v-spacer>
                        <v-btn
                          color="primary"
                          text
                          @click="dialog = false"
                        >
                          Submit
                        </v-btn>
                      </v-card-actions>
                    </v-card>
                  </v-dialog>
                </div>
              </template>
            </v-col> -->
          <!-- </v-card-actions> -->
        </v-card>
      </v-col>
    </v-row>
    <v-alert border="left" close-text="Close Alert" color="red accent-4" dark dismissible
      v-if="this.$route.params.message">
      {{ this.$route.params.message }}
    </v-alert>
    <v-row no-gutters>
      <v-col sm="4" class="pa-3" v-for="post in posts" :key="post._id">
        <v-card class="pa-1" :to="{ name: 'post', params: { id: post._id } }">
          <v-img height="550" :src="`/${post.image}`"></v-img>
          <v-btn class="ml-4 mt-3" small outlined color="indigo">
            {{ post.category }}
          </v-btn>
          <v-card-title class="headline">
            {{ post.title }}
          </v-card-title>
          <v-card-text class="py-0">
            <p>{{ post.content.substring(0, 100) + "..." }}</p>
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import API from '../api';

export default {
  name: 'Home',
  data() {
    return {
      posts: [],
      dialog: false,
      date: (new Date(Date.now() - (new Date()).getTimezoneOffset() * 60000)).toISOString().substr(0, 10),
      title:  null
    };
  },
  async created() {
    this.posts = await API.getAllPost();
    console.log(this.posts);
  },
  methods(){
    async function onsubmit(){
      this.dialog = false
      console.log(this.title)
    }
  }
};

</script>
