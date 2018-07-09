<template>
  <div class="main flex-col flex-x-center flex-y-center">
    <div class="center">
      <!--头部-->
      <my-head/>
      <!--位置提示栏-->
      <div class="location flex-row flex-left flex-y-center ">
        <span class="location-inner flex-row flex-space-between">
          <p>您当前的位置：</p>
          <p>美丽培道</p>
        </span>
      </div>
       <div class="photonews flex-col flex-y-center flex-x-center">
        <div class="flex-col">
          <p class="photonews-title-1">美丽培道</p>
          <span class="photonews-title-2 flex-row  flex-space-between ">
            <p>发表时间：2017-09-13</p>&nbsp;&nbsp;
            <p>作者：七中宣传组</p>&nbsp;&nbsp;
            <p>浏览次数：121</p>
          </span>
        </div>
        <div class="photonews-inner flex-col flex-x-center" v-for="item in items">
          <img :src="'../../../static/img/beautifulSchool/'+item.message+'.jpg'" alt="" class="photonews-inner-img photo-width ">
        </div>
      </div>
       
    <!--底部-->
    <my-bottom/>
  </div>
  </div>
</template>

<script>
  export default {
    data(){
      return{
        items:[
          {message:'artRoom'},
          {message:'balcony'},
          {message:'biologicalRoom'},
          {message:'canteen1'},
          {message:'canteen2'},
           {message:'chemicalRoom'},
          {message:'classroom'},
           {message:'dormitory'},
          {message:'hall'},
           {message:'ITRoom'},
          {message:'musicRoom'},
           {message:'physicalRoom'}
          
        ]
      }
    }
  }
</script>
