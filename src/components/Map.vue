<template>
  <div class="h-full w-full" id="mapContainer"></div>
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
      container = map("mapContainer").setView([38.9072, -77.0369], 12);

      basemapLayer("Topographic").addTo(container);
    });

    onBeforeUnmount(() => {
      container.remove();
    });
  }
};
</script>
