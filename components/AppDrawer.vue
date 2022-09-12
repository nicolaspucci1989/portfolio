<template>
  <div class="drawer-side">
    <label for="my-drawer-2" class="drawer-overlay"></label>
    <!--    TODO: center here-->
    <div class="overflow-y-auto flex lg:justify-end w-fit lg:w-[40vw]">
      <!-- Sidebar content here -->
      <div class="w-fit p-3 lg:m-6 bg-base-100">
        <DrawerAvatar :src="data.src"/>
        <h1 class="text-2xl p-2 pl-4">{{ data.title }}</h1>
        <p class="text-sm pl-4">{{ data.subtitle }}</p>
        <DrawerSocials/>
        <div class="divider"></div>
        <DrawerMenu/>
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
const data = {
  title: 'Nicolas Pucci',
  subtitle: 'Desarrolador Web',
  src: 'https://api.lorem.space/image/face?hash=92310'
}
</script>

<style scoped>

</style>
