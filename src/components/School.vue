<template>
<v-container fluid>
  <v-row dense justify="space-between">
    <v-col v-for="i in 5" :key="i" cols="2">
      <v-card flat hover>
        <v-img
          class="white--text align-center"
          height="200px"
          src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"
        >
          <p>Top 10 Australian beaches</p>
            <v-card-subtitle class="pb-0">Number 10</v-card-subtitle>

        <v-card-text class="text--primary">
          <div>Whitehaven Beach</div>

          <div>Whitsunday Island, Whitsunday Islands</div>
        </v-card-text>

        <v-card-actions>
          <v-btn
            color="orange"
            text
          >
            Share
          </v-btn>

          <v-btn
            color="orange"
            text
          >
            Explore
          </v-btn>
        </v-card-actions>
        </v-img>
      </v-card>
    </v-col>
    <v-col cols="2" class="my-auto">
      <v-card flat hover class="ml-5 d-inline-block">
        <v-img
          class="white--text align-center"
          width="100"
          src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"
        >
          <v-card-text class="white--text headline  font-weight-bold">
            <p>
              More
            </p>
            <v-icon
              color="white"
              class=""
              justify-center
              large
            >
              mdi-chevron-double-right
            </v-icon>
          </v-card-text>
        </v-img>
      </v-card>
    </v-col>
  </v-row>
</v-container>
</template>
