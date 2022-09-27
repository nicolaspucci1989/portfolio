<template>
  <div class="avatar w-60">
    <div class="w-16 lg:w-32 rounded-full mx-auto">
      <img src="~/assets/img/avatar.png"/>
    </div>
  </div>
</template>

<script lang="ts" setup>
defineProps<{
  src: string
}>()
</script>

<style scoped>

</style>
