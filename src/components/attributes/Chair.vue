<template>
	<div class="chair" v-bind:class="{ 'chair--right': right}">
		<div class="chair__back"></div>
		<div class="chair__seat"></div>
		<div class="chair__legs">
			<div class="chair__leg"></div>
			<div class="chair__leg"></div>
		</div>
	</div>
</template>
<script>
	export default {
		props: {
			right: Boolean
		}
	}
</script>
<style lang="scss">
	.chair {
		$s: &;
		width: 50px;
		margin: 10px;


		&__back {
			width: 5px;
			height: 30px;
			background: brown;
		}

		&__seat {
			clear:both;
			height: 5px;
			background: brown;
		}

		&__legs {
			display: flex;
			justify-content: space-between;
		}

		&__leg {
			width: 10px;
			height: 30px;
			background: brown;
		}

		&--right {
			#{$s}__back {
				float: right;
			}
		}
	}

</style>
