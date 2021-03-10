<template>
  <div id="mapContainer"></div>
</template>

<script>
import { map } from "leaflet";
import { basemapLayer } from "esri-leaflet";
import { onMounted, onBeforeUnmount } from "vue";

export default {
  name: "Map",
  setup() {
    let container = null;

    onMounted(() => {
      container = map("mapContainer").setView([51.959, -8.623], 6);

      basemapLayer("Streets").addTo(container);
    });

    onBeforeUnmount(() => {
      container.remove();
    });
  }
};
</script>

<style scoped>
#mapContainer {
  width: 40vw;
  height: 40vh;
}
</style>
