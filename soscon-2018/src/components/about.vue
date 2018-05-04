<template>
  <div>
    <div style="width: 80%;margin: 0 auto;">
      <div>
        <div style="display: inline-block;text-align: center;margin-top: 135px">
          <!--<p style="background-color: black;color: white;width: 260px;height: 65px;font-size: x-large" >GNOME.Asia<span style="color:#66ccff;">18</span></p>-->
        <h4 style="background-color: black;color: white;padding: 20px 20px;">GNOME.Asia<span style="color: #66ccff"> 2018</span></h4>
        </div>
        <p style="font-weight: 700;font-size: x-large">————</p>
        <p style="font-weight: 600;font-size: large">GNOME.Asia</p>
        <p>GNOME基金會亞洲委員會在2008年成立，旨在通過舉辦GNOME.Asia亞洲峰會在亞洲地區推廣GNOME項目以及自由開源軟體的理念。GNOME.Asia 峰會與 GUADEC 峰會和 Boston 峰會一起成為了 GNOME 基金會每年的全球三大活動。此前的 GNOME.Asia 分別在北京、越南胡志明、台北、印度班加羅爾、香港和韓國首爾、印尼雅加達和重慶舉辦。如果您有任何建議或聯繫的必要，請發送郵件至 asia-summit-list@gnome.org 取得聯絡。
        </p>
        <p style="font-weight: 600;font-size: large">年会展望</p>
        <p>GNOME.Asia Summit 2018 将于 2018 年 8 月 11 日 - 12 日在台北举办，来自全国各地的学生届时将齐聚一堂，想必是一场技术与思考的饕餮盛宴！<br/>我们也希望GNOME.Asia所聚集而成的社群会作为一个长期的舞台，活跃在各地，成为交流技术、开放讨论的平台，使得开源理念能够在社群中茁壮成长。<br/>会议期间希望学生能积极交流，让学生站上舞台，展示诞生在实验室里的创想，分享蕴含在编码中的激情，畅聊属于开源理念的未来。也期待参会者能继续发挥自己的影响力，让周围更多的人为开源做贡献。</p>

      </div>
      <div> 
        <p style="font-weight: 700;font-size: x-large">————</p>
        <p style="font-weight: 700;font-size: large;display: inline;margin-right: 20px">举办时间：<span style="font-weight: normal">2018年8月11-12日</span></p>
        <p style="font-weight: 700;font-size: large;display: inline">地点:<span style="font-weight: normal">台灣科技大學</span></p>
      </div>
      <div style="margin-top: 2%;margin-bottom: 50px" >
        <iframe v-bind:width="mapWidth" height="500" frameborder="0" scrolling="no" marginheight="0" marginwidth="0" src="https://www.openstreetmap.org/export/embed.html?bbox=106.45307779312135%2C29.56162451639962%2C106.48067235946656%2C29.574968703557974&amp;layer=mapnik&amp;marker=29.56830242911509%2C106.46686649270123" style="border: 1px solid black"></iframe><br/><small><a href="https://www.openstreetmap.org/?mlat=29.5683&amp;mlon=106.4669#map=16/29.5683/106.4669&amp;layers=N">查看更大的地图</a></small>
      </div>
    </div>
    <div style="width: 80%; left: 0;right: 0;margin: 50px auto 10px auto;overflow: hidden;">
      <span style="font-size: small;color: gray">畅想未来，拥抱开源</span>
      <span class="foot" style="margin-left: 10px">Attending us</span>
      <span class="foot" style="margin-left: 10px">Follow us</span>
      <span class="foot">About us</span>
      <hr style="clear: both"/>
      <span style="font-size: small;color: gray;">Copyright &copy; 2018 GNOME.Asia Summit</span>
      <i class="iconfont icon" style="margin-left: 10px">&#xe8d0;</i>
      <i class="iconfont icon" style="margin-left: 10px">&#xe660;</i>
      <i class="iconfont icon">&#xe8db;</i>
    </div>
  </div>
</template>

<script>
    export default {
        name: "about",
        data(){
          return {
            center: {lng: 0, lat: 0},
            zoom: 3,
            aboutUsWidth: '100px'
          }
        },
      computed:{
          w_screen:function(){
            return document.documentElement.clientWidth
          },
          mapWidth:function () {
              return this.w_screen / 1.26 + 'px'
            }

      },

    }


</script>

<style scoped>
  body{
    font-size: 1rem;
  }
</style>
