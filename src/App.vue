<template>
  <div class="h-full w-full">
    <SideBarContainer>
      <Map></Map>
    </SideBarContainer>
  </div>
</template>

<script>
// import Map from "./components/Map";
import SideBarContainer from "./components/SideBarContainer";
import Map from "./components/Map";

export default {
  name: "App",
  components: {
    Map,
    SideBarContainer
  }
};
</script>
