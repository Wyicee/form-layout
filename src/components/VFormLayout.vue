<script setup>
import VIllustration from '@/components/form-layout/VIllustration.vue'
import VForm from '@/components/form-layout/VForm.vue'
</script>

<template>
  <main class="main-wrapper">
    <div class="main-wrapper__body">
      <v-illustration />
      <v-form />
    </div>
  </main>
</template>

<style scoped lang="scss">
.main-wrapper {
  width: 100%;
  margin: rem(20);
  background: var(--color-light);
  box-shadow: var(--shadow);
  border: var(--border);
  border-radius: rem(35);

  &__body {
    display: flex;
    justify-content: space-between;
  }
}
</style>
