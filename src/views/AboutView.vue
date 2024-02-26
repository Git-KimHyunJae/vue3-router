<template>
  <div>
    <h2>About View</h2>
    <p>{{ $route.path }}</p>
    <button class="btn btn-primary" @click="goHome">Home 으로 이동</button>
  </div>
</template>

<script setup>
import {useRoute,useRouter} from 'vue-router'
const route = useRoute()
const router = useRouter()

const goHome = () => {
  router.push('/')
}
</script>


<style lang="scss" scoped>

</style>