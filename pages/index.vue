<script setup lang="ts">
const { setLocale } = useI18n()
</script>

<template>
  <div class="h-full w-full flex flex-col items-center justify-center">
    <div class="flex items-center text-3xl text-red font-semibold">
      <button @click="setLocale('en')">EN</button>
      <button @click="setLocale('fr')">FR</button>
      <p>Darius, {{ $t('welcome') }}</p>
    </div>


    <p>Liste of buttons</p>
    <Button variant="destructive">
      Button
    </Button>
  </div>
</template>
