<template>
<div id="app">
  <v-app id="inspire">
    <v-card class="mt-16 pt-16" >

      <v-sheet
        id="scrolling-techniques-2"
        class="overflow-y-auto"
        max-height="600"
      >
        <v-container style="height: 1000px;">
          <v-card
      class="mx-auto"
      max-width="100%"
      tile
    >
        Welcome to the homepage for Aroundabouts Laundry , Cornwall.<br>
        <v-list flat width="600" left>
        <v-subheader>Are you looking for :</v-subheader>
        <v-list-item-group
          v-model="selectedItem"
          color="primary"
        >
          <v-list-item
            v-for="(item, i) in items"
            :key="i"
          >
            <v-list-item-icon>
              <v-icon v-text="item.icon"></v-icon>
            </v-list-item-icon>
            <v-list-item-content>
              <v-list-item-title v-text="item.text"></v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-list-item-group>
      </v-list>
         <br>
</v-card>
        </v-container>
      </v-sheet>
    </v-card>
  </v-app>
</div>
</template>

<script>
import { mdiWashingMachine } from '@mdi/js';

export default {
  name: 'Home',
  data: () => ({
    items: [
      { text: 'A Cornish Laundry company based in the heart of Cornwall.', icon: mdiWashingMachine },
      { text: 'Linen and Laundry in Cornwall.', icon: mdiWashingMachine },
      { text: 'Domestic and Commercial Cleaning in Cornwall', icon: mdiWashingMachine },
    ],
  }),
}
</script>
