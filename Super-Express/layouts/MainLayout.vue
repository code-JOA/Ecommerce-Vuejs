<template>
  <div id="MainLayout" class="w-full fixed z-50">
    <div id="TopMenu" class="w-full bg-[#fafafa] border-b md:block hidden">
      <ul
        class="flex items-center justify-end text-xs text-[#333333] font-light px-2 h-10 bg-[#fafafa] max-w-[1200px]"
      >
        <li
          class="border-r border-r-gray-400 px-3 hover:text-[#ff4646] cursor-pointer"
        >
          Sell On AliExpress
        </li>
        <li
          class="border-r border-r-gray-400 px-3 hover:text-[#ff4646] cursor-pointer"
        >
          Cookie Preferences
        </li>
        <li
          class="border-r border-r-gray-400 px-3 hover:text-[#ff4646] cursor-pointer"
        >
          Help
        </li>
        <li
          class="border-r border-r-gray-400 px-3 hover:text-[#ff4646] cursor-pointer"
        >
          Buyer Protection
        </li>
        <li class="px-3 hover:text-[#ff4646] cursor-pointer">
          <Icon name="ic:sharp-install-mobile" size="17" />
          App
        </li>
        <li
          @mouseenter="isAccountMenu = true"
          @mouseleave="isAccountMenu = false"
          class="relative flex items-center px-2.5 hover:text-[#ff4646] h-full cursor-pointer"
          :class="isAccountMenu ? 'bg-white border z-40 
        shadow-[0_15px_100px_40px_rgba(0,0,0,0.3)]' : border border"
        >
          <Icon name="ph:user-thin" size="17" />
          Account
          <Icon name="mdi:chevron-down" size="15" class="ml-5" />
        </li>
      </ul>
    </div>
  </div>
</template>

<script setup>
let isAccountMenu = ref(false);
</script>
