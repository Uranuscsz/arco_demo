<template>
  <a-space>
    <a-input
      :style="{width:'320px'}"
      placeholder="Please enter something"
      allow-clear
    />
    <a-input
      :style="{width:'320px'}"
      default-value="content"
      placeholder="Please enter something"
      allow-clear
    />
  </a-space>
  <br>
  <Switch/>
  
</template>

<script lang="ts">
import { defineComponent, ref, getCurrentInstance, onMounted } from "vue";
import Switch from './components/switch.vue'
export default defineComponent({
  components: {Switch},
  setup() {
    const { proxy } = getCurrentInstance() as any;
    const name = ref("尼古拉斯凯奇");
    onMounted(() => {});
    return { name };
  },
});
</script>

<style lang="less" scoped></style>
