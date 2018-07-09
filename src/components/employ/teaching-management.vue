<template>
  <div class="main flex-col flex-x-center flex-y-center">
    <div class="center">
      <!--头部-->
      <my-head/>
      <div class="list flex-row flex-left flex-space-between">
        <div class="list-left">
            <ul class="list-left-inner flex-col flex-space-between flex-x-center">
              <router-link :to="{path:'/GermanManagement'}"><li class="black-bg">德育管理</li></router-link>
              <router-link :to="{path:'/SectionPage'}"><li class="black-bg">科组主页</li></router-link>
              <router-link :to="{path:'/TeachingManagement'}"><li class="green-bg">教学管理</li></router-link>
            </ul>
        </div>
        <div class="list-right flex-col">
          <div class="list-right-title flex-row flex-y-center"><span class="list-right-title-inner">您当前的位置：教学管理</span></div>
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

