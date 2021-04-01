<template>
  <nav class="navbar bg-black max-w-full">
    <div class="max-w-full px-2 sm:px-6 lg:px-8">
      <div class="flex items-center justify-between h-16">
        <div class="flex item-center min-w-full">
          <!-- <div class="min-w-full flex grid grid-cols-3 gap-4 hidden md:block"> -->
          <div class="min-w-full flex">
            <div
              :class="'w-max visible md:invisible'"
              @click="showNav = !showNav"
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
                class="h-6 w-6 text-white"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M4 6h16M4 12h16M4 18h16"
                />
              </svg>
            </div>
            <div class="flex items-baseline hidden md:block">
              <a
                href="#"
                class="px-3 py-2 rounded-md text-sm font-bold text-gray-300 hover:text-white hover:bg-gray-700 focus:outline-none focus:text-white focus:bg-gray-700"
                >THE ETERNAL</a
              >
              <a
                href="#"
                class="ml-4 px-3 py-2 rounded-md text-sm font-bold text-gray-300 hover:text-white hover:bg-gray-700 focus:outline-none focus:text-white focus:bg-gray-700"
                >SHOP</a
              >
              <a
                href="#"
                class="ml-4 px-3 py-2 rounded-md text-sm font-bold text-gray-300 hover:text-white hover:bg-gray-700 focus:outline-none focus:text-white focus:bg-gray-700"
                >STORE</a
              >
            </div>
            <div id="logo" class="flex m-auto">
              <img src="logo.png" alt="logo" />
            </div>
            <div class="flex items-baseline hidden md:block">
              <a
                href="#"
                class="px-3 py-2 rounded-md text-sm font-bold text-gray-300 hover:text-white hover:bg-gray-700 focus:outline-none focus:text-white focus:bg-gray-700"
                >SIGN UP</a
              >
              <a
                href="#"
                class="ml-4 px-3 py-2 rounded-md text-sm font-bold text-gray-300 hover:text-white hover:bg-gray-700 focus:outline-none focus:text-white focus:bg-gray-700"
                >BAG(0)</a
              >
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Mobile menu, show/hide based on menu state. -->
    <div id="mobile-menu" class="sm:hidden">
      <div
        :class="
          'px-2 pt-2 pb-3 space-y-1 bg-black' +
          (showNav == true ? ' visible ' : ' invisible ')
        "
      >
        <!-- Current: "bg-gray-900 text-white", Default: "text-gray-300 hover:bg-gray-700 hover:text-white" -->
        <a
          href="#"
          class="bg-gray-900 text-white block px-3 py-2 rounded-md text-base font-medium"
          aria-current="page"
          >THE ETERNAL</a
        >
        <a
          href="#"
          class="text-gray-300 hover:bg-gray-700 hover:text-white block px-3 py-2 rounded-md text-base font-medium"
          >SHOP</a
        >
        <a
          href="#"
          class="text-gray-300 hover:bg-gray-700 hover:text-white block px-3 py-2 rounded-md text-base font-medium"
          >STORE</a
        >
        <a
          href="#"
          class="text-gray-300 hover:bg-gray-700 hover:text-white block px-3 py-2 rounded-md text-base font-medium"
          >SIGN-UP</a
        >
        <a
          href="#"
          class="text-gray-300 hover:bg-gray-700 hover:text-white block px-3 py-2 rounded-md text-base font-medium"
          >BAG(0)</a
        >
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      showNav: false,
    }
  },
}
</script>

<style>
.navbar {
  height: 64px;
}
#logo {
  width: 7em;
}
</style>
