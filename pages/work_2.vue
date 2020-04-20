<template>
	<div class="container">
		<p>ただいまリニューアル作業中です！乞うご期待！</p>
		<p><img src="~/assets/image/work_3.gif"></p>
	</div>
</template>


<script>
export default {
	layout: 'plain',
	head: {
	},
	head () {
		return {
			title: '事例2 🚀',
		}
	},
	data: function(){
		return {
			title: '俺のホームページ',
			message: 'this is message.',
		};
	},
};
</script>

<style lang="scss">
.container {
	text-align: center;
	p {
		margin: 30px 0 0;
	}
}
</style>
