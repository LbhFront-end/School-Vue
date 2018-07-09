<template>
  <div class="main flex-col flex-x-center flex-y-center">
    <div class="center">
      <!--头部-->
      <my-head/>
      <div class="list flex-row flex-left flex-space-between">
        <div class="list-left">
            <ul class="list-left-inner flex-col flex-space-between flex-x-center">
             <router-link :to="{path:'/PhotoNews'}"><li class="black-bg">图片新闻</li></router-link>
              <router-link :to="{path:'/LatestInformation'}"><li class="black-bg">最新资讯</li></router-link>
              <router-link :to="{path:'/SchoolNotice'}"><li class="green-bg">学校公告</li></router-link>
            </ul>
        </div>
        <div class="list-right flex-col">
          <div class="list-right-title flex-row flex-y-center"><span class="list-right-title-inner">您当前的位置：学校公告</span></div>
          <div class="list-right-inner">
            <div class="list-right-inner-words   flex-col flex-space-around ">
              <div v-for="item in items">
             <router-link :to="{path:'/Inside'}" >
            <span class="list-right-inner-words1 flex-row flex-space-between"><p>{{item.message}}</p><p>2017-07-10</p></span>       
            
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
          <span>页码：1/8</span>
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
          {message:'2017级高一分班公布'},
          {message:'高一新生取得住宿资格名单'},
          {message:'2017高一新生住宿特别通知'},
          {message:'“培英计划”广州培道遂志班通知'},
          {message:'2017培道高一新生住宿申请'},
          {message:'2017高一新生报到分组名单'},
          {message:'“遂志班”招生报到'},
          {message:'遂志班招生简章'},
          {message:'2017年广州培道初特长生招生工作领导小组'},
          {message:'2017年越秀区初中体育特长生招生方案'},
          {message:'广州市培道中学2017年高中特长生招生方案'},
          {message:'广州市培道中学“培道杯”音乐类第二轮交流活动启事'},
          {message:'2017年高中“培道杯”交流活动'},
          {message:'2017年高一新生报到分组名单'},
          {message:'2016级高一分班名单'},
          {message:'高二分班名单'},
          {message:'2016高一分班表'},
          {message:"2016年上学期高一/高二住宿生名单及住宿注意事项"}
        ]
      }
    }
  }
</script>

