<script setup lang="ts">
const zoom = ref(6)
</script>

<template>
  <div style="height:100vh; width:100vw">
    <LMap
        ref="map"
        :zoom="zoom"
        :center="[47.21322, -1.559482]"
    >
      <LTileLayer
          url="https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png"
          attribution="&amp;copy; <a href=&quot;https://www.openstreetmap.org/&quot;>OpenStreetMap</a> contributors"
          layer-type="base"
          name="OpenStreetMap"
      />
    </LMap>
  </div>
</template>

<style scoped>

</style>