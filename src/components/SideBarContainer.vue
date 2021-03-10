<template>
  <div class="flex">
    <div class="flex flex-col h-screen w-72 bg-gray-800">
      <div class="flex-1 flex flex-col pt-5 pb-4 overflow-y-auto">
        <div class="flex items-center flex-shrink-0 px-4">
          <span class="flex flex-nowrap items-center">
            <svg
              class="h-10 w-10 text-indigo-500"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M9 20l-5.447-2.724A1 1 0 013 16.382V5.618a1 1 0 011.447-.894L9 7m0 13l6-3m-6 3V7m6 10l4.553 2.276A1 1 0 0021 18.382V7.618a1 1 0 00-.553-.894L15 4m0 13V4m0 0L9 7"
              />
            </svg>
            <span class="text-gray-300 font-bold text-xl pl-3">
              ASRM
            </span>
          </span>
        </div>
        <Nav></Nav>
      </div>
    </div>
    <div class="h-screen flex-grow flex flex-col bg-gray-200">
      <!-- content -->
      <slot></slot>
    </div>
  </div>
</template>

<script>
import Nav from "./Nav";
export default {
  name: "SideBarContainer",
  components: { Nav }
};
</script>
