<template>

  <v-container style="padding-top: 60px;">
    <v-row dense>
      <v-col cols="12">
        <p class="text-center font-weight-black text-h5">Our Staff</p>
        <p class="text-center text-grey">Meet our professional and passionate staff</p>
      </v-col>
    </v-row>
    <v-row>
      <v-col cols="12" sm="4" v-for="(person,index) in staff" :key="index">
        <v-card color="blue" variant="flat" style="border:1px solid #2196F3">
          <v-card-text class="text-center">
            <v-icon size="70">mdi-account-circle-outline</v-icon>
            <p class="text-center text-h5 font-weight-black">{{person.name}}</p>
          </v-card-text>
          <v-card-text class="bg-white">
            <v-list-item>
              <v-list-item-title>{{person.qualification}}</v-list-item-title>
            <v-list-item-subtitle class="text-grey">Position</v-list-item-subtitle>
            </v-list-item>

            <v-list-item>
              <v-list-item-title>{{person.email}}</v-list-item-title>
            <v-list-item-subtitle class="text-grey">email</v-list-item-subtitle>
            </v-list-item>

            <v-list-item>
              <v-list-item-title>{{person.phone}}</v-list-item-title>
            <v-list-item-subtitle class="text-grey">Phone Number</v-list-item-subtitle>
            </v-list-item>

            <v-list-item>
              <v-list-item-title>{{person.location}}</v-list-item-title>
            <v-list-item-subtitle class="text-grey">Location</v-list-item-subtitle>
            </v-list-item>

          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
  </v-container>

</template>

<script lang="ts">
import {defineComponent} from 'vue'

export default defineComponent({
  name: "staff",
  data() {
    return {
      staff: [

        {
          name: "Rania",
          qualification: "Founder & CEO",
          phone: "(708)-665-6000",
          email: "rania@myatsii.com",
          location: "Orland Park"
        },

        {
          name: "Sam",
          qualification: "Chief Operation Officer (COO)",
          phone: "(708)-665-6000",
          email: "sam@myatsii.com",
          location: "Orland Park"
        },
        {
          name: "Sara",
          qualification: "Accounting Specialist",
          phone: "(708)-665-6000",
          email: "sara@myatsii.com",
          location: "Orland Park"
        },
        {
          name: "Fatima",
          qualification: "Accounting Specialist",
          phone: "(708)-665-6000",
          email: "fatima@myatsii.com",
          location: "Orland Park"
        },
        {
          name: "Rufida",
          qualification: "Accounting Specialist",
          phone: "(708)-665-6000",
          email: "rufida@myatsii.com",
          location: "Orland Park"
        }
        ,
        {
          name: "Loubna",
          qualification: "Tax Specialist",
          phone: "(708)-665-6000",
          email: "tax@myatsii.com",
          location: "Orland Park"
        }

      ]
    }
  }
})
</script>


<style scoped>

</style>