<script setup lang="ts">
import { ref } from "vue";

defineProps<{ msg: string }>();

const count = ref(0);
const value = ref(true);
// const color=
</script>

<template>
	<el-button type="info">+新建项目</el-button>
	<div class="project">
		<el-button type="info">体验</el-button>
		<span class="default">设置默认</span>
		<el-switch v-model="value" />
		<el-icon :size="30" :color="hotpink">
			<Edit />
		</el-icon>
	</div>
</template>

<style scoped>
.project {
	margin-top: 20px;
	border: 2px solid #000;
	display: flex;
	padding: 5px 10px 10px 10px;
	.default {
		display: line-block;
		font-size: 12px;
		margin-top: 2px;
	}
}
</style>
