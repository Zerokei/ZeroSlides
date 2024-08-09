<template>
  <div class="slidev-layout single">
    <div class="my-auto w-full">
      <slot />
    </div>
  </div>
</template>

<style lang="postcss">
.slidev-layout.single {
  /* 居中 */
  @apply flex items-center justify-center;
  @apply text-center;
  h1 {
    font-family: 'Smiley Sans Oblique';
    @apply text-6xl mb-5 text-amber-900;
    @apply inline-block;

    @apply pb-1 pr-5 pl-5;
  }
  .footnote-ref {
    @apply text-3xl;
  }
  .footnotes {
    @apply text-sm;
  }
}


</style>
