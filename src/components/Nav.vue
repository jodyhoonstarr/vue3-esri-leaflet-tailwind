<template>
  <nav class="mt-5 flex-1 px-2 bg-gray-800 space-y-1" aria-label="Sidebar">
    <!-- Current: "bg-gray-900 text-white", Default: "text-gray-300 hover:bg-gray-700 hover:text-white" -->
    <a
      href="#"
      class="bg-gray-900 text-white group flex items-center px-2 py-2 text-sm font-medium rounded-md"
    >
      <!-- Current: "text-gray-300", Default: "text-gray-400 group-hover:text-gray-300" -->
      <!-- Heroicon name: home -->
      <svg
        class="text-gray-300 mr-3 h-6 w-6"
        xmlns="http://www.w3.org/2000/svg"
        fill="none"
        viewBox="0 0 24 24"
        stroke="currentColor"
        aria-hidden="true"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          d="M3 12l2-2m0 0l7-7 7 7M5 10v10a1 1 0 001 1h3m10-11l2 2m-2-2v10a1 1 0 01-1 1h-3m-6 0a1 1 0 001-1v-4a1 1 0 011-1h2a1 1 0 011 1v4a1 1 0 001 1m-6 0h6"
        />
      </svg>
      Home
    </a>

    <a
      href="#"
      class="text-gray-300 hover:bg-gray-700 hover:text-white group flex items-center px-2 py-2 text-sm font-medium rounded-md"
    >
      <!-- Heroicon name: search -->
      <svg
        class="text-gray-400 group-hover:text-gray-300 mr-3 h-6 w-6"
        xmlns="http://www.w3.org/2000/svg"
        fill="currentColor"
        viewBox="0 0 24 24"
        stroke="none"
        aria-hidden="true"
      >
        <path
          fill-rule="evenodd"
          d="M8 4a4 4 0 100 8 4 4 0 000-8zM2 8a6 6 0 1110.89 3.476l4.817 4.817a1 1 0 01-1.414 1.414l-4.816-4.816A6 6 0 012 8z"
          clip-rule="evenodd"
        />
      </svg>
      Search
    </a>

    <a
      href="#"
      class="text-gray-300 hover:bg-gray-700 hover:text-white group flex items-center px-2 py-2 text-sm font-medium rounded-md"
    >
      <!-- Heroicon name: outline/folder -->
      <svg
        class="text-gray-400 group-hover:text-gray-300 mr-3 h-6 w-6"
        xmlns="http://www.w3.org/2000/svg"
        fill="currentColor"
        viewBox="0 0 24 24"
        stroke="none"
        aria-hidden="true"
      >
        <path
          fill-rule="evenodd"
          d="M5.05 4.05a7 7 0 119.9 9.9L10 18.9l-4.95-4.95a7 7 0 010-9.9zM10 11a2 2 0 100-4 2 2 0 000 4z"
          clip-rule="evenodd"
        />
      </svg>
      Add Address
    </a>
  </nav>
</template>

<script>
export default {
  name: "Nav"
};
</script>
