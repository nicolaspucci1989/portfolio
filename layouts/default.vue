<template>
  <div class="drawer drawer-mobile">
    <input id="my-drawer-2" type="checkbox" class="drawer-toggle"/>
    <div class="drawer-content flex justify-center lg:justify-start">
      <div class="lg:w-[60vw] max-w-screen-lg lg:pt-4 lg:p-4">
        <AppHeader/>
        <div class="flex-1 p-3 md:py-[35]">
          <NuxtPage/>
          <div class="divider"></div>
          <Footer/>
        </div>
      </div>
    </div>
    <AppDrawer/>
  </div>
</template>

<script lang="ts" setup>

</script>

<style scoped>

</style>
