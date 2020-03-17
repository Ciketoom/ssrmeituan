<template>
  <div class="scene">
  	<dl class="dll">
  		<dt class="dtt">
  			<dd class="ddd">有格调</dd>
	  		<dd>全部</dd>
	  		<dd>约会聚餐</dd>
	  		<dd>丽人SPA</dd>
	  		<dd>电影演出</dd>
	  		<dd>品质出游</dd>
  		</dt>
  	</dl>
  	<div class="down">
  		<a href="#">
  			<div class="img"
  				v-for="item in imglist" 
         :key="item.img">
        <img :src="item.img">
  			</div>
  		</a>
  	</div>
  </div>
</template>

<script>
export default {
	data: () => {
    return {
      imglist: [{
        url: '#abc',
        img: 'http://p0.meituan.net/codeman/00c8bc1c25fbcc6d0651b29a2057a8c1560658.png'
      }, {
        url: '#bsbsb',
        img: 'http://p1.meituan.net/codeman/826a5ed09dab49af658c34624d75491861404.jpg'
      }, {
        url: '#sjfkajfj',
        img: 'http://p0.meituan.net/codeman/a97baf515235f4c5a2b1323a741e577185048.jpg'
      }, {
        url: '#sjfkajfja',
        img: 'http://p0.meituan.net/codeman/33ff80dc00f832d697f3e20fc030799560495.jpg'
      }, {
        url: '#kjljj',
        img: 'http://p1.meituan.net/codeman/bb0abb3435a60c44d87e90ed4237b61039329.jpg'
      },
      {
        url: '#kjljj',
        img: 'http://p1.meituan.net/codeman/bb0abb3435a60c44d87e90ed4237b61039329.jpg'
      }]
    }
  }
}
</script>

<style lang="css">
.scene{
	width: 1170px;
    margin-left: 20px;
  	margin-top: 40px;
}
.dll{
	height: 44px;
    line-height: 44px;
    background-color: rgb(190, 164, 116);
    width: 1170px;
   
    
    font-size: 14px;
    color: #fff;
    border-top-right-radius: 5px;
    border-top-left-radius: 5px;
    
}
	    
.dtt dd{
	display: inline-flex;
	padding-left: 10px;	
}
.img{
	text-align: center;
}
</style>