<template>
	<div id="app">

		<House red>
			<HouseRoom>
				<div style="display: flex; align-items: flex-end;">
					<Chair></Chair>
					<Table>
						<Flower></Flower>
					</Table>
					<Chair right></Chair>
				</div>
			</HouseRoom>
			<HouseRoom></HouseRoom>
			<HouseRoom></HouseRoom>
			<HouseRoom></HouseRoom>
		</House>
		<Garden>
			<div style="display: flex; align-items: flex-end;">
			</div>
		</Garden>
	</div>
</template>

<script>
	import House from './components/House'
	import Garden from './components/Garden'
	import HouseRoom from './components/HouseRoom'
	import Chair from './components/attributes/Chair'
	import Table from './components/attributes/Table'
	import Flower from './components/attributes/Flower'

	export default {
		name: 'app',
		components: {
			House,
			Garden,
			HouseRoom,
			Chair,
			Table,
			Flower
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
