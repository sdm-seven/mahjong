<template>
	<view>
		<view class="section">
			<!-- <view class="section__title">flex-direction: column</view> -->
			<view class="flex-wrp" style="height: 300px;">
				<!--  <view class="flex-item bc_green " style="margin: 5px;">1</view>
                <view class="flex-item bc_red" style="margin: 5px;">2</view>
                <view class="flex-item bc_blue" style="margin: 5px;">3</view> -->

				<view class="index-content" style="display: flex;flex-direction: column;">
					<view class="li index1">
						<navigator href="findWorker/all-orders.html"><i></i><em>我想找师傅上门帮我维修和安装麻将机</em></navigator>
					</view>
					<view class="li index2">
						<navigator href="worker/waiting-orders.html"><i></i><em>我想去维修和安装麻将机<text>（需通过技术员认证）</text></em></navigator>
					</view>
					<view class="li index3">
						<navigator href="praise/my-brand.html"><i></i><em>被赞最多的麻将机10大品牌评选</em></navigator>
					</view>
					<view class="li index4">
						<navigator href="ad/ad-hall.html"><i></i><em>麻将机行业广告区</em></navigator>
					</view>						
					<view class="li index5">
						<navigator href="mall/shop-index.html"><i></i><em>商城（可以在这里开淘宝或者京东的分店）</em></navigator>
					</view>
					<view class="li index6">
						<navigator href="personal/leave-message.html"><i></i><em>留言箱<text>（我们会在第一时间给您答复）</text></em></navigator>
					</view>
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data: {
			orders: [{
				orderNo: '1',
				title: '1',
				address: '',
				publisher: '',
				publishTime: '',
				detailAdd: '',
				tel: ''
			}, {
				orderNo: '2',
				title: '2',
				address: '',
				publisher: '',
				publishTime: '',
				detailAdd: '',
				tel: ''
			}]
		}
	}
</script>

<style>
	@import "../lib/weui.wxss";

	.page-section {
		margin-bottom: 20rpx;
	}

	.section__title {
		display: flex;
		flex-direction: column;
	}

	.flex-wrp {
		display: flex;
		flex-direction: column;
	}


	.index1 {
		background: #8ecdf6;
		box-shadow: 0 0.05rem 0.3rem rgba(142, 205, 246, 0.75);
	}

	.index2 {
		background: #83dfb6;
		box-shadow: 0 0.05rem 0.3rem rgba(131, 223, 182, 0.75);
	}

	.index3 {
		background: #e3cfae;
		box-shadow: 0 0.05rem 0.3rem rgba(227, 207, 174, 0.75);
	}

	.index4 {
		background: #aec1e3;
		box-shadow: 0 0.05rem 0.3rem rgba(142, 205, 246, 0.75);
	}

	.index5 {
		background: #fad680;
		box-shadow: 0 0.05rem 0.3rem rgba(250, 214, 128, 0.75);
	}

	.index6 {
		background: #fca2c8;
		box-shadow: 0 0.05rem 0.3rem rgba(252, 162, 200, 0.75);
	}
	.index-content view{
		margin: 2px 5px;;
	}

	.index-content .li .i {
		width: 1.08rem;
		height: 1.08rem;
		background-size: cover;
		float: left;
		margin-left: 0.5rem;
		margin-right: 0.25rem;
	}

	.index-content .li em {
		width: 5.1rem;
		color: #fff;
		font-size: 0.38rem;
		font-weight: 0.44rem;
	}

	.index-content .li em span {
		margin-left: -0.3rem;
	}

	/* .index1 .i {
		background-image: url("../images/icon/index-1.png");
	}

	.index2 .i {
		background-image: url("../images/icon/index-2.png");
	}

	.index3 .i {
		background-image: url("../images/icon/index-3.png");
	}

	.index4 .i {
		background-image: url("../images/icon/index-4.png");
	}

	.index5 .i {
		background-image: url("../images/icon/index-5.png");
	}

	.index6 .i {
		background-image: url("../images/icon/index-6.png");
	} */
</style>
