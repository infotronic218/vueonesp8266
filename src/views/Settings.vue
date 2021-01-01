<template>
  <v-container>
    <v-row justify="center" align-content="center" align-content-md="center" class="text-center">
      <v-col md="12" cols="12">
        <h2 class="text-center text-uppercase">Settings</h2>
      </v-col>
      <v-col cols="12" md="4" class="text-center ">
        <div class="text-center">
        <v-card>
          <v-card-text>
            <v-card-title  class="justify-center text-center ">
              <h4 class="d-inline text-uppercase">Connection info</h4>
            </v-card-title>
            <v-text-field name="ip" label="IP Address" placeholder="IP Address">
            </v-text-field>

            <v-text-field name="ip2" label="IP Address" placeholder="IP Address">
            </v-text-field>
          </v-card-text>
          <v-btn color="primary" class="mb-3">Save</v-btn>
        </v-card>
        </div>
      </v-col>

    </v-row>
  </v-container>
</template>

