<template>
  <div class="slidev-layout center">
    <div class="my-auto w-full">
      <slot />
    </div>
  </div>
</template>

<style lang="postcss">
.slidev-layout.center {
  /* 居中 */
  @apply flex items-center justify-center;
  @apply text-center;
  h1 {
    @apply text-6xl mb-5;
    @apply inline-block;

    @apply pb-1 pr-5 pl-5;
    background-image: linear-gradient(90deg, #edb6c8, #f9debb);
    background-position: bottom;
    background-size: 100% 50%;
    background-repeat: no-repeat;
  }
}


</style>