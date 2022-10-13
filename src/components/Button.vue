<script setup>
defineProps({
  content: String,
})
</script>
<template>
  <button class="btn">{{ content }}</button>
</template>
