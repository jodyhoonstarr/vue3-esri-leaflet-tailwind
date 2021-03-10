<template>
  <div id="mapContainer"></div>
</template>

<script>
import { map, tileLayer } from "leaflet";
import { onMounted, onBeforeUnmount } from "vue";

export default {
  name: "Map",
  setup() {
    let container = null;

    onMounted(() => {
      container = map("mapContainer").setView([51.959, -8.623], 12);

      tileLayer("http://{s}.tile.osm.org/{z}/{x}/{y}.png", {
        attribution:
          '&copy; <a href="http://osm.org/copyright">OpenStreetMap</a> contributors'
      }).addTo(container);
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
