<template lang="html">
	<div class="kuang">
		<div class="sign">
			<span class="left">
				<p>会员等级</p>
			</span>
			<div class="center">
				<p>立即登录&nbsp;马上赚钱！</p>
			</div>
			<div class="right">
				<p>签到</p>
			</div>
		</div>
	</div>
</template>

<script>
</script>

<style lang="scss">
	.kuang{
		width: 640px;
		height: 130px;
		margin-top: -46px;
		margin-bottom: 20px;
		background-color: #fff;
		.sign{
			margin: 0 32px;
			height: 130px;
			background: #fff;
			text-align: center;
			position: relative;
			border-radius: 2px;
			z-index: 3;
			box-shadow: 0 0 10px 0.5px rgba(101,118,155,.15);
			.left{
				position: absolute;
				left: 0;
				top:30px;
				width: 112px;
				height: 66px;
				p{
					width: 92px;
					height: 66px;
					line-height: 66px;
					margin-left: 20px;
					color: #fff;
					background-color: #c6a76f;
					font-size: 18px;
					border-radius: 4px;
					box-shadow: 0 6px 8px 0 hsla(41,44%,63%,.51);
				}
			}
			.center{
				margin: 0 170px 0 112px;
				height: 100%;
				p{
					font-family: PingFangSC-Semibold;
					font-size: 28px;
					color: #c6a76f;
					letter-spacing: 0;
					line-height: 130px;
					text-align: left;
					padding-left: 20px;
					box-sizing: border-box;
				}
			}
			.right{
				width: 170px;
				position: absolute;
				right: 0;
				top: 30px;
				p{
					width: 140px;
					height: 66px;
					line-height: 66px;
					color: #fff;
					font-size: 24px;
					border-radius: 30px;
					background-color: #c6a76f;
					box-shadow: 0 8px 12px 0 hsla(40,41%,61%,.41);
				}
			}
		}
	}
</style>
