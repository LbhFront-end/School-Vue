<template>
  <div class="main flex-col flex-x-center flex-y-center">
    <div class="center">
      <!--头部-->
      <my-head/>
      <div class="list flex-row flex-left flex-space-between">
        <div class="list-left">
            <ul class="daohang1 flex-col flex-space-between flex-x-center">
               <router-link :to="{path:'/Achievement'}"><li class="black-bg">教学成果</li></router-link>
              <router-link :to="{path:'/TeachingResearch'}"><li class="black-bg">教学研究</li></router-link>
              <router-link :to="{path:'/EnvironmentalProtectionTeaching'}"><li class="black-bg">环保教育</li></router-link>
              <router-link :to="{path:'/TeachingResource'}"><li class="green-bg">教育资源</li></router-link>
            </ul>
        </div>
        <div class="list-right flex-col">
          <div class="list-right-title flex-row flex-y-center"><span class="list-right-title-inner">您当前的位置：教育资源</span></div>
            <span class="flex-row"><p>暂无消息</p></span>       
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
