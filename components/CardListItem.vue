<template>
  <div class="card md:card-side bg-base-100 shadow-xl">
    <figure v-if="img">
      <img
          :src="img"
          alt="image"
          width="400"
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
      <article class="prose prose-stone" v-html="text">
      </article>
      <div class="card-actions justify-end">
        <button class="btn btn-primary">
          <a :href="link" target="_blank">
            <span class="mr-3">Ver en Github</span>
            <GithubIcon/>
          </a>
        </button>
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>

defineProps<{
  title: string
  text: string
  img?: string
  link: string
  tags: {
    color: string
    name: string
  }
}>()
</script>
