<template>
  <v-app>
    <NavBar />
    <PopupView
      :laptops="dataPopup"
      v-if="isShowPopup"
      @Close="isShowPopup = false"
    />
    <v-container fluid>
      <v-card
        color="#F7F7F7"
        height="180px"
        tile
        flat
        class="d-flex align-center justify-center mt-12"
        dark
      >
        <v-col cols="12" sm="12">
          <v-item-group mandatory class="mt-n1">
            <v-container>
              <v-row justify="center" class="space">
                <v-col cols="12" xs="12" md="2" ms="2">
                  <v-item v-slot="{ active }">
                    <v-card
                      :color="active ? '#D5F0DB' : 'white'"
                      :class="active ? 'borderme' : 'borderout'"
                      class="d-flex-algin-center rounded-lg mx-2 pa-5"
                      dark
                      height="170"
                      @click="() => handleCardClick('FPT SHOP')"
                      flat
                    >
                      <v-row>
                        <v-col cols="12" sm="12">
                          <v-list-item
                            three-line
                            class="text-center align-center justify-center pa-0"
                          >
                            <v-list-item-content>
                              <div
                                align="center"
                                justify="center"
                                class="mt-5"
                                style="height: 70px"
                              >
                                <v-img
                                  src="../../public/fpt1.png"
                                  max-height="80"
                                  max-width="80"
                                  contain
                                />
                              </div>
                              <v-list-item-subtitle
                                :class="active ? 'green--text' : 'black--text'"
                                class="caption mt-5"
                              >
                                FPT SHOP
                              </v-list-item-subtitle>
                            </v-list-item-content>
                          </v-list-item>
                        </v-col>
                      </v-row>
                    </v-card>
                  </v-item>
                </v-col>
                <v-col cols="12" xs="12" md="2" ms="2">
                  <v-item v-slot="{ active }">
                    <v-card
                      :color="active ? '#D5F0DB' : 'white'"
                      :class="active ? 'borderme' : 'borderout'"
                      class="d-flex-algin-center rounded-lg mx-2 pa-5"
                      dark
                      height="170"
                      @click="() => handleCardClick('Thế Giới Di Động')"
                      flat
                    >
                      <v-row>
                        <v-col cols="12" sm="12">
                          <v-list-item
                            three-line
                            class="text-center align-center justify-center pa-0"
                          >
                            <v-list-item-content>
                              <div
                                align="center"
                                justify="center"
                                class="mt-5"
                                style="height: 70px"
                              >
                                <v-img
                                  src="../../public/tgdd.png"
                                  max-height="80"
                                  max-width="80"
                                  contain
                                />
                              </div>
                              <v-list-item-subtitle
                                :class="active ? 'green--text' : 'black--text'"
                                class="caption mt-5"
                              >
                                Thế Giới Di Động
                              </v-list-item-subtitle>
                            </v-list-item-content>
                          </v-list-item>
                        </v-col>
                      </v-row>
                    </v-card>
                  </v-item>
                </v-col>
                <v-col cols="12" xs="12" md="2" ms="2">
                  <v-item v-slot="{ active }">
                    <v-card
                      :color="active ? '#D5F0DB' : 'white'"
                      :class="active ? 'borderme' : 'borderout'"
                      class="d-flex-algin-center rounded-lg mx-2 pa-5"
                      dark
                      height="170"
                      @click="() => handleCardClick('Phong Vũ')"
                      flat
                    >
                      <v-row>
                        <v-col cols="12" sm="12">
                          <v-list-item
                            three-line
                            class="text-center align-center justify-center pa-0"
                          >
                            <v-list-item-content>
                              <div
                                align="center"
                                justify="center"
                                class="mt-5"
                                style="height: 70px"
                              >
                                <v-img
                                  src="../../public/phongvu.png"
                                  max-height="80"
                                  max-width="80"
                                  contain
                                />
                              </div>
                              <v-list-item-subtitle
                                :class="active ? 'green--text' : 'black--text'"
                                class="caption mt-5"
                              >
                                Phong Vũ
                              </v-list-item-subtitle>
                            </v-list-item-content>
                          </v-list-item>
                        </v-col>
                      </v-row>
                    </v-card>
                  </v-item>
                </v-col>
                <v-col cols="12" xs="12" md="2" ms="2">
                  <v-item v-slot="{ active }">
                    <v-card
                      :color="active ? '#D5F0DB' : 'white'"
                      :class="active ? 'borderme' : 'borderout'"
                      class="d-flex-algin-center rounded-lg mx-2 pa-5"
                      dark
                      height="170"
                      @click="() => handleCardClick('HACOM')"
                      flat
                    >
                      <v-row>
                        <v-col cols="12" sm="12">
                          <v-list-item
                            three-line
                            class="text-center align-center justify-center pa-0"
                          >
                            <v-list-item-content>
                              <div
                                align="center"
                                justify="center"
                                class="mt-5"
                                style="height: 70px"
                              >
                                <v-img
                                  src="../../public/hacom.png"
                                  max-height="80"
                                  max-width="80"
                                  contain
                                />
                              </div>
                              <v-list-item-subtitle
                                :class="active ? 'green--text' : 'black--text'"
                                class="caption mt-5"
                              >
                                HACOM
                              </v-list-item-subtitle>
                            </v-list-item-content>
                          </v-list-item>
                        </v-col>
                      </v-row>
                    </v-card>
                  </v-item>
                </v-col>
                <v-col cols="12" xs="12" md="2" ms="2">
                  <v-item v-slot="{ active }">
                    <v-card
                      :color="active ? '#D5F0DB' : 'white'"
                      :class="active ? 'borderme' : 'borderout'"
                      class="d-flex-algin-center rounded-lg mx-2 pa-5"
                      dark
                      height="170"
                      @click="() => handleCardClick('Phúc Anh')"
                      flat
                    >
                      <v-row>
                        <v-col cols="12" sm="12">
                          <v-list-item
                            three-line
                            class="text-center align-center justify-center pa-0"
                          >
                            <v-list-item-content>
                              <div
                                align="center"
                                justify="center"
                                class="mt-5"
                                style="height: 70px"
                              >
                                <v-img
                                  src="../../public/phucanh.png"
                                  max-height="80"
                                  max-width="80"
                                  contain
                                />
                              </div>
                              <v-list-item-subtitle
                                :class="active ? 'green--text' : 'black--text'"
                                class="caption mt-5"
                              >
                                Phúc Anh
                              </v-list-item-subtitle>
                            </v-list-item-content>
                          </v-list-item>
                        </v-col>
                      </v-row>
                    </v-card>
                  </v-item>
                </v-col>
              </v-row>
            </v-container>
          </v-item-group>
        </v-col>
      </v-card>

      <v-divider></v-divider>
      <v-toolbar color="transparent">
        <v-toolbar-title>Danh sách Laptop</v-toolbar-title>
        <v-spacer></v-spacer>
        <v-text-field
          density="compact"
          variant="outlined"
          label="Search"
          append-inner-icon="fas fa-search"
          single-line
          hide-details
          class="mr-2"
          v-model="searchKeyword"
        ></v-text-field>
      </v-toolbar>
      <v-row class="ma-5">
        <v-col
          @click="handleDataPopup(laptop)"
          cols="12"
          sm="3"
          align="center"
          justify="center"
          v-for="(laptop, i) in laptops"
          :key="i"
        >
          <v-card align="center" tile>
            <v-img :src="laptop.ImageLink" width="200" height="200" contain>
            </v-img>
            <v-card-text class="mt-n1" style="height: 50px">
              <strong>{{ laptop.Name }}</strong>
            </v-card-text>
            <v-card-text class="">
              <button
                class="pa-2 rounded"
                style="background-color: #cb1c22; color: white"
              >
                <strong>{{ laptop.Price }}</strong>
              </button>
            </v-card-text>
            <v-card-text class="ma-2" style="background-color: #f8f9fa">
              <div class="ml-2">
                <v-row style="color: #6c757d">{{
                  "Brand: " + laptop.Brand
                }}</v-row>
                <v-row style="color: #6c757d">{{ "CPU: " + laptop.CPU }}</v-row>
                <v-row style="color: #6c757d">{{
                  "Storage: " + laptop.Storage
                }}</v-row>
                <v-row style="color: #6c757d">{{
                  "Weight: " + laptop.Weight
                }}</v-row>
              </div>
            </v-card-text>
            <v-row>
              <v-col
                ><v-btn
                  class="ma-4"
                  style="background-color: #cb1c22; color: white"
                >
                  <strong>Mua ngay</strong></v-btn
                ></v-col
              >
              <v-col
                ><v-btn
                  class="ma-4"
                  style="background-color: #99a2aa; color: white"
                >
                  <strong>So sánh</strong></v-btn
                ></v-col
              >
            </v-row>
          </v-card>
        </v-col>
      </v-row>
      <v-divider></v-divider>
      <v-toolbar color="transparent">
        <!-- <v-toolbar-title class="text-caption">
          Show more laptop</v-toolbar-title> -->
        <v-spacer></v-spacer>
        <v-btn rounded @click="leftButton">
          <v-icon color="grey">fas fa-long-arrow-alt-left</v-icon>
        </v-btn>

        <span class="text-caption"></span>
        <v-btn rounded @click="rightButton"
          ><v-icon color="grey">fas fa-long-arrow-alt-right</v-icon></v-btn
        >
        <v-spacer></v-spacer>
      </v-toolbar>
    </v-container>
    <FooterView />
  </v-app>
</template>

<script>
import { defineComponent } from "vue";

import NavBar from "@/components/NavBar.vue";
import FooterView from "@/components/FooterView.vue";
import PopupView from "@/components/PopupView.vue";
// import axios from "axios";
export default defineComponent({
  name: "HomeView",
  components: {
    NavBar,
    FooterView,
    PopupView,
  },
  data() {
    return {
      laptop: true,
      other: false,
      slider2: 50,
      categories: [
        { imgLink: "../../public/fpt1.png", title: "FPT SHOP" },
        { imgLink: "../../public/tgdd.png", title: "Thế Giới Di Động" },
        { imgLink: "../../public/phongvu.png", title: "Phong Vũ" },
        { imgLink: "../../public/hacom.png", title: "HACOM" },
        { imgLink: "../../public/phucanh.png", title: "Phúc Anh" },
      ],
      laptops: [],
      dataPopup: [],
      isShowPopup: false,
      data: [],
      pageNumber: 1,
      checkFilter: "",
      searchKeyword: "",
    };
  },
  created() {
    this.checkFilter = "";
  },
  mounted() {
    this.fetchData();
  },
  methods: {
    async fetchData() {
      let fullUrl = `http://localhost:3000/laptops?page=${this.pageNumber}`;
      const response = await fetch(fullUrl);
      this.laptops = await response.json();
    },
    async fetchDataFilter(title) {
      let fullUrl = `http://localhost:3000/laptops/filter?source=${title}&pageNumber=${this.pageNumber}`;
      const response = await fetch(fullUrl);
      this.laptops = await response.json();
    },
    async handleCardClick(title) {
      this.pageNumber = 1;
      if (title == "FPT SHOP") {
        this.checkFilter = "fptshop";
        this.fetchDataFilter(this.checkFilter);
      }
      if (title == "Thế Giới Di Động") {
        this.checkFilter = "tgdd";
        this.fetchDataFilter(this.checkFilter);
      }
      if (title == "Phong Vũ") {
        this.checkFilter = "phongvu";
        this.fetchDataFilter(this.checkFilter);
      }
      if (title == "HACOM") {
        this.checkFilter = "hanoicomputer";
        this.fetchDataFilter(this.checkFilter);
      }
      if (title == "Phúc Anh") {
        this.checkFilter = "phucanh";
        this.fetchDataFilter(this.checkFilter);
      }
      console.log(this.laptops);
    },
    handleDataPopup(laptop) {
      this.dataPopup = laptop.matching;
      this.isShowPopup = true;
    },
    leftButton() {
      if (this.pageNumber > 1) {
        this.pageNumber--;
      } else {
        this.pageNumber = 1;
      }

      this.fetchData();
    },
    rightButton() {
      this.pageNumber++;

      this.fetchData();
    },
  },
  watch: {
    pageNumber: {
      handler: function (newValue) {
        if (newValue) {
          this.$router.push({ name: "home", params: { id: newValue } });
        }
      },
    },
    searchKeyword: {
      handler: function (newValue) {
        if (newValue) {
          setTimeout(async () => {
            let fullUrl = `http://localhost:3000/laptops/search?name=${newValue}&pageNumber=1`;
            const response = await fetch(fullUrl);
            this.laptops = await response.json();
          }, 500);
        }
      },
    },
    
  },
});
</script>
<style scoped>
.v-container {
  width: 100%;
  padding: 16px 0px o !important;
  margin-right: auto;
  margin-left: auto;
}

.v-card.borderme {
  border: 2px solid black !important;
}

.v-card.borderout {
  border: 1px solid #d5f0db !important;
}
</style>
