<template>
	<div class="flower">
		<div class="flower__center">
			<div class="flower__leaf"></div>
			<div class="flower__leaf"></div>
			<div class="flower__leaf"></div>
			<div class="flower__leaf"></div>
			<div class="flower__leaf"></div>
		</div>
	</div>
</template>

<style lang="scss">
	.flower {
		position: relative;
		height: 20px;

		&__center {
			border-radius: 100%;
			background: orange;
			width: 10px;
			height: 10px;
			position: relative;
		}

		&__leaf {
			width: 20px;
			height: 5px;
			border-radius: 100%;
			background: yellowgreen;
			position: absolute;
			left: 50%;
			top: 50%;
			transform-origin: center;
			z-index: -10;

			&:nth-child(1){
				transform: translate(-50%, -50%)  rotate(72deg) ;
			}

			&:nth-child(2){
				transform: translate(-50%, -50%) rotate(144deg);
			}

			&:nth-child(3){
				transform: translate(-50%, -50%) rotate(216deg);
			}

			&:nth-child(4){
				transform: translate(-50%, -50%) rotate(288deg);
			}

			&:nth-child(5){
				transform: translate(-50%, -50%) rotate(360deg);
			}
		}
	}
</style>
