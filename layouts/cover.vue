<script setup lang="ts">
import { computed } from 'vue'
import { handleBackground } from '../layoutHelper'

const props = defineProps({
  background: {
    default: '',
  },
})

const style = computed(() => handleBackground(props.background, true))
</script>

<template>
  <div class="slidev-layout cover" :style="style">
    <div class="my-20 w-full">
      <slot />
    </div>
  </div>
</template>

<style lang="postcss">
.slidev-layout.cover {
  background-image: url("../assets/cover.svg");
  h1 {
    /* 字体样式设置 */
    font-family: 'Smiley Sans Oblique';
    @apply text-8xl leading-20 text-amber-900;
    padding-bottom: 20px;
    padding-right: 50px;
    padding-left: 5px;

    /* 大标题下划线 */
    background-image: linear-gradient(90deg, #f080a5, #faa940);
    background-position: bottom;
    background-size: 100% 50%;
    background-repeat: no-repeat;
    @apply inline-block
  }
  h2 {
    /* 设置字体为黑体 */
    font-family: 'Noto Sans', 'Noto Sans SC', sans-serif;
    @apply text-5xl mt-10 text-black;
  }
  h3 {
    font-family: 'Jetbrains Mono';
    @apply text-5xl font-bold text-amber-600;
    /* 置底，右下角 */
    position: absolute;
    bottom: 40px;
    right: 40px;
  }
}
</style>