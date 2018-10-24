<template>
  <v-container
    fluid
    pa-0
  >
    <one-time />

    <patreon-sub />

    <patrons />
  </v-container>
</template>

<script>
  export default {
    components: {
      OneTime: () => import('./OneTime'),
      PatreonSub: () => import('@/components/supporters/PatreonSub'),
      Patrons: () => import('@/components/supporters/Patrons')
    }
  }
</script>
