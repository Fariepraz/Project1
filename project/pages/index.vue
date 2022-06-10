<template>

<div>
  
<Navbar/>


<v-row class=" justify-center mt-10" >
<v-col md="6">
 <v-card
  elevation="12"
  class="grey lighten-2"
>

<v-form>
  <h2 class="indigo darken-4"><center> Registration form</center></h2>
    <v-container>
      <v-row>
        <v-col
          cols="12"
          sm="6"
        >
          <v-text-field
            v-model="first"
            label="First Name"
            filled
          ></v-text-field>
        </v-col>

        <v-col
          cols="12"
          sm="6"
        >
          <v-text-field
            v-model="last"
            label="Last Name"
            filled
          ></v-text-field>
        </v-col>
      </v-row>
       <v-row>
        <v-col
          cols="12"
          sm="6"
        >
          <v-text-field
            v-model="email"
            label="Email Address"
            filled
          ></v-text-field>
        </v-col>

        <v-col
          cols="12"
          sm="6"
        >
          <v-text-field
            v-model="number"
            label="Phone Number"
            filled
          ></v-text-field>
        </v-col>
          <v-col
          cols="12"
          sm="6"
        >
          <v-text-field
            v-model="Age"
            label="Age"
            filled
          ></v-text-field>
        </v-col>
      
        <v-col
          cols="12"
          sm="6"
        >
          <v-text-field
            v-model="Address"
            label="Pysical Address"
            filled
          ></v-text-field>
        </v-col></v-row>
    </v-container>
   <v-btn 
  color="green"
  depressed
  elevation="2"
  tile
>
Register</v-btn> 
    <v-btn
  color="red"
  depressed
  elevation="2"
  tile
>
Cancel</v-btn>
  </v-form>
  
</v-card> 
</v-col>
</v-row>


</div>
  
</template>

<script>
import Navbar from '../components/navbar.vue';
export default {
    name: "IndexPage",
    components: { Navbar }
}
</script>
