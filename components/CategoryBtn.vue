<template>
  <button
      class="btn btn-xs mr-1.5 hover:cursor-default hover:bg-"
      :class="colorClass"
  >
    {{ name }}
  </button>
</template>

<script lang="ts" setup>
import {computed} from "#imports";

const props = defineProps<{
  name: string
  color: string
}>()

const colors = {
  yellow: 'btn-warning',
  red: 'btn-warning',
  green: 'btn-success',
  secondary: 'btn-secondary',
  primary: 'btn-primary',
  accent: 'btn-accent'
}

const colorClass = computed(() => colors[props.color])
</script>
