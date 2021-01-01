<template>
    <v-card :color="bodyColor" class="w-100">
      <v-card-title :class="headColor">
        <h4  class="text-uppercase white--text w-100 text-center text-uppercase " >
          <span v-text="title">Voltage</span>
        </h4>
      </v-card-title>
      <v-card-text class="mt-2">
          <v-row class="row">
             <v-col class="text-number blue--text " >
               <span v-text="value">20</span>
             </v-col>
             <v-col class="text-unit" >
               <span v-text="unit">°C</span>
             </v-col>
          </v-row>
      </v-card-text>
    </v-card>
</template>

<script>
    export default {
        name: "SimpleIndicator",
      props: {
         title:{
           default:"No title",

         },
        unit:{
           default:'W',
        },
        value:{
           default:0.0
        },
        headColor:{
           default:'purple darken-4'
        },
        bodyColor:{
           default:'white'
        }

      }
    }
</script>

<style >
  .text-number{
    font-family:'Digital-7' ;
    font-weight: bold;
    font-size: 72px;
  ;
  }
  .text-unit{
    font-size: 56px;
    font-weight: bold;
    color: green;
  }
</style>
