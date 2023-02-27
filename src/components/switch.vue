<template>
	  <a-space size="large">
    <a-switch />
    <a-switch type="round"/>
    <a-switch type="line"/>
  </a-space>
</template>

<script lang="ts">
import { defineComponent, ref, getCurrentInstance, onMounted } from 'vue';

export default defineComponent({
	components: {},
	setup() {
		const { proxy } = getCurrentInstance() as any;
		const name = ref('尼古拉斯凯奇');
		onMounted(() => {});
		return { name };
	},
});
</script>

<style lang="less" scoped></style>
