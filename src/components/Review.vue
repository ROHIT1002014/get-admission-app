<template>
  <v-container fluid style="background-color:yellow">
    <v-row justify="center">
      <v-col cols="8">
        <v-card elevation="5" class="pa-5">
          <h1>Review: </h1>
          <v-textarea clearable height="200" background-color="grey lighten-3" outlined />
          <v-card-actions>
            <v-btn class="primary" text>Submit</v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>