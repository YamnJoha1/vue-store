<template>
  <v-app-bar app dark color="#323b50" flat>
    <v-tabs color="#c">
      <v-tabs-slider color="#f34f64"></v-tabs-slider>
      <v-tab class="withoutupercase">Shirt</v-tab>
      <v-tab class="withoutupercase">Shoes</v-tab>
      <v-tab class="withoutupercase">Jacket</v-tab>
      <v-tab class="withoutupercase">Hats</v-tab>
      <v-tab class="withoutupercase">Trousers</v-tab>
    </v-tabs>
    <v-btn small color="#f34f64">
      <v-icon>mdi-chevron-down</v-icon>
    </v-btn>
    <v-spacer></v-spacer>
    <v-divider vertical inset class="mr-8"></v-divider>
    <v-text-field label="Search" prepend-inner-icon="mdi-magnify" dense class="mt-4 pr-8" ></v-text-field>
    <v-btn text small class="withoutupercase grey--text ml-4 mr-4 mt-2">
      Hi,Yamn Jo
      <v-icon small>mdi-chevron-down</v-icon>
    </v-btn>
  </v-app-bar>
</template>

<script>
export default {
  data: () => ({
    links: [
      'Dashboard',
      'Message',
      'Profile',
      'Updates'
    ],
    items: [
      { icon: "mdi-laptop" },
      { icon: "mdi-tag-outline" },
      { icon: "mdi-shopping-outline" },
      { icon: "mdi-wallet-travel" },
      { icon: "mdi-apps" },
      { icon: "mdi-text-box-multiple-outline" },
    ]
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
  border-radius: 150px 150px 0 0 ;
  background-color: #f34f64;
}
.v-tab.withoutupercase {
  text-transform: none !important;
}
.v-tabs {
  width: 30% !important;
}
.v-btn:not(.v-btn--round).v-size-small {
  min-width: 10px !important;
  padding: 0 5px !important;
}
.theme--dark.v-text-field > .v-input_control > .v-input_slot::before{
  border-color: #323b50 !important ;
}
</style>