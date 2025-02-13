<script setup>

</script>

<template>
  <div class="illustrator">
    <div class="illustrator__body">
      <span class="top-left-planet"></span>
      <img
        class="illustrator__body-skeleton"
        src="../../assets/images/skeleton.svg"
        alt=""
        width="500" height="565"
      >
      <h1 class="illustrator__title">Turn your ideas into reality.</h1>
      <h2 class="illustrator__tag h3">Start for free and get attractive offers from the community</h2>
    </div>
  </div>
</template>

<style scoped lang="scss">
.illustrator {
  color: var(--color-accent);
  background-color: var(--color-background);
  border-radius: rem(35) 0 0 rem(35);
  max-width: rem(1100);
  width: 100%;
  position: relative;
  overflow: hidden;

  &__body {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: rem(80) rem(120) rem(80) rem(120);
  }

  .top-left-planet::after {
    content: url('@/assets/images/top-left-planet.svg');
    position: absolute;
    top: rem(-100);
    left: rem(-80);
  }

  &__title {
    margin-top: rem(29);
  }
}
</style>
