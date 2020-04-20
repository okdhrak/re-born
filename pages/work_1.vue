<template>
	<div class="container">
		<p><img src="~/assets/image/work_1.gif"></p>
		<p><img src="~/assets/image/work_2.gif"></p>
	</div>
</template>


<script>
export default {
	layout: 'plain',
	head: {
	},
	head () {
		return {
			title: '事例1 🚀',
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
