<template>
  <v-app :style="{ background: $vuetify.theme.themes.dark.background }">
    <SideBar />
    <NavBar />
    <v-container fluid>
      <v-app-bar dark color="transparent" flat>
        <v-tabs color="#f34f64" v-model="tab">
          <v-tabs-slider color="#f34f64"></v-tabs-slider>
          <v-tab class="withoutupercase">Paresut</v-tab>
          <v-tab class="withoutupercase">Parke</v-tab>
          <v-tab class="withoutupercase">Steve</v-tab>
          <v-tab class="withoutupercase">Dennise</v-tab>
        </v-tabs>
      </v-app-bar>  
      <v-card tile color="#323b50" class="my-2 card_global">
        <v-row>
          <v-col cols="12" sm="8">
            <v-tabs-items v-model="tab">
              <v-tab-item>
                <v-card color="#323b50" flat class="card_item pa-2">
                  <v-row>
                    <v-col cols="12" sm="3" v-for="(parasut, i) in parasuts" :key="i">
                      <v-hover v-slot="{hover}" close-delay="200">
                        <v-card :elevation="hover ? 16 : 2" :class="{ 'on-hover' :hover }"
                        class="mx-auto" height="250" tile color="#333c51" align="center">
                          <v-card-actions>
                            <v-spacer></v-spacer>
                            <v-btn tile small :color="hover ? '#f34f64' : '#777d8b'" dark>
                              {{ parasut.price }}
                            </v-btn>
                          </v-card-actions>
                          <v-img src="../image/shirt-2.jpg" width="150" height="150"></v-img>
                          <v-card-text :class="hover ? 'red--text' : 'white--text'">
                            {{ parasut.title }}
                          </v-card-text>
                        </v-card> 
                      </v-hover>
                    </v-col>
                  </v-row>
                </v-card>
              </v-tab-item>

              <v-tab-item>
                <v-card color="#323b50" flat class="card_item pa-2">
                  <v-row>
                    <v-col cols="12" sm="3" v-for="(Parke, i) in Parkes" :key="i">
                      <v-hover v-slot="{hover}" close-delay="200">
                        <v-card :elevation="hover ? 16 : 2" :class="{ 'on-hover' :hover }"
                        class="mx-auto" height="250" tile color="#333c51" align="center">
                          <v-card-actions>
                            <v-spacer></v-spacer>
                            <v-btn tile small :color="hover ? '#f34f64' : '#777d8b'" dark>
                              {{ Parke.price }}
                            </v-btn>
                          </v-card-actions>
                          <v-img src="../image/shirt-2.jpg" width="150" height="150"></v-img>
                          <v-card-text :class="hover ? 'red--text' : 'white--text'">
                            {{ Parke.title }}
                          </v-card-text>
                        </v-card> 
                      </v-hover>
                    </v-col>
                  </v-row>
                </v-card>
              </v-tab-item>

              <v-tab-item>
                <v-card color="#323b50" flat class="card_item pa-2">
                  <v-row>
                    <v-col cols="12" sm="3" v-for="(parasut, i) in parasuts" :key="i">
                      <v-hover v-slot="{hover}" close-delay="200">
                        <v-card :elevation="hover ? 16 : 2" :class="{ 'on-hover' :hover }"
                        class="mx-auto" height="250" tile color="#333c51" align="center">
                          <v-card-actions>
                            <v-spacer></v-spacer>
                            <v-btn tile small :color="hover ? '#f34f64' : '#777d8b'" dark>
                              {{ parasut.price }}
                            </v-btn>
                          </v-card-actions>
                          <v-img src="../image/shirt-3.jpg" width="150" height="150"></v-img>
                          <v-card-text :class="hover ? 'red--text' : 'white--text'">
                            {{ parasut.title }}
                          </v-card-text>
                        </v-card> 
                      </v-hover>
                    </v-col>
                  </v-row>
                </v-card>
              </v-tab-item>

              <v-tab-item>
                <v-card color="#323b50" flat class="card_item pa-2">
                  <v-row>
                    <v-col cols="12" sm="3" v-for="(parasut, i) in parasuts" :key="i">
                      <v-hover v-slot="{hover}" close-delay="200">
                        <v-card :elevation="hover ? 16 : 2" :class="{ 'on-hover' :hover }"
                        class="mx-auto" height="250" tile color="#333c51" align="center">
                          <v-card-actions>
                            <v-spacer></v-spacer>
                            <v-btn tile small :color="hover ? '#f34f64' : '#777d8b'" dark>
                              {{ parasut.price }}
                            </v-btn>
                          </v-card-actions>
                          <v-img src="../image/shirt-1.jpg" width="150" height="150"></v-img>
                          <v-card-text :class="hover ? 'red--text' : 'white--text'">
                            {{ parasut.title }}
                          </v-card-text>
                        </v-card> 
                      </v-hover>
                    </v-col>
                  </v-row>
                </v-card>
              </v-tab-item>

            </v-tabs-items>
          </v-col>
          <v-col cols="12" sm="4">
            <PaymentBar />
          </v-col>
        </v-row>
      </v-card>
    </v-container>
  </v-app>
</template>

<script>
import SideBar from "../components/SideBar.vue";
import NavBar from "../components/NavBar.vue";
import PaymentBar from "../components/PaymentBar.vue";

export default {
  name: "HomeView",
  data: () => ({
    tab: null,
    parasuts: [
      {
        avatar: "../image/avatar-05.png",
        price: "$80",
        title: "1 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$80",
        title: "2 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$90",
        title: "3 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$80",
        title: "4 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$85",
        title: "5 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$80",
        title: "6 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$70",
        title: "7 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$100",
        title: "8 Cotton Shirt",
      },
    ],
    Parkes: [
      {
        avatar: "avatar-05.png",
        price: "$80",
        title: "1 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$80",
        title: "2 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$90",
        title: "3 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$80",
        title: "4 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$85",
        title: "5 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$80",
        title: "6 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$70",
        title: "7 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$100",
        title: "8 Cotton Shirt",
      },
    ],
    towParkas: [
      {
        avatar: "avatar-05.png",
        price: "$80",
        title: "1 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$80",
        title: "2 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$90",
        title: "3 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$80",
        title: "4 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$85",
        title: "5 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$80",
        title: "6 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$70",
        title: "7 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$100",
        title: "8 Cotton Shirt",
      },
    ],
    steves: [
      {
        avatar: "avatar-05.png",
        price: "$80",
        title: "1 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$80",
        title: "2 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$90",
        title: "3 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$80",
        title: "4 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$85",
        title: "5 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$80",
        title: "6 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$70",
        title: "7 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$100",
        title: "8 Cotton Shirt",
      },
    ],
    threeParkas: [
      {
        avatar: "avatar-05.png",
        price: "$80",
        title: "1 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$80",
        title: "2 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$90",
        title: "3 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$80",
        title: "4 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$85",
        title: "5 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$80",
        title: "6 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$70",
        title: "7 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$100",
        title: "8 Cotton Shirt",
      },
    ],
    dennise: [
      {
        avatar: "avatar-05.png",
        price: "$80",
        title: "1 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$80",
        title: "2 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$90",
        title: "3 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$80",
        title: "4 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$85",
        title: "5 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$80",
        title: "6 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$70",
        title: "7 Cotton Shirt",
      },
      {
        avatar: "avatar-05.png",
        price: "$100",
        title: "8 Cotton Shirt",
      },
    ],
  }),
  components: {
    SideBar,
    NavBar,
    PaymentBar
  },
};
</script>

<style>

.v-tabs-slider {
  position: absolute;
  top: 30%;
  left: 50%;
  transform: translate(-50%, -50%);
  height: 15px !important;
  width: 20px !important;
  border-radius: 150px 150px 0 0 ;
  background-color: #f34f64;
}
.v-tab.withoutupercase {
  text-transform: none !important;
}
.v-tabs {
  width: 50% !important;
}
.container {
  padding: 0px !important;
}
.v-card.card_global {
 height: 800px !important; 
}

.theme--light.v-card.card-item {
  background-color: #323b50 !important;
  color: #babec9 !important;
}
.v-sheet.v-card.card-item {
  border-radius: 0px !important;
}
.v-btn:not(.v-btn-round).v-size--small {
  width: 50px !important;
}
.v-application .red--text {
  color: #f34f64 !important;
  caret-color: #f34f64 !important;
}
</style>