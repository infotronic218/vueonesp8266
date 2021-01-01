<template>
  <div class="home">
     <v-row class="text-center">
            <v-col cols="12" md="12" class="text-center">

                    <h2 class="text-center text-uppercase">Analog Inputs</h2>

            </v-col>
            <v-col md="3" cols="12" class="m-2">
                <div class="mx-2">
                   <simple-indicator headColor="blue-grey darken-2" unit="V" title="Analog 0 (A0)" ></simple-indicator>
                </div>
            </v-col>
            <v-col md="3" cols="12" class="m-2">
                <div class="mx-2">
                     <simple-indicator headColor="deep-purple lighten-1" unit="V" title="Analog 1 (A1)"></simple-indicator>
                </div>
            </v-col><v-col md="3" cols="12" class="m-2">
                 <div class="mx-2">
                    <simple-indicator headColor="pink accent-4" unit="V" title="Analog 2 (A2)"></simple-indicator>
                 </div>
            </v-col>
            <v-col md="3" cols="12" class="m-2">
                <div class="mx-2">
                   <simple-indicator headColor="pink darken-4" unit="V" title="Analog 3 (A3)"></simple-indicator>
                </div>
            </v-col>

        </v-row>
    <v-row>
            <v-col cols="12" md="12">

                    <h2 class="text-uppercase text-center">Relays</h2>

            </v-col>
            <v-col cols="12" md="3">
                <simple-switch title="Relay 1"></simple-switch>
            </v-col>
            <v-col cols="12" md="3">
                <simple-switch title="Relay 2"></simple-switch>
            </v-col>
            <v-col cols="12" md="3">
                <simple-switch title="Relay 3"></simple-switch>
            </v-col>
            <v-col cols="12" md="3">
                <simple-switch title="Relay 4"></simple-switch>
            </v-col>
        </v-row>
      <v-row  class="mt-3 align-content-center justify-center text-center">
          <v-col cols="12">
              <v-btn rounded color="green" class="white--text">Connect</v-btn>
          </v-col>
      </v-row>
  </div>

</template>

<script>


import SimpleIndicator from "../components/Indicator";
import SimpleSwitch from "../components/SimpleSwitch";
export default {
  name: 'Home',
  components: {
    SimpleSwitch,
    SimpleIndicator

  }
}
</script>
