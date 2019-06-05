<template>
	<div class="house"  v-bind:class="{ 'house--stone-red': red}">
		<slot>House</slot>
	</div>
</template>
<script>
	export default {
		props: {
			red: Boolean
		}
	}
</script>
