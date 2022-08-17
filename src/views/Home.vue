<template>
  <v-app
    id="inspire"
    :style="{ background: $vuetify.theme.themes.dark.background }"
  >
    <SideBar />
    <Navbar />
    <v-container>
      <v-row>
        <v-col cols="12" sm="9">
          <v-row>
            <v-col cols="12" sm="12">
              <Contact />
            </v-col>
            <v-col cols="12" sm="12">
            <Agenda />
            </v-col>
          </v-row>
        </v-col>
        <v-col cols="12" sm="3">
            <Doctor />
        </v-col>
      </v-row>
    </v-container>
  </v-app>
</template>

<script>
// @ is an alias to /src
import SideBar from "@/components/SideBar.vue";
import Navbar from "../components/Navbar.vue";
import Contact from "../components/Contact.vue";
import Agenda from "../components/Agenda.vue";
import Doctor from "../components/Doctor.vue";

export default {
  data: () => ({
    
  }),
 

  components: {
    SideBar,
    Navbar,
    Contact,
    Agenda,
    Doctor
},
};
</script>
