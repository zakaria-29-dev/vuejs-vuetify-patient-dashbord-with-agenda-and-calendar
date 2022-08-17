<template>
  <v-app-bar color="white" app dark flat >
    <v-icon color="black">fas fa-long-arrow-alt-left</v-icon>
      <h4 class="black--text ml-3">Patient Card</h4> 
    
    <v-spacer></v-spacer>

      <h4 class="blue--text text--lighten-2">Appointments history</h4>
    

    <v-icon x-small color="#2784FF" class="ml-2 mr-2"
      >fas fa-caret-down</v-icon
    >
    <v-btn color="#2784FF" class="withoutupercase">
        <v-icon left>fas fa-plus</v-icon>
        New Patient
    </v-btn>

<v-badge dot overlap color="green" class="ml-3 mr-2" dark>
    <v-avatar tile color="#E5F1FF">
         <v-icon color="#2784FF">fas fa-bell</v-icon>
    </v-avatar>
     
    </v-badge>

     <v-avatar tile color="#E5F1FF">
        <v-img src="p.png" />
    </v-avatar>

    

   
    
  </v-app-bar>
</template>

<script>
export default {
  data: () => ({}),
};
</script>
<style>
.v-btn.withoutupercase {
  text-transform: none !important;
}</style>