<template>
  <div class="m-card" :style="width? {width: width + 'px'} : {}">
    <div class="m-card-img" :style="imgHeight? {height: imgHeight + 'px'} : {}">
      <img :src="imgSrc" alt="img">
    </div>
    <div v-if="summary" class="m-card-summary">
      {{summary}}
    </div>
    <div v-else class="m-card-summary">
      <slot></slot>
    </div>
    <slot name="footer"></slot>

  </div>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: 'm-card',
  props: {
    width: {// 卡片宽度
      type: Number,
      default: 0,
    },
    imgSrc: {// 卡片地址
      type: String,
      default: '',
    },
    imgHeight: {//卡片高度
      type: Number,
      default: 0,
    },
    summary: {//卡片概述
      type: String,
      default: '',
    }
  }
}
</script>
<style lang="scss">
@import "./card.scss";
</style>
