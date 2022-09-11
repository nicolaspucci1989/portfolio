<template>
  <div class="card card-side bg-base-200 shadow-xl">
    <figure v-if="img">
      <img
          :src="img"
          alt="Book"
      />
    </figure>
    <div class="card-body">
      <h2 class="card-title">{{ title }}</h2>
      <div class="justify-start">
       <CategoryBtn
           v-for="tag in tags"
           v-bind="tag"
       />
      </div>
      <p>
        {{ text }}
      </p>
    </div>
  </div>
</template>

<script lang="ts" setup>

defineProps<{
  title: string
  text: string
  img?: string
  tags: {
    color: string
    name: string
  }
}>()
</script>
