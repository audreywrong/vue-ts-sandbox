<script setup>
import { NavBar, BaseAlert } from '@/components'
import { useAuthStore } from '@/stores'

const authStore = useAuthStore()
</script>

<template>
  <div class="app-container" :class="authStore.user && 'bg-light'">
    <NavBar />
    <BaseAlert />
    <div class="container pt-4 pb-4">
      <router-vew />
    </div>
  </div>
</template>

<style>
@import '@/assets/base.css';
</style>
