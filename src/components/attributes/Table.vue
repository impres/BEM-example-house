<template>
	<div class="table">
		<div class="table__top">
			<div class="table__on-table">
				<slot></slot>
			</div>
		</div>
		<div class="table__legs">
			<div class="table__leg"></div>
			<div class="table__leg"></div>
		</div>
	</div>
</template>


<style lang="scss">
	.table {
		width: 100px;
		margin: 10px;

		&__top {
			height: 5px;
			background: brown;
			position: relative;
		}

		&__legs{
			display: flex;
			justify-content: space-between;
		}

		&__leg {
			width: 10px;
			height: 50px;
			background: brown;
		}

		&__on-table{
			position: absolute;
			bottom: 0;
			left: 50%;
			transform: translate(-50%,-100%);
		}
	}

</style>
