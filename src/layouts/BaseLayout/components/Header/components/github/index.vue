<script setup>
import { Github } from 'lucide-vue-next'
import { BrowserUtils } from '@/utils/index.ts'
import { AppMetadata } from '@/constants/index.ts'
</script>

<template>
  <Github
    :size="24"
    class="cursor-pointer hover:text-orange-500"
    @click="() => BrowserUtils.openNewWindow(AppMetadata.REPO_GITHUB_URL)"
  />
</template>
