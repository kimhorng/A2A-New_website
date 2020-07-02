<template>
  <v-card width="250" flat class="blue-grey lighten-5">
    <v-file-input
      v-model="files"
      color="red darken-3"
      counter
      label="File input"
      multiple
      placeholder="Attach Resume/ CV "
      prepend-icon="mdi-paperclip"
      outlined
      :show-size="1000"
    >
      <template v-slot:selection="{ index, text }">
        <v-chip v-if="index < 2" color="red" dark label small>
          {{ text }}
        </v-chip>

        <span
          v-else-if="index === 2"
          class="overline grey--text text--darken-3 mx-2"
        >
          +{{ files.length - 2 }} File(s)
        </span>
      </template>
    </v-file-input>
  </v-card>
</template>
