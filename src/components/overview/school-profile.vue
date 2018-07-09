<template>
  <div class="main flex-col flex-x-center flex-y-center">
    <div class="center">
      <!--头部-->
      <my-head/>
      <div class="list flex-row flex-space-between">
        <div class="list-left">
            <ul class="daohang2 flex-col flex-space-between flex-x-center">
              <router-link :to="{path:'/SchoolProfile'}"><li class="green-bg">学校简介</li></router-link>
              <router-link :to="{path:'/History'}"><li class="black-bg">百年历史</li></router-link>
              <router-link :to="{path:'/Teacher'}"><li class="black-bg">师资力量</li></router-link>
              <router-link :to="{path:'/GiftedPerson'}"><li class="black-bg">培道英才</li></router-link>
              <router-link :to="{path:'/BeautifulSchool'}"><li class="black-bg">美丽培道</li></router-link>
            </ul>
        </div>
        <div class="list-right flex-col">
          <div class="list-right-title flex-row flex-y-center"><span class="list-right-title-inner">您当前的位置：学校简介</span></div>
          <div class="list-right-inner flex-col flex-right">
            <div class="profile-inner flex-col flex-space-around ">
              <div v-for="item in items">
            <router-link :to="{path:'/Inside'}" >
            <span class="words-width flex-row flex-space-between" ><p>{{item.message}}</p><p>2017-07-10</p></span>       
          </router-link>
              </div>
            </div>
          </div>
          <div class="list-right-bottom flex-row flex-right flex-x-center flex-y-center">
          <ul class="flex-row flex-right flex-x-center">
            <li class="list-right-bottom-li">首页</li>
            <li class="list-right-bottom-li">上一页</li>
            <li class="list-right-bottom-li">下一页</li>
            <li class="list-right-bottom-li">末页</li>
          </ul>
          <span>页码：1/1</span>
          </div>
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
          {message:'校长简介'},
          {message:'东山钟灵，培道毓秀'},
           {message:'A Brief Introduction To Guangzhou Nu...'},
          {message:'培道校训'},
           {message:'广州培道教学理念————个性、合作、求实、发展'},
          {message:'校园歌曲《培道艳》'}
        ]
      }
    }
  }
</script>