<template>
  <v-card flat class="card_item pa-2 mt-2" elevation="2">
    <v-list subheader two-line color="transparent">
      <v-list-item>
        <v-list-item-avatar size="50px">
          <v-icon class="blue-grey darkent-2" color="#737e97">
            mdi-account-outline
          </v-icon>
        </v-list-item-avatar>
        <v-list-item-content>
          <v-list-item-title class="white--text">Unknown Customer</v-list-item-title>
          <v-list-item-subtitle class="grey--text mt-2">Tab here to add Customer</v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>
    </v-list>
    <v-tabs color="#f34f64" v-model="tab1" background-color="transparent" class="order" dark grow>
      <v-tabs-slider color="#f34f64"></v-tabs-slider>
      <v-tab class="withoutupercase">Current Order</v-tab>
      <v-tab class="withoutupercase">Order on Hold</v-tab>
    </v-tabs>
    <v-divider color="#3f495e" class="divider_tab"></v-divider>
    <v-tabs-items v-model="tab1">
      <v-tab-item>
        <v-list subheader two-line color="#323b50">
          <v-list-item>
            <v-list-item-content>
              <v-list-item-title class="white--text subtitle-2 text-center">Brown Casual Shose</v-list-item-title>
              <v-list-item-subtitle class="grey--text mt-2 text-center">Shose</v-list-item-subtitle>
            </v-list-item-content>
            <v-list-item-content>
              <v-list-item-subtitle class="grey--text ml-10">1</v-list-item-subtitle>
            </v-list-item-content>
            <v-list-item-action>
              <v-list-item-title class="white--text subtitle-2 mr-2">$87</v-list-item-title>
            </v-list-item-action>
          </v-list-item>
          <v-divider color="#3f495e" class="divider_tab"></v-divider>
          <v-list-item>
            <v-list-item-content>
              <v-list-item-title class="white--text subtitle-2 text-center">Hoodie kece</v-list-item-title>
              <v-list-item-subtitle class="grey--text mt-2 text-center">Jacket</v-list-item-subtitle>
            </v-list-item-content>
            <v-list-item-content>
              <v-list-item-subtitle class="grey--text ml-10">2</v-list-item-subtitle>
            </v-list-item-content>
            <v-list-item-action>
              <v-list-item-title class="white--text subtitle-2 mr-2">$187</v-list-item-title>
            </v-list-item-action>
          </v-list-item>
          <v-divider color="#3f495e" class="divider_tab"></v-divider>
          <v-list-item>
            <v-list-item-content>
              <v-list-item-title class="white--text subtitle-2 text-center">Brown Casual Shose</v-list-item-title>
              <v-list-item-subtitle class="grey--text mt-2 text-center">Shose</v-list-item-subtitle>
            </v-list-item-content>
            <v-list-item-content>
              <v-list-item-subtitle class="grey--text ml-10">3</v-list-item-subtitle>
            </v-list-item-content>
            <v-list-item-action>
              <v-list-item-title class="white--text subtitle-2 mr-2">$87</v-list-item-title>
            </v-list-item-action>
          </v-list-item>
          <v-divider color="#3f495e" class="divider_tab"></v-divider>
          <v-list-item>

            <v-list-item-content>
              <v-list-item-title class="grey--text">Discount</v-list-item-title>
              <v-list-item-subtitle class="white--text subtitle mt-2 ">Total</v-list-item-subtitle>
            </v-list-item-content>

            <v-list-item-content>
              <v-list-item-subtitle class="orange--text">-4$</v-list-item-subtitle>
            </v-list-item-content>
            <v-list-item-action>
              <v-list-item-title class="green--text subtitle-2 mr-2">$287</v-list-item-title>
            </v-list-item-action>
          </v-list-item>
          <v-divider color="#3f495e" class="divider_tab"></v-divider>
          <div class="text-center mt-6 mb-6">
            <v-btn text color="#f34f64" class="withoutupercase">Delete</v-btn>
            <v-btn  color="#f34f64" dark rounded class="withoutupercase">Checkout</v-btn>
          </div>
        </v-list>
      </v-tab-item>
      <v-tab-item>
        <v-list subheader two-line color="#323b50">
          <v-list-item>
            <v-list-item-content>
              <v-list-item-title class="white--text subtitle-2 text-center">Brown Casual Shose</v-list-item-title>
              <v-list-item-subtitle class="grey--text mt-2 text-center">Shose</v-list-item-subtitle>
            </v-list-item-content>
            <v-list-item-content>
              <v-list-item-subtitle class="grey--text ml-10">1</v-list-item-subtitle>
            </v-list-item-content>
            <v-list-item-action>
              <v-list-item-title class="white--text subtitle-2 mr-2">$87</v-list-item-title>
            </v-list-item-action>
          </v-list-item>
          <v-divider color="#3f495e" class="divider_tab"></v-divider>
          <v-list-item>
            <v-list-item-content>
              <v-list-item-title class="white--text subtitle-2 text-center">Hoodie kece</v-list-item-title>
              <v-list-item-subtitle class="grey--text mt-2 text-center">Jacket</v-list-item-subtitle>
            </v-list-item-content>
            <v-list-item-content>
              <v-list-item-subtitle class="grey--text ml-10">2</v-list-item-subtitle>
            </v-list-item-content>
            <v-list-item-action>
              <v-list-item-title class="white--text subtitle-2 mr-2">$187</v-list-item-title>
            </v-list-item-action>
          </v-list-item>
          <v-divider color="#3f495e" class="divider_tab"></v-divider>
          <v-list-item>
            <v-list-item-content>
              <v-list-item-title class="white--text subtitle-2 text-center">Brown Casual Shose</v-list-item-title>
              <v-list-item-subtitle class="grey--text mt-2 text-center">Shose</v-list-item-subtitle>
            </v-list-item-content>
            <v-list-item-content>
              <v-list-item-subtitle class="grey--text ml-10">3</v-list-item-subtitle>
            </v-list-item-content>
            <v-list-item-action>
              <v-list-item-title class="white--text subtitle-2 mr-2">$87</v-list-item-title>
            </v-list-item-action>
          </v-list-item>
          <v-divider color="#3f495e" class="divider_tab"></v-divider>
          <v-list-item>

            <v-list-item-content>
              <v-list-item-title class="grey--text">Discount</v-list-item-title>
              <v-list-item-subtitle class="white--text subtitle mt-2 ">Total</v-list-item-subtitle>
            </v-list-item-content>

            <v-list-item-content>
              <v-list-item-subtitle class="orange--text">-4$</v-list-item-subtitle>
            </v-list-item-content>
            <v-list-item-action>
              <v-list-item-title class="green--text subtitle-2 mr-2">$287</v-list-item-title>
            </v-list-item-action>
          </v-list-item>
          <v-divider color="#3f495e" class="divider_tab"></v-divider>
          <div class="text-center mt-6 mb-6">
            <v-btn text color="#f34f64" class="withoutupercase">Delete</v-btn>
            <v-btn  color="#f34f64" dark rounded class="withoutupercase">Checkout</v-btn>
          </div>
        </v-list>
      </v-tab-item>
    </v-tabs-items>
  </v-card>
</template>

<script>
export default {
  data: () => ({
    tab1: null
  })
}
</script>

<style>
.v-tabs-slider {
  position: absolute;
  top: 30%;
  left: 50%;
  transform: translate(-50%, -50%);
  height: 15px !important;
  width: 20px !important;
  border-radius: 150px 150px 0 0;
  background-color: #f34f64;
}
.v-tab.withoutupercase ,
.v-btn.withoutupercase {
  text-transform: none !important;
}
.v-tabs {
  width: 50% !important;
}
.v-tabs.order { 
  width: 100% !important;
}
.theme--light.v-card.card_item {
  background-color: #323b50;
  color: #babec9;
}
.v-sheet.v-card.card_item {
  border-radius: 0 !important;
}
.v-divider.divider_tab {
  height: 2px !important;
  max-height: 2px !important;
}

</style>