<template>
  <v-card
    :href="value.href"
    :width="small ? 150 : 175"
    flat
    tile
    color="transparent"
    class="d-inline-flex mx-2"
    target="_blank"
    rel="noopener"
  >
    <div>
      <v-img
        :class="value.dark ? 'black' : ''"
        :height="small ? 40 : 70"
        :src="`https://cdn.vuetifyjs.com/images/${value.logo}`"
        class="mb-3"
        contain
      />
    </div>
  </v-card>
</template>

<script>
  export default {
    props: {
      small: {
        type: Boolean,
        default: false
      },
      value: {
        type: Object,
        required: true
      }
    }
  }
</script>
