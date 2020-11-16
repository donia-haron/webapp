<template>
<div class="post-box">
	<span class="post-views">{{views}}</span>
	<h3 class="post-title">{{title | uppercase}}</h3>
	<span class="post-date">{{date}}</span>
	<p class="post-content">{{content |shorten(20)}}</p>
	<div class="row">
	<div class="col-sm-6"> 
	<span class="post-author">{{author}}</span>
	</div>
	<div class="col-sm-6 text-right"> 
	<span class="post-category">{{category}}</span>
	</div>
	</div>

</div>

</template>
<style lang="scss" scoped>
.post-box{
	padding:15px;
	background-color:#fff;
	box-shadow:0 0 10px #DDD;
	position:relative;
	text-align:left;
	.post-views{
		   position:absolute;
			top:5px;
			right:5px;
			background-color:#F00;
			border-radius:4px;
			padding:1px 5px;
			color:#FFF;
			text-align:center;
			font-weight:bold;
	          }
	.post-title{
		color:#818080;
		font-weight:bold;
	}
	.post-date{
		display:block;
		padding:0 0 5px;
		color:#888;
		font-size:14px;
	}
	.post-content{
		line-height:1.8;
		color:#666;
	}
	.post-author{
		background-color:#607D8B;
		padding:6px 10px;
		border-radius:4px;
		color:#FFF;
	}
    .post-category {
        background-color: #E91E63;
        padding: 6px 10px;
        border-radius: 4px;
        color: #FFF;
    }
}


</style>


<script>
	export default {
	props:["views","title","author","category","content","date"],
	name:"post",
	};

</script>
