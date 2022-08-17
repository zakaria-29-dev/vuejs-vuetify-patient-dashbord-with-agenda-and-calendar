<template>
   <v-card color="white" class="rounded-lg mt-2" flat>
            <v-row justify="center" class="pt-2">
              <v-date-picker
                v-model="picker"
                color="#2784FF"
                width="260"
              ></v-date-picker>
            </v-row>

            <v-toolbar color="transparent" flat class="mt-4">
              <h4 class="black--text">Doctors</h4>
              <v-spacer></v-spacer>
              <v-avatar tile color="#ECF5FF">
                <v-icon color="#2784FF">fas fa-angle-up</v-icon>
              </v-avatar>
            </v-toolbar>
            <v-list class="mt-n6" color="transparent" dense>
              <v-list-item v-for="chat in chats" :key="chat.title">
                <v-list-item-avatar tile>
                  <v-img :src="chat.img" />
                </v-list-item-avatar>
                <v-list-item-content>
                  <v-list-item-title
                    v-text="chat.title"
                    class="black--text"
                  ></v-list-item-title>
                  <v-list-item-subtitle
                    v-text="chat.subtitle"
                    class="grey--text"
                  ></v-list-item-subtitle>
                </v-list-item-content>
              </v-list-item>
            </v-list>
          </v-card>
</template>

<script>
export default {
data: () => ({
    chats: [
      {
        img: "p2.jpg",
        subtitle: "Therapist",
        title: "Dr.Clarence Hamilton",
      },
      {
        img: "p5.jpg",
        subtitle: "Surgeon ",
        title: "Dr.Brett Hoffman",
      },
      {
        img: "p4.jpg",
        subtitle: "Hematologist ",
        title: "Dr.Miguel Leonard",
      },
    ],
    picker: new Date(Date.now() - new Date().getTimezoneOffset() * 60000)
      .toISOString()
      .substr(0, 10),
   
})
}
</script>

<style>

</style>