<template>
  <div id="userpage" class="">
    <meta http-equiv="X-UA-Compatible" content="IE=edge"/>
    <meta http-equiv="content-type" content="text/html; charset=utf-8"/>
    <!--<link href="files/用户界面/styles.css" type="text/css" rel="stylesheet"/>-->
      <!-- Unnamed (矩形) -->

    <div id="u0" class="ax_default box_1">
      <img id="u0_img" class="img " src="../assets/images/用户界面/regen/u0.svg"/>
      <div id="u0_text" class="text " style="display:none; visibility: hidden">
        <p></p>
      </div>
    </div>

    <!-- Unnamed (矩形) -->
    <div id="u1" class="ax_default box_1">
      <img id="u1_img" class="img " src="../assets/images/用户界面/regen/u1.svg"/>
      <div id="u1_text" class="text " style="display:none; visibility: hidden">
        <p></p>
      </div>
    </div>

    <!-- Unnamed (图片 ) -->
    <div id="u2" class="ax_default image">
      <img id="u2_img" class="img " src="../assets/images/用户界面/regen/u2.svg"/>
      <div id="u2_text" class="text " style="display:none; visibility: hidden">
        <p></p>
      </div>
    </div>

    <!-- Unnamed (矩形) -->
    <div id="u3" class="ax_default _一级标题">
      <div id="u3_div" class=""></div>
      <div id="u3_text" class="text ">
        <p><span>User Name</span></p>
      </div>
    </div>

    <!-- Unnamed (矩形) -->
    <div id="u4" class="ax_default _三级标题">
      <div id="u4_div" class=""></div>
      <div id="u4_text" class="text">
        <p><span>Themes I have published</span></p>
      </div>
    </div>

    <!-- Unnamed (矩形) -->
    <div id="u5" class="ax_default _三级标题">
      <div id="u5_div" class=""></div>
      <div id="u5_text" class="text ">
        <p><span>Messages</span></p>
      </div>
    </div>

    <!-- Unnamed (内联框架) -->
    <div id="u6" class="ax_default">
      <iframe id="u6_input" scrolling="auto" frameborder="1" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
    </div>

    <!-- Unnamed (矩形) -->
    <div id="u7" class="ax_default _三级标题">
      <div id="u7_div" class=""></div>
      <div id="u7_text" class="text ">
        <p><span>Themes I have joined</span></p>
      </div>
    </div>

    <!-- Unnamed (矩形) -->
    <div id="u8" class="ax_default _二级标题">
      <div id="u8_div" class=""></div>
      <div id="u8_text" class="text " style="display:none; visibility: hidden">
        <p></p>
      </div>
    </div>

    <!-- userpot (组合) -->
    <div id="u9" class="ax_default" data-label="userpot" data-left="117" data-top="325" data-width="610" data-height="126" v-for='item in topicList'>

      <!-- theme (矩形) -->
      <div id="u10" class="ax_default _二级标题" data-label="theme">
        <div id="u10_div" class=""></div>
        <div id="u10_text" class="text ">
          <p><span>{{item.context}}</span></p>
        </div>
      </div>

      <!-- Unnamed (图片 ) -->
      <div id="u11" class="ax_default image">
        <img id="u11_img" class="img " src="../assets/images/用户界面/regen/u11.svg"/>
        <div id="u11_text" class="text " style="display:none; visibility: hidden">
          <p></p>
        </div>
      </div>

      <!-- reply (矩形) -->
      <div id="u12" class="ax_default label" data-label="reply">
        <div id="u12_div" class=""></div>
        <div id="u12_text" class="text ">
          <p><span>2,808 Reply</span></p>
        </div>
      </div>

      <!-- Unnamed (矩形) -->
      <div id="u13" class="ax_default _文本段落">
        <div id="u13_div" class=""></div>
        <div id="u13_text" class="text ">
          <p><span>{{item.description}}</span></p>
        </div>
      </div>

      <!-- username (矩形) -->
      <div id="u14" class="ax_default label" data-label="username">
        <div id="u14_div" class=""></div>
        <div id="u14_text" class="text ">
          <p><span>Name_of_Manager</span></p>
        </div>
      </div>

      <!-- Unnamed (形状) -->
      <div id="u15" class="ax_default icon">
        <img id="u15_img" class="img " src="../assets/images/用户界面/regen/u15.svg"/>
        <div id="u15_text" class="text " style="display:none; visibility: hidden">
          <p></p>
        </div>
      </div>

      <!-- hots (矩形) -->
      <div id="u16" class="ax_default label" data-label="hots">
        <div id="u16_div" class=""></div>
        <div id="u16_text" class="text ">
          <p><span>3500</span></p>
        </div>
      </div>

      <!-- time (矩形) -->
      <div id="u17" class="ax_default label" data-label="time">
        <div id="u17_div" class=""></div>
        <div id="u17_text" class="text ">
          <p><span>{{item.date | format('MM-dd hh:mm')}}</span></p>
        </div>
      </div>

      <!-- topic (矩形) -->
      <div id="u18" class="ax_default label" data-label="topic">
        <div id="u18_div" class=""></div>
        <div id="u18_text" class="text ">
          <p><span>{{item.tag}}</span></p>
        </div>
      </div>

      <!-- delete (形状) -->
      <div id="u19" class="ax_default icon" data-label="delete">
        <img id="u19_img" class="img " src="../assets/images/用户界面/regen/delete_u19.svg" @click="deletepot"/>
        <div id="u19_text" class="text " style="display:none; visibility: hidden">
          <p></p>
        </div>
      </div>
    </div>

    <!-- Unnamed (形状) -->
    <div id="u20" class="ax_default icon">
      <img id="u20_img" class="img " src="../assets/images/用户界面/regen/u20.svg"/>
      <div id="u20_text" class="text " style="display:none; visibility: hidden">
        <p></p>
      </div>
    </div>

    <!-- Unnamed (形状) -->
    <div id="u21" class="ax_default icon">
      <img id="u21_img" class="img " src="../assets/images/用户界面/regen/u21.svg"/>
      <div id="u21_text" class="text " style="display:none; visibility: hidden">
        <p></p>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    data(){
      return{
        topicList:[],
        user:[{token:'',username:'',commentid:''}],
      }
    },
    methods:{
      getpersonalcomment:async function(){
        await this.$axios.get("comment/getPersonalComment",{//该功能未实现
          token:this.token,
        });
      },
      deletepot:async function(){
        var ret = await this.$axios.post("comment/deleteComment",{
          token:this.token,
          commentid:this.commentid,
        }).then(function (response) {
          console.log(response)})
          .catch(function (error) {
            console.log(error.response);
          });
        console.log("删除该主题帖成功");
      },
      getusertopic:async function(){
        var ret=await this.$axios.get("topic/getPersonalTopic",{
          token:this.token,
        }).then(function (response) {
          console.log(response)})
          .catch(function (error) {
            console.log(error.response);
          });
        this.topicList=ret.data.topicList;
      }
    },
    mounted:function(){
      this.getusertopic();
    }
}


</script>

<style scoped>
@import '../assets/files/用户界面/styles.css';
</style>
