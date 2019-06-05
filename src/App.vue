<template>
	<div id="app">

		<House>
			<HouseRoom>
				<Chair></Chair>
				<Chair></Chair>
			</HouseRoom>
			<HouseRoom></HouseRoom>
			<HouseRoom></HouseRoom>
			<HouseRoom></HouseRoom>
		</House>
		<div class="garden">garden</div>
	</div>
</template>

<script>
	import House from './components/House'
	import HouseRoom from './components/HouseRoom'
	import Chair from './components/Chair'

	export default {
		name: 'app',
		components: {
			House,
			HouseRoom,
			Chair
		}
	}
</script>

<style>
	#app {
		font-family: 'Avenir', Helvetica, Arial, sans-serif;
		-webkit-font-smoothing: antialiased;
		-moz-osx-font-smoothing: grayscale;
		text-align: center;
		color: #2c3e50;
		margin-top: 60px;
	}
</style>
