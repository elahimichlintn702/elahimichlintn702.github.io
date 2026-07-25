<!DOCTYPE html>
<html lang="zh-CN">

<head>

<meta charset="UTF-8">

<meta name="viewport" content="width=device-width, initial-scale=1.0">


<title>
陈先生 | Live Creator & AI Operator
</title>


<link rel="preconnect" href="https://fonts.googleapis.com">


<style>

/* =========================
基础
========================= */


*{

margin:0;

padding:0;

box-sizing:border-box;

}



html{

scroll-behavior:smooth;

}



body{


font-family:

-apple-system,
BlinkMacSystemFont,
"SF Pro Display",
"PingFang SC",
"Microsoft YaHei",
sans-serif;


background:#fff;


color:#111;


overflow-x:hidden;


}




#particles{


position:fixed;


top:0;


left:0;


width:100%;


height:100%;


z-index:-1;


}







/* =========================
导航
========================= */


.nav{


position:fixed;


top:0;


left:0;


width:100%;


height:72px;


display:flex;


align-items:center;


justify-content:space-between;


padding:0 8%;


background:

rgba(255,255,255,.7);


backdrop-filter:

blur(25px);



z-index:100;


border-bottom:

1px solid rgba(0,0,0,.05);


}



.logo{


font-size:22px;


font-weight:700;


}



.nav nav{


display:flex;


gap:35px;


}



.nav a{


text-decoration:none;


color:#333;


font-size:15px;


}



.mobile-btn{


display:none;


font-size:28px;


}







/* =========================
首页
========================= */


.hero{


height:100vh;


display:flex;


align-items:center;


justify-content:center;


text-align:center;


padding:120px 20px 40px;


background:

radial-gradient(
circle at top,
#fff,
#f7f7f7
);


}



.hero-inner{


max-width:900px;


}




.avatar-box{


width:230px;


height:230px;


margin:auto;


border-radius:50%;


overflow:hidden;


padding:8px;


background:

rgba(255,255,255,.8);



box-shadow:

0 40px 120px rgba(0,0,0,.15);



animation:

floating 5s infinite ease-in-out;


}




.avatar-box img{


width:100%;


height:100%;


object-fit:cover;


border-radius:50%;


}





.name{


margin-top:45px;


font-size:90px;


letter-spacing:-5px;


font-weight:700;


animation:

showName 1.5s ease;


}





.role{


margin-top:25px;


font-size:42px;


line-height:1.15;


font-weight:600;


background:

linear-gradient(
90deg,
#111,
#888
);


-webkit-background-clip:text;


color:transparent;


}



.slogan{


margin-top:35px;


font-size:20px;


line-height:2;


color:#666;


}





.tags{


display:flex;


justify-content:center;


gap:15px;


margin-top:35px;


flex-wrap:wrap;


}



.tags span{


padding:12px 28px;


border-radius:40px;


background:

rgba(255,255,255,.7);


border:

1px solid #eee;


backdrop-filter:

blur(20px);


}





.main-btn{


display:inline-block;


margin-top:45px;


padding:16px 45px;


border-radius:50px;


background:#111;


color:#fff;


text-decoration:none;


transition:.3s;


}



.main-btn:hover{


transform:translateY(-5px);


}







/* =========================
通用区域
========================= */


section{


padding:120px 8%;


}



section h2{


font-size:60px;


letter-spacing:-3px;


margin-bottom:60px;


}







/* =========================
玻璃卡片
========================= */


.glass-box,
.number-card,
.project-card{


background:

rgba(255,255,255,.65);


backdrop-filter:

blur(25px);



border:

1px solid rgba(0,0,0,.05);



box-shadow:

0 30px 80px rgba(0,0,0,.08);


border-radius:35px;


}







/* 数据 */


.numbers{


display:grid;


grid-template-columns:

repeat(4,1fr);


gap:25px;


}



.number-card{


padding:40px;


text-align:center;


}



.number-card h3{


font-size:55px;


}





.number-card p{


color:#777;


margin-top:15px;


}







/* 关于 */


.glass-box{


padding:45px;


line-height:2;


color:#555;


}







/* 技能 */


.skill-list{


display:flex;


gap:15px;


flex-wrap:wrap;


}



.skill-list span{


padding:12px 25px;


background:#f5f5f5;


border-radius:30px;


}







/* =========================
经历
========================= */


.experience-list{


display:grid;


gap:30px;


}



.experience-card{


padding:40px;


}




.experience-card h3{


font-size:28px;


margin-bottom:20px;


}



.experience-card h4{


color:#777;


margin-bottom:20px;


}







/* =========================
项目
========================= */


.project-grid{


display:grid;


grid-template-columns:

repeat(3,1fr);


gap:30px;


}



.project-card{


padding:35px;


transition:.5s;


transform-style:preserve-3d;


overflow:hidden;


}



.project-card:hover{


transform:

translateY(-20px)
rotateX(5deg)
rotateY(-5deg);


}



.project-cover{


height:180px;


border-radius:25px;


background:#f5f5f5;


display:flex;


align-items:center;


justify-content:center;


font-size:30px;


font-weight:700;


letter-spacing:2px;


}




.project-card span{


display:inline-block;


margin-top:25px;


padding:8px 18px;


background:#f5f5f5;


border-radius:30px;


font-size:13px;


}




.project-card h3{


font-size:28px;


margin:20px 0;


}




.project-number{


margin-top:25px;


font-size:25px;


font-weight:700;


}




.detail-btn{


margin-top:25px;


border:none;


background:#111;


color:#fff;


padding:12px 25px;


border-radius:30px;


}



.project-detail{


display:none;


margin-top:25px;


line-height:2;


color:#666;


}



.project-card.active .project-detail{


display:block;


}







/* 联系 */


.contact-box{


font-size:20px;


line-height:2.2;


}





footer{


text-align:center;


padding:40px;


color:#999;


}







/* =========================
动画
========================= */


@keyframes floating{


0%,100%{


transform:translateY(0);


}


50%{


transform:translateY(-20px);


}


}




@keyframes showName{


from{


opacity:0;


transform:translateY(50px);


}



to{


opacity:1;


transform:none;


}



}






/* =========================
手机适配
========================= */


@media(max-width:768px){



.nav{


padding:0 25px;


}



.nav nav{


position:absolute;


top:72px;


left:0;


width:100%;


background:white;


display:none;


flex-direction:column;


padding:30px;


}



.nav nav.active{


display:flex;


}



.mobile-btn{


display:block;


}



.name{


font-size:55px;


}



.role{


font-size:32px;


}



.slogan{


font-size:16px;


}



.numbers{


grid-template-columns:

repeat(2,1fr);


}



.project-grid{


grid-template-columns:

1fr;


}



section h2{


font-size:42px;


}



.avatar-box{


width:180px;


height:180px;


}



}

</style>


</head>



<body>



<!-- 粒子背景 -->

<canvas id="particles"></canvas>





<!-- 顶部导航 -->


<header class="nav">


<div class="logo">

CHEN

</div>



<nav>


<a href="#about">
关于
</a>


<a href="#experience">
经历
</a>


<a href="#projects">
作品
</a>


<a href="#contact">
联系
</a>


</nav>



<div class="mobile-btn">

☰

</div>



</header>








<!-- HERO首页 -->


<section class="hero">



<div class="hero-inner">



<div class="avatar-wrap">


<div class="avatar-box">


<img src="images/avatar.jpg"
alt="陈先生头像">


</div>


</div>





<h1 class="name">


陈先生


</h1>





<h2 class="role">


Live Creator

<br>

&

<br>

AI Operator


</h2>






<p class="slogan">


连接直播生态与人工智能，

<br>

创造数字内容的新增长方式


</p>





<div class="tags">


<span>
直播运营
</span>


<span>
AI工具
</span>


<span>
个人IP
</span>


</div>







<a href="#projects"
class="main-btn">


查看作品


</a>




</div>


</section>









<!-- 数据展示 -->


<section class="numbers">



<div class="number-card">


<h3>
3年
</h3>


<p>
直播行业经验
</p>


</div>





<div class="number-card">


<h3>
10万
</h3>


<p>
单月最高流水
</p>


</div>





<div class="number-card">


<h3>
5.5万
</h3>


<p>
账号粉丝增长
</p>


</div>





<div class="number-card">


<h3>
10万
</h3>


<p>
创业项目盈利
</p>


</div>



</section>









<!-- 关于我 -->


<section id="about">



<h2>
About Me
</h2>




<div class="glass-box">


<p>


我是陈先生，18岁。


<br><br>


拥有3年直播行业实战经验，

1年以上团播主播经验。


<br><br>


熟悉直播全流程：

主播培养、直播内容设计、

用户互动、流量增长。


<br><br>


擅长Kpop、Hiphop舞蹈，

原创编舞以及直播节目效果设计。


<br><br>


熟悉抖音、快手、Bigo等平台运营，

并使用AI工具提升内容效率。


</p>



</div>




</section>









<!-- 技能 -->


<section class="skills-section">



<h2>

Skills

</h2>




<div class="skill-list">


<span>
Live Operation
</span>


<span>
Content Growth
</span>


<span>
AI Tools
</span>


<span>
IP Building
</span>


<span>
PS Design
</span>


<span>
Data Analysis
</span>



</div>



</section>

<!-- 工作经历 -->

<section id="experience">


<h2>

Experience

</h2>



<div class="experience-list">



<div class="experience-card glass-box">


<h3>

重庆星丹文化传媒有限公司

</h3>


<h4>

主播 & 运营

<br>

2023.11 - 至今

</h4>


<p>


负责团播直播内容输出，

直播间气氛打造以及用户互动。


<br><br>


负责账号运营：

<br>

内容策划

<br>

流量测试

<br>

粉丝增长

<br>

用户维护


<br><br>


业绩：

<br>

单月最高流水 ¥100,000

<br>

月均流水 ¥30,000

<br>

单日最高流水 ¥8,000


</p>


</div>








<div class="experience-card glass-box">


<h3>

自媒体账号运营

</h3>


<h4>

2023

</h4>


<p>


独立完成账号定位、

内容策划、拍摄、剪辑、

发布以及数据分析。


<br><br>


2个月：

<br>

账号增长至5.5万粉丝。


</p>


</div>









<div class="experience-card glass-box">


<h3>

信息差创业项目

</h3>


<h4>

2022

</h4>



<p>


发现市场机会，

独立完成项目运营。


<br><br>


2个月盈利近 ¥100,000。


</p>



</div>



</div>



</section>













<!-- 项目作品 -->

<section id="projects">



<h2>

Featured Projects

</h2>




<div class="project-grid">







<!-- 项目1 -->


<div class="project-card glass-box">



<div class="project-cover">

LIVE GROWTH

</div>



<span>

直播运营

</span>



<h3>

直播增长运营系统

</h3>



<p>


从账号定位、

内容设计、

直播运营到商业转化，

打造完整增长体系。


</p>




<div class="project-number">


¥100,000

<br>

最高月流水


</div>



<button class="detail-btn">

VIEW CASE

</button>




<div class="project-detail">


<h4>

项目职责

</h4>


<p>


主播运营

<br>

直播策划

<br>

数据分析

<br>

用户增长


</p>




<h4>

成果

</h4>


<p>

单月最高流水10万元。

</p>



</div>




</div>













<!-- 项目2 -->


<div class="project-card glass-box">



<div class="project-cover">

BIGO LIVE

</div>




<span>

海外直播

</span>




<h3>

海外直播生态运营

</h3>



<p>


研究海外直播平台玩法，

主播培养和用户增长。


</p>



<div class="project-number">


GLOBAL

<br>

LIVE OPERATION


</div>




<button class="detail-btn">

VIEW CASE

</button>




<div class="project-detail">


<h4>

平台

</h4>


<p>

Bigo Live

</p>




<h4>

能力

</h4>


<p>


主播管理

<br>

活动策划

<br>

直播运营

<br>

用户增长


</p>



</div>



</div>














<!-- 项目3 -->


<div class="project-card glass-box">



<div class="project-cover">

CREATOR

</div>



<span>

个人IP

</span>



<h3>

自媒体增长项目

</h3>




<p>


从0开始打造账号，

完成内容增长和粉丝积累。


</p>




<div class="project-number">


55K+

<br>

粉丝


</div>



<button class="detail-btn">

VIEW CASE

</button>





<div class="project-detail">


<h4>

负责内容

</h4>


<p>


账号定位

<br>

选题策划

<br>

视频制作

<br>

数据复盘


</p>



<h4>

成果

</h4>


<p>

2个月达到5.5万粉丝。

</p>



</div>



</div>







</div>



</section>









<!-- 联系方式 -->


<section id="contact">



<h2>

Contact

</h2>



<div class="contact-box glass-box">



<p>

陈先生

</p>



<p>

📞 18198492700

</p>



<p>

主播 / 直播运营 / 新媒体运营

</p>



<p>

揭阳 · 广州 · 深圳 · 杭州

</p>




</div>



</section>







<footer>


© 2026 Chen Portfolio


</footer>





<!-- 第3部分CSS和JS会继续放这里 -->

<script>


// =====================
// 项目详情展开
// =====================


const detailButtons = document.querySelectorAll(".detail-btn");


detailButtons.forEach(button=>{


button.addEventListener("click",()=>{


const card = button.closest(".project-card");


// 切换展开状态

card.classList.toggle("active");



// 修改按钮文字

if(card.classList.contains("active")){


button.innerHTML="CLOSE CASE";


}else{


button.innerHTML="VIEW CASE";

button.innerHTML="VIEW CASE";


});


});

// ==========================
// V4.2 头像3D跟随效果
// ==========================


const avatarBox = document.querySelector(".avatar-box");


if(avatarBox){


avatarBox.addEventListener("mousemove",(e)=>{


const rect = avatarBox.getBoundingClientRect();


const x = e.clientX - rect.left;

const y = e.clientY - rect.top;


const rotateY =
(x / rect.width - 0.5) * 20;


const rotateX =
(y / rect.height - 0.5) * -20;



avatarBox.style.transform =
`
rotateX(${rotateX}deg)
rotateY(${rotateY}deg)
`;



});



avatarBox.addEventListener("mouseleave",()=>{


avatarBox.style.transform =
"rotateX(0deg) rotateY(0deg)";


});


}
</script>






<!-- ESSPSEEK AI助手 -->
<style>
#ai-btn{position:fixed;right:22px;bottom:22px;z-index:9999;background:#111;color:#fff;border:0;border-radius:50px;padding:14px 22px;font-size:16px;box-shadow:0 10px 30px #0002;cursor:pointer}
#ai-box{display:none;position:fixed;right:20px;bottom:80px;width:320px;height:420px;background:#fff;border:1px solid #eee;border-radius:24px;z-index:9999;box-shadow:0 20px 60px #0003;overflow:hidden}
#ai-head{padding:16px;font-weight:700;border-bottom:1px solid #eee}
#ai-chat{height:300px;overflow:auto;padding:15px;font-size:14px}
#ai-input{display:flex;padding:12px;gap:8px}
#ai-input input{flex:1;padding:10px;border-radius:12px;border:1px solid #ddd}
#ai-input button{border:0;border-radius:12px;padding:0 14px;background:#111;color:#fff}
.msg{margin-bottom:10px;line-height:1.5}
</style>
<button id="ai-btn">🤖 ESSPSEEK</button>
<div id="ai-box">
<div id="ai-head">ESSPSEEK AI运营助手</div>
<div id="ai-chat"><div class="msg">AI：你好，我是你的AI运营助手。</div></div>
<div id="ai-input"><input id="ai-text" placeholder="输入问题..."/><button onclick="askESSPSEEK()">发送</button></div>
</div>
<script>
const aiBtn=document.getElementById('ai-btn');
const aiBox=document.getElementById('ai-box');
aiBtn.onclick=()=>aiBox.style.display=aiBox.style.display==='block'?'none':'block';
async function askESSPSEEK(){
 const input=document.getElementById('ai-text');
 const chat=document.getElementById('ai-chat');
 const q=input.value.trim(); if(!q)return;
 chat.innerHTML+=`<div class="msg">你：${q}</div>`;
 input.value='';
 try{
  const res=await fetch('/api/chat',{
   method:'POST',headers:{'Content-Type':'application/json'},
   body:JSON.stringify({message:q,role:'运营官'})
  });
  const data=await res.json();
  chat.innerHTML+=`<div class="msg">AI：${data.reply||data.message||'接口已连接'}</div>`;
 }catch(e){
  chat.innerHTML+=`<div class="msg">AI：请检查ESSPSEEK Gateway接口。</div>`;
 }
 chat.scrollTop=chat.scrollHeight;
}
</script>

</body>


</html>
