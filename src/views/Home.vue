<template>
  <v-container fluid>
    <v-layout wrap>
      <v-flex xs2>
        <v-card>
          <v-container>
            <v-layout>
              <v-flex xs12>
                <v-select v-model="selectItem" :items="items"></v-select>
              </v-flex>
            </v-layout>
          </v-container>
        </v-card>
      </v-flex>
    </v-layout>
    <v-layout>
      <v-flex xs8>
        <v-card raised>
          <v-container>
            <v-layout>
              <v-flex xs12>
                <v-calendar></v-calendar>
              </v-flex>
            </v-layout>
          </v-container>
        </v-card>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  data: () => ({
    items: ["user1", "user2", "user3", "user4", "user5"],
    selectItem: []
  })
};
</script>
