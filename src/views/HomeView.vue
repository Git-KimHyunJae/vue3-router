<template>
  <div>
    <h2>Home View</h2>
    <p>{{ $route.path }}</p>
    <button class="btn btn-primary" @click="goAboutPage">About 으로 이동</button>
  </div>
</template>

<script setup>
import { useRoute,useRouter } from 'vue-router'
const route = useRoute()
const router = useRouter()
const goAboutPage = () => {
  router.push('/About')
}
</script>

<style lang="scss" scoped>

</style>