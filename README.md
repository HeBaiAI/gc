<!doctype html>
<html>
 <head> 
  <meta charset="UTF-8"> 
  <meta name="viewport" id="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=0"> 
  <!-- MDUI --> 
  <link rel="stylesheet" href="https://unpkg.com/mdui@1.0.2/dist/css/mdui.min.css"> 
  <script src="https://unpkg.com/mdui@1.0.2/dist/js/mdui.min.js"></script> 
  <link rel="shortcut icon" href="favicon.png" type="image/x-icon"> 
  <title>赫晖</title>
   
  <script src="index.js"></script> 
  <script src="index.js"></script> 
  <script src="https://unpkg.com/vue@3/dist/vue.global.prod.js"></script> 
  <link rel="stylesheet" type="text/css" href="theme.css"> 
  <meta name="viewport" content="width=device-width, initial-scale=1.0"> 
  <script>
    function activeTab1() {
        document.getElementById('tabIcon1').classList.add("mdui-color-blue-200");
        document.getElementById('tabIcon1').style.padding = "4px 24px";
        document.getElementById('tabIcon2').classList.remove("mdui-color-blue-200");
        document.getElementById('tabIcon2').style.padding = "4px 4px";
        document.getElementById('tabIcon3').classList.remove("mdui-color-blue-200");
        document.getElementById('tabIcon3').style.padding = "4px 4px";
        document.getElementById('tabIcon4').classList.remove("mdui-color-blue-200");
        document.getElementById('tabIcon4').style.padding = "4px 4px";
    }
    }

    function activeTab2() {
        document.getElementById('tabIcon3').classList.remove("mdui-color-blue-200");
        document.getElementById('tabIcon3').style.padding = "4px 4px";
        document.getElementById('tabIcon2').classList.add("mdui-color-blue-200");
        document.getElementById('tabIcon2').style.padding = "4px 24px";
        document.getElementById('tabIcon1').classList.remove("mdui-color-blue-200");
        document.getElementById('tabIcon1').style.padding = "4px 4px";
        document.getElementById('tabIcon4').classList.remove("mdui-color-blue-200");
        document.getElementById('tabIcon4').style.padding = "4px 4px";
    
    }

    function activeTab3() {
        document.getElementById('tabIcon3').classList.add("mdui-color-blue-200");
        document.getElementById('tabIcon3').style.padding = "4px 24px";
        document.getElementById('tabIcon2').classList.remove("mdui-color-blue-200");
        document.getElementById('tabIcon2').style.padding = "4px 4px";
        document.getElementById('tabIcon1').classList.remove("mdui-color-blue-200");
        document.getElementById('tabIcon1').style.padding = "4px 4px";
        document.getElementById('tabIcon4').classList.remove("mdui-color-blue-200");
        document.getElementById('tabIcon4').style.padding = "4px 4px";
    } 
    }
    activeTab1();
</script>
 </head>
   
 <body id="v1" class="mdui-theme-primary-indigo mdui-theme-accent-blue" style="padding-top: 150px"> 
  <div id="app" class="mdui-container"> 
   <div id="v2" class="mdui-appbar mdui-appbar-fixed"> 
    <header id="v3" class="mdui-appbar mdui-appbar-fixed mdui-appbar-inset mdui-shadow-0"> 
     <div id="v4" class="mdui-toolbar  mdui-color-blue-100"> 
      <a id="v5" class="mdui-btn mdui-btn-icon waves-circle toolbar-btn" mdui-drawer="{target: '#drawer', swipe: true}"> <i id="v6" class="mdui-icon material-icons">menu</i> </a> 
      <span id="v7" class="mdui-typo-headline"></span> 
      <span id="v8" class="mdui-typo-title"> </span> 
      <div id="v9" class="mdui-toolbar-spacer"></div> 
      <a id="v10" href="javascript:window.open('http://192.168.1.70:8080');" class="mdui-btn mdui-btn-icon"><i id="v11" class="mdui-icon material-icons">link</i></a> 
      <a id="v12" href="javascript:mdui.webtools-static-lert('欢迎使用本网站，群号：763742667<br>','关于')" class="mdui-btn mdui-btn-icon"><i id="v13" class="mdui-icon material-icons">info_outline</i></a> 
     </div> 
     
     <div id="v14" class="mdui-tab mdui-tab-centered mdui-color-blue-100" mdui-tab> 
      <a id="v15" href="#example-1" class="mdui-ripple mdui-ripple-white" onclick="activeTab1()"> <i class="mdui-icon material-icons" id="tabIcon1">apps</i> <label id="v16">主页</label> </a> 
      <a id="v17" href="#example-2" class="mdui-ripple mdui-ripple-white" onclick="activeTab2()"> <i class="mdui-icon material-icons" id="tabIcon2">beach_access</i> <label id="v18">视频</label> </a> 
      <a id="v19" href="#example-3" class="mdui-ripple mdui-ripple-white" onclick="activeTab3()"> <i class="mdui-icon material-icons" id="tabIcon3">business_center</i> <label id="v20">软件库</label> </a> 
      <a id="v21" href="#example-4" class="mdui-ripple mdui-ripple-white" onclick="activeTab3()"> <i class="mdui-icon material-icons" id="tabIcon4">business_center</i> <label id="v22">GM</label> </a> 
     </div> 
    </header> 
   </div> 
   
   <div class="mdui-drawer mdui-drawer-full-height mdui-color-theme-blue" id="drawer"> 
    <!-- 顶部图片 --> 
    <div id="v23" class="chtb"> 
     <img id="v24" src="https://ldbbs.ldmnq.com/bbs/topic/attachment/2023-2/76aed787-5fa3-4e8c-8b89-b1e16b9f22c5.jpg" style="aspect-ratio: 1225/597;width: 100%;"> 
    </div> 
    <ul id="v25" class="mdui-list" mdui-collapse="{accordion: true}" style="padding: 8px;"> 
     <!-- 侧滑布局 --> 
     <li id="v26" v-if="config &amp;&amp; config.drawer" v-for="item in config.drawer.items" class="mdui-collapse-item mdui-collapse-item"> 
      <ul id="v27" class="mdui-list"> 
       <a id="v28" href="https://www.123pan.com/s/1Ao8Vv-VsqBH" class="mdui-list-item mdui-ripple"> <i id="v29" class="mdui-list-item-icon mdui-icon material-icons">move_to_inbox</i> 
        <div id="v30" class="mdui-list-item-content">
         下载
        </div> </a> 
       <a id="v31" href="https://jq.qq.com/?_wv=1027&amp;k=EhZW7rBP" class="mdui-list-item mdui-ripple"> <i id="v32" class="mdui-list-item-icon mdui-icon material-icons">send</i> 
        <div id="v33" class="mdui-list-item-content">
         群聊
        </div> </a> 
       <a id="v34" href="https://ldbbs.ldmnq.com/bbs/topic/attachment/2023-2/ba338cc6-42b6-4fa6-a8fc-3f19a31299ea.jpg" class="mdui-list-item mdui-ripple"> <i id="v35" class="mdui-list-item-icon mdui-icon material-icons">delete</i> 
        <div id="v36" class="mdui-list-item-content">
         赞助
        </div> </a> 
       <a id="v37" href="https://ldbbs.ldmnq.com/bbs/topic/attachment/2023-2/a9735dcb-93e1-45f4-8420-7e63a828f003.jpg" class="mdui-list-item mdui-ripple"> <i id="v38" class="mdui-list-item-icon mdui-icon material-icons">error</i> 
        <div id="v39" class="mdui-list-item-content">
         作者
        </div> </a> 
       <a id="v40" href="https://www.123pan.com/s/1Ao8Vv-VsqBH" class="mdui-list-item mdui-ripple"> <i id="v41" class="mdui-list-item-icon mdui-icon material-icons"></i> 
        <div id="v42" class="mdui-list-item-content">
         赫晖影视
        </div> </a> 
      </ul> </li>
    </ul>   
   </div> 
   
   <div id="v43" class="mdui-container"> 
    <div id="example-1" class="mdui-p-a-2"> 
     <div id="v44" class="mdui-row mdui-typo"> 
      <div id="v45" class="mdui-col-sm-6 mdui-col-md-4"> 
       <div id="v46" class="mdui-card"> 
        <div id="v47" class="mdui-card-header"> 
         <img id="v48" class="mdui-card-header-avatar" src="https://ldbbs.ldmnq.com/bbs/topic/attachment/2023-2/9b66a125-0525-4fb8-af48-ad0d535b5ef1.jpg"> 
         <div id="v49" class="mdui-card-header-title">
          赫晖漫剪

         </div> 
         <div id="v50" class="mdui-card-header-subtitle">
          人生犹如一场戏，明知是假的，但是你还是陪他走到最后
         </div> 
        </div> 
        <div id="v51" class="mdui-card-media"> 
         <img id="v52" src="https://ldbbs.ldmnq.com/bbs/topic/attachment/2023-2/57235b53-b15f-4f63-a8f6-43ec56dacf94.gif"> 
         <div id="v53" class="mdui-card-menu"> 
          <button id="v54" class="mdui-btn mdui-btn-icon mdui-text-color-white"><i id="v55" class="mdui-icon material-icons">share</i></button> 
         </div> 
        </div> 
        <div id="v56" class="mdui-card-primary"> 
         <div id="v57" class="mdui-card-primary-title">
          感慨
         </div> 
         <div id="v58" class="mdui-card-primary-subtitle">
          赫晖日
         </div> 
        </div> 
        <div id="v59" class="mdui-card-content">
         「人本来就不是什么深情的动物，根据科学家的研究证明了这项事实，如果在婚礼上你看到别人说我会爱你一辈子，那都是假的，所以男的为什么先死，都已经把下辈子给提前预约了」
         <!---->
						</div>
						<!-- 音乐播放器跨站开始 -->
		<link rel="stylesheet" href="css/player.css">
       <div id="QPlayer">  
          <div id="pContent">
	         <div id="player">
	         	<span class="cover"></span>
	             	<div class="ctrl">
			<div class="musicTag marquee">
				<strong>Title</strong>
				 <span> - </span>
				<span class="artist">Artist</span>
			</div>
			<div class="progress">
				<div class="timer left">0:00</div>
				<div class="contr">
					<div class="rewind icon"></div>
					<div class="playback icon"></div>
					<div class="fastforward icon"></div>
				</div>
				<div class="right">
					<div class="liebiao icon"></div>
				</div>
			</div>
		</div>
	</div>
	 <div class="ssBtn">
	   <div class="adf"></div>
    </div>
</div>
    <ol id="playlist"></ol>
</div>
   <script src="js/jquery.min.js"></script>
   <script src="js/jquery.marquee.min.js"></script>
<script>
var	playlist = [
{title: "网易热歌榜",artist: "随机音乐",mp3: "https://api.uomg.com/api/rand.music?sort=热歌榜&format=mp3",cover: "http://ccwj.l-api.com/files/2022/10/25/IMG_20221024_095846.png",},];
	    var isRotate = true;<!--图片旋转-->
	    var autoplay = true;<!--自动播放-->
</script>
    <script src="js/player.js"></script>
  <script>
     function bgChange(){
     	var lis= $('.lib');
    	for(var i=0; i<lis.length; i+=2)
    	lis[i].style.background = 'rgba(246, 246, 246, 0.5)';
        }
        window.onload = bgChange;
   </script>
<!-- 音乐播放器跨站结束 -->
        </div> 
        <div id="v60" class="mdui-card-actions"> 
         <button id="v61" class="mdui-btn mdui-ripple" onclick="mdui.snackbar('就是一辈子都当单身狗算了')">或许我可以给你一些信息提示</button> 
         <button id="v62" class="mdui-btn mdui-ripple" onclick="window.open('https://v.kuaishou.com/Hel6KW 看了这么多快手，还是「赫晖漫剪」最好玩了！ 复制此消息，打开【快手极速版】直接观看！')">快手主页</button> 
        </div> 
        

       </div> 
      </div> 
     </div> 
    </div> 
    <div id="example-2" class="mdui-p-a-2"> 
     <div id="v63" class="mdui-typo"> 
  

       
       <br id="v92"> 
       <div id="v93" class="mdui-table-fluid"> 
        <meta id="v98" charset="utf-8" name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no">
        <title id="v99">WebCat</title>
        <link id="v100" rel="stylesheet" href="https://unpkg.com/swiper@8/swiper-bundle.css">
        <link id="v101" rel="stylesheet" href="https://unpkg.com/swiper@8/swiper-bundle.min.css">
        <div id="v104" class="swiper mySwiper"> 
         <div id="v105" class="swiper-wrapper"> 
          <div id="v106" class="swiper-slide"> 
           <div id="v107" class="spk"> 
            <video id="v108" width="100%" height="100%" poster="" preload="auto" controls="controls"> 
             <source id="v109" src="https://alimov2.a.kwimgs.com/upic/2023/02/11/00/BMjAyMzAyMTEwMDMzNTRfNDk0MjkyMzA0Xzk1OTI5ODY0MDI3XzJfMw==_b_B56cda720d6f2fb58a9049c7bb76aa87a.mp4?clientCacheKey=3xwbfk69772stwa_b.mp4&amp;tt=b&amp;di=7925590b&amp;bp=10000" type="video/mp4"> 
            </video> 
           </div> 
          </div> 
         </div>
        </div>
        <title id="v111">WebCat</title>
        <link id="v112" rel="stylesheet" href="https://unpkg.com/swiper@8/swiper-bundle.css">
        <link id="v113" rel="stylesheet" href="https://unpkg.com/swiper@8/swiper-bundle.min.css">
        <div id="v116" class="swiper mySwiper"> 
         <div id="v117" class="swiper-wrapper"> 
          <div id="v118" class="swiper-slide"> 
           <div id="v119" class="spk"> 
            <video id="v120" width="100%" height="100%" poster="" preload="auto" controls="controls"> 
             <source id="v121" src="https://txmov2.a.kwimgs.com/upic/2023/02/03/18/BMjAyMzAyMDMxODU1NThfMTU0ODI1MDQ3Nl85NTM1MjIxOTk0NF8yXzM=_b_B7720a071ffeebd824c185a12120b5139.mp4?clientCacheKey=3xre43hcthq3uzi_b.mp4&amp;tt=b&amp;di=7925590b&amp;bp=10000"> 
                </video> 
           </div> 
          </div> 
         </div>
        </div>
       <br id="v92"> 
       <div id="v93" class="mdui-table-fluid"> 
        <meta id="v98" charset="utf-8" name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no">
        <title id="v99">WebCat</title>
        <link id="v100" rel="stylesheet" href="https://unpkg.com/swiper@8/swiper-bundle.css">
        <link id="v101" rel="stylesheet" href="https://unpkg.com/swiper@8/swiper-bundle.min.css">
        <div id="v104" class="swiper mySwiper"> 
         <div id="v105" class="swiper-wrapper"> 
          <div id="v106" class="swiper-slide"> 
           <div id="v107" class="spk"> 
            <video id="v108" width="100%" height="100%" poster="" preload="auto" controls="controls"> 
             <source id="v109" src="https://alimov2.a.kwimgs.com/upic/2023/02/07/18/BMjAyMzAyMDcxODQyNTJfMjQwNjk2NjQ5Xzk1NjkzMjIwNzE1XzJfMw==_b_B42c25fb300768226610478d53992db4f.mp4?clientCacheKey=3xvw35fhpy4gh7c_b.mp4&amp;tt=b&amp;di=7925590b&amp;bp=10000"> 
            </video> 
           </div> 
          </div> 
         </div>
        </div>
            </tbody>
                            </table>
                        </div>
                    </div>
                </div>
             
           
          </div>
          </div> 
               <div id="example-3" class="mdui-p-a-2">
                <div class="mdui-typo">
                    
                    <button class="mdui-btn mdui-color-theme-accent mdui-ripple" onclick="window.open('https://www.mdui.org/docs/panel')">下载赫晖商店</button>
                    <div style="margin-top: 50px">
                        <div class="mdui-panel mdui-panel-popout" mdui-panel>
                            <div class="mdui-panel-item">
                                <div class="mdui-panel-item-header">
                                    <div class="mdui-panel-item-title">网站推广</div>
                                    <div class="mdui-panel-item-summary"></div>
                                    <i class="mdui-panel-item-arrow mdui-icon material-icons">keyboard_arrow_down</i>
                                </div>
                                <div class="mdui-panel-item-body">
                                    <p>匿名聊天室</p>
                                    <id="v1"href="没有"
                                    <p>密语岛</p>
                                    <id="v2"href="http://xia.xiaocha.fun/myd/">
                                    <p>今天吃什么</p>
                                    <id="v3">
                                    <p>空</p>
                                    <p>短信弹出</p>
                                    <id="v4">
                                    <p>表白墙</p>
                                    <id="v5">
                                    <div class="mdui-panel-item-actions">
                                        <button class="mdui-btn mdui-ripple">cancel</button>
                                        <button class="mdui-btn mdui-ripple">save</button>
                                        <href="http://xia.xiaocha.fun/myd/">
                                        
                                    </div>
                                </div>
                            </div>
                            <div class="mdui-panel-item">
                                <div class="mdui-panel-item-header">
                                    <div class="mdui-panel-item-title">外版软件</div>
                                    <i class="mdui-panel-item-arrow mdui-icon material-icons">keyboard_arrow_down</i>
                                </div>
                                <div class="mdui-panel-item-body">
                                    <p>小蓝鸟</p>
                                    <p>ig</p>
                                    <p>yt</p>
                                    <p>f</p>
         <                           <p>谷歌</p>
                                    <p>纸飞机</p>
                                    <div class="mdui-panel-item-actions">
                                        <button class="mdui-btn mdui-ripple">cancel</button>
                                        <button class="mdui-btn mdui-ripple">save</button>
                                    </div>
                                </div>
                            </div>
                            <div class="mdui-panel-item">
                                <div class="mdui-panel-item-header">
                                    <div class="mdui-panel-item-title">代做</div>
                                    <div class="mdui-panel-item-summary"></div>
                                    <div class="mdui-panel-item-summary"></div>
                                    <i class="mdui-panel-item-arrow mdui-icon material-icons">keyboard_arrow_down</i>
                                </div>
                                <div class="mdui-panel-item-body">
                                    <p>代做网站</p>
                                    <p>代剪视频</p>
                                    <p>代做小程序</p>
                                    <p>帮搭建网站</p>
                                    <p>代做软件</p>
                                    <p>代做脚本</p>
                                    <div class="mdui-panel-item-actions">
                                        <button class="mdui-btn mdui-ripple">cancel</button>
                                        <button class="mdui-btn mdui-ripple">save</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
</body>

          
          
          
          <script src="https://cdn.bootcdn.net/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
		<script src="js/Mouse.js"></script><!-- 点击烟花特效 -->
  </div> 
     </div> 
    </div>   
          <div id="example-4" class="mdui-p-a-2"> 
  
      <div class="mdui-list">

  <label class="mdui-list-item mdui-ripple">
    <div class="mdui-list-item-avatar">
      <img src="https://ldbbs.ldmnq.com/bbs/topic/attachment/2023-2/57235b53-b15f-4f63-a8f6-43ec56dacf94.gif"/>
    </div>
    <div class="mdui-list-item-content">HeBai</div>
    <div class="mdui-checkbox">
      <input type="checkbox" checked/>
      <i class="mdui-checkbox-icon"></i>
    </div>
  </label>
  <div class="mdui-card">
  <div class="mdui-card-media">
    <img src="https://ldbbs.ldmnq.com/bbs/topic/attachment/2023-2/50ec06de-8735-468a-bfdd-10c073f8c3a0.jpg"/>
  </div>
  <div class="mdui-card-actions mdui-card-actions-stacked">
    <button class="mdui-btn mdui-ripple">GM</button>
    <button class="mdui-btn mdui-ripple">13号站</button>
    <button class="mdui-btn mdui-ripple">1号站</button>
    <button class="mdui-btn mdui-ripple">原神</button>
    <button class="mdui-btn mdui-ripple">6号站</button>
    <button class="mdui-btn mdui-ripple">9号站</button>
  </div>
</div>
