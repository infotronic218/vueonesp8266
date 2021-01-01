<template>
    <div>
        <v-app-bar app color="purple darken-4"  dense>
       <v-toolbar-title>
         <label class="white--text"><strong>Vue On ESP</strong></label>
       </v-toolbar-title>
       <v-spacer></v-spacer>
      <v-toolbar-items primary class="">
        <div class=" py-2 ml-3 desktop-menu">
           <v-btn  active-class="deep-orange darken-3 white--text" to="/" class="mx-1 theme--light" >Dashboard</v-btn>
           <v-btn  active-class="deep-orange white--text"  to="/settings" class="mx-1" >Settings</v-btn>
        </div>

          <div class="py-1 ml-3 mobile-menu">
              <v-menu offset-y auto close-delay="4" min-width="100%">
              <template v-slot:activator="{ on, attrs }">
                   <v-app-bar-nav-icon v-bind="attrs" v-on="on" ></v-app-bar-nav-icon>
              </template>

                          <div class="d-flex flex-column ma-2">
                               <v-btn active-class="deep-orange" :to="{name:'Settings'}" class="ma-1" color="deep-orange darken-1">Settings</v-btn>
                                <v-btn exact-active-class="deep-orange" :to="{name:'Measurements'}" class="ma-1" color="deep-orange darken-1">Measurements</v-btn>
                                <v-btn exact-active-class="deep-orange" :to="{name:'Relays'}" class="ma-1" color="deep-orange darken-1">Relays</v-btn>
                          </div>

              </v-menu>
          </div>
      </v-toolbar-items>

    </v-app-bar>
    </div>
</template>

<script>
    export default {
        name: "Navigation"
    }
</script>
<style>
    @media only screen and (max-width: 600px) {
       .desktop-menu{
           display: none;
        }
    }
    @media only screen and (min-width: 600px) {

        .mobile-menu{
           display: none;
       }

    }
</style>

