<template>
  <div class="navbar bg-base-100 lg:hidden sticky top-0 w-full z-50">
    <div class="flex-none">
      <HamburgerBtn/>
    </div>
    <div class="flex-1">
      <router-link class="btn btn-ghost normal-case text-xl" :to="{name: 'index'}">Portfolio</router-link>
    </div>
    <div class="flex-none">
      <AppSolarMode/>
      <AppReadMode/>
      <AppDarkMode/>
    </div>
  </div>
</template>

<script lang="ts" setup>
</script>

<style scoped>

</style>
