<template>
  <div class="main flex-col flex-x-center flex-y-center">
    <div class="center">
      <!--头部-->
      <my-head/>
      <div class="location flex-row flex-left flex-y-center ">
        <span class="location-inner flex-row flex-space-between">
          <p>您当前的位置：</p>
          <p>科组主页</p>
        </span>
      </div>
      <div class="section-page flex-col flex-y-center">
        <div class="section-page-inner flex-row flex-wrap flex-space-between">
          <div class="img-box1 flex-row  flex-y-center" v-for="(item,index) in items" @click="changes(index)" :class="{'img-box flex-x-center':changeBox==index}">

            <img :src="'../../../static/img/sectionPage/'+item.message+'.jpg'">
          </div>
          <!-- <div v-for="item in items" :class="{'img-box flex-x-center':changeBox!=null}">
            <img  :src="'../../../static/img/sectionPage/'+item[1].message+'.jpg'" >
          </div> -->

          <div>

          </div>
        </div>
      </div>

      <!--底部-->
      <my-bottom/>

    </div>
  </div>

</template>


<script>
  let self;

  export default {
    data() {
      return {
        items: [{
            message: "PE"
          },
          {
            message: "IT"
          },
          {
            message: "art"
          },
          {
            message: "biology"
          },
          {
            message: "chemistry"
          },
          {
            message: "chinese"
          },
          {
            message: "english"
          },
          {
            message: "geography"
          },
          {
            message: "history"
          },
          {
            message: "maths"
          },
          {
            message: "physical"
          },
          {
            message: "politics"
          }
        ],
        changeBox: null,
      };
    },
    created() {

      self = this;
    },
    methods: {
      changes: function (index) {
        if (this.changeBox === null) {
          this.changeBox = index;
        } else {
          this.changeBox = null;
        }
      }
    }
  };

</script>
