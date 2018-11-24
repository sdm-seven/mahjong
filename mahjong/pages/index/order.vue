<template>
	<view class="content">
		<view class="section">		  
		  <view class="flex-wrp" style="height: 300px;flex-direction:column;">
			  <view v-for="(order,index) in orders" :key ="index">										  
					<view class="section__title">{{order.orderNo}}<navigator class='a' url="">【置顶】</navigator></view>
					<view class="flex-wrp" style="height: 300px;flex-direction:column;">
						<view class="flex-item">订单发布者：{{order.publisher}} <navigator url="" class="pull-r">申请维修并投送简历</navigator></view>
						<view class="flex-item">{{order.title}}</view>
						<view class="flex-item">大概地址：{{order.address}}</view>
						<view class="flex-item">详细地址：{{order.detailAdd}}</view>
						<view class="flex-item">电话：{{order.tel}}</view>
						<view class="flex-item">订单发布日期：{{order.publishTime}}</view>
					</view>
				</view>
		  </view>
		</view>
	</view>	
</template>

<script>
	export default {
		data: {
			orders:[{
				orderNo:'1',				
				title:'1',
				address:'',
				publisher:'',
				publishTime:'',
				detailAdd:'',
				tel:''
			},{
				orderNo:'2',				
				title:'2',
				address:'',
				publisher:'',
				publishTime:'',
				detailAdd:'',
				tel:''
			}]
		}
	}
</script>

<style>
	.content {
		flex: 1;
		justify-content: center;
		align-items: center;
	}

	.title {
		font-size: 36upx;
		color: #8f8f94;
	}
	
	.box{
	    box-shadow: 0 0.01rem 0.1rem #ececec;
	    background-color: #fff;
	    margin-bottom: 0.3rem;
	    border-radius: 0.1rem;
	    position: relative;
	}
	
	.box .h2{
	    font-weight: 400;
	    color: #999999;
	    font-size: 0.26rem;
	    padding: 0.15rem 0.2rem 0.1rem;
	    border-bottom: 1px dotted #e4e4e4;
	}
	.box .h2 .a{
	    color: #f68e8e;
	    font-size: 0.28rem;
	    float: right;
	}
	.box .ul{
	    padding: 0.2rem;
	}
	.box .ul .li{
	    margin-bottom: 0.2em;
	}
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
</style>
