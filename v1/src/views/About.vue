<template>
  <div class="about-image">
    <img alt="about image" src="../assets/about1.png">
    <figure>
  <div class="about-menu">
      <div class="amtitle">
       <p>사업소개 </p>
     </div>
        <router-link to="/about">
            <p id="menu-selected">인사말</p>
            </router-link> 
  <hr>
        <a href="https://sw7up.cbnu.ac.kr/organization/objective">
            <p>사업목표</p>
            </a>
 <hr>
        <a href="https://sw7up.cbnu.ac.kr/organization/vision">
            <p>추진방향</p>
            </a>
 <hr>
        <a href="https://sw7up.cbnu.ac.kr/organization/member">
            <p>조직도</p>
            </a>
 <hr>
        <a href="https://sw7up.cbnu.ac.kr/organization/facility">
            <p>교육시설</p>
            </a>
  <hr>
        <router-link to="/location">
            <p>오시는 길</p>
            </router-link> 
  </div>
      </figure>
 <br>
  <div class="context">
    <h1>인사말</h1>
    <p><router-link to="/">&#127968;</router-link>
    &nbsp;&nbsp;/&nbsp;&nbsp;사업소개&nbsp;&nbsp;/&nbsp;&nbsp;인사말</p>
    <hr>
    <br>
    <p>포스트 코로나를 대비해야 하는 격변의 시대를 맞아 소프트웨어(SW)는 
      더 이상 ICT분야의 전유물이 아닌 새로운 일상의 필수요소가 되었습니다. 개인에게는 
      SW를 이해하고 활용할 수 있는 SW 리터러시(literacy)가 요구되며, 국가는 경쟁력 제고를 위해 
      창의적이고 도전적인 SW핵심인력을 필요로 하고 있습니다.</p>
      <br>
    <p>충북대학교 SW중심대학사업단은 이러한 시대적∙국가적 요구에 대응하기 위해
      과학기술정보통신부 지원을 받아 <strong>‘도전적이며 커뮤니티에 기여하는 
      핵심직무역량을 갖춘 지능 SW 인재양성’</strong>을 
      목표로, 지능형 SW, 산업 AI, 빅데이터, 지능형 IoT, 임베디드 SW, 
      지능로봇 SW 등의 심화트랙을 운영합니다.</p>
       <br>
     <p>"또한, 빅데이터, 보안컨설팅, 스마트자동차공학, 뇌∙인지공학, 공공데이터사이언스, 
       스마트 팩토리, 스마트 전력IT, 스마트 디자인, 스마트 도시 등의 융합과정을
      지원하여 SW융합교육 강화에 기여하고 있습니다."</p>     
      <br>
     <p>차별화된 SW교육을 위해 7-Up SW 교육혁신모델, 산학멘토와 가디언 기반의 산학협력 및
        창업교육, 오픈소스 특화프로그램 등을 지원하고 있습니다.</p>   <br>
      <p>캠퍼스 밖에서는 충청권의 초중등 학생, 청소년, 일반인, 재직자 등을 대상으로 SW 리터러시 강화를 위한
         다양한 프로그램을 온∙오프라인으로 제공하고 있습니다. 충북의 거점대학으로서 
         지역의 지능SW 역량강화를 위해 산업체와 공동연구 및 
          기술지원 체계 구축으로 산업경쟁력 제고에 최선을 다해 노력하고 있습니다.</p> 
           <br>
      <p>꾸준한 준비와 노력으로 새로운 일상을 대응하는 충북대학교 SW중심대학 사업단이 되겠습니다. 감사합니다.
        </p>
        <br>
        <h2 id="representative">충북대학교&nbsp;&nbsp; SW중심대학사업단</h2>      
  </div>
  </div>
  
</template>


<style scoped>

.about-image {
  position: relative;
}
.about-image img {
  padding-top: 5.8em;
  width:100%;
}

.about-menu {
  width: 13em;
  height: 30.5em;
  position: absolute;
  top: 200px;
  left : 12em;
  border: 1px solid gray;
  background-color: white;
  opacity: 75%;
  font-weight: bolder;
}

.about-menu ul {
  list-style: none;
  margin-left:0;
  padding-left:0;
}

.about-menu a {
    text-decoration: none;
};


.amtitle {




}

.amtitle p {

  color: white;
  padding-top:60px;
  padding-bottom:60px;
  margin:0;
  background-color: rgb(3, 40, 114);
    top: 80px;
    opacity: 85%;
    margin: auto;
    font-size: 25px;
}

.about-menu a p {
  text-decoration: none;
  text-align: left;
  padding-left: 1em;
  font-size: 18px;
  margin: 0;
  padding-top: 1em;
  padding-bottom: 1em;
  color: rgb(29, 29, 29);
  font-weight: bolder;
}

.about-menu a p:hover {
  text-decoration: none;
  text-align: left;
  padding-left: 1em;
  font-size: 18px;
  margin: 0;
  padding-top: 1em;
  padding-bottom: 1em;
  color: white;
  background-color: rgb(29, 70, 151);
  font-weight: bolder;
}

#greeting {
  text-decoration: none;
  text-align: left;
  padding-left: 1em;
  font-size: 18px;
  margin: 0;
  padding-top: 1em;
  padding-bottom: 1em;
  color: white;
  background-color: rgb(29, 70, 151);
  font-weight: bolder;
}

hr {
  margin:0;
}

.context {
  margin-left: 30em;
  text-align: left;
  width: 60em;
  line-height: 1.5em;
}

.context p{
  margin : 0;
}

#representative {
  text-align: right;
}

#menu-selected {
  text-decoration: none;
  text-align: left;
  padding-left: 1em;
  font-size: 18px;
  margin: 0;
  padding-top: 1em;
  padding-bottom: 1em;
  color: white;
  background-color: rgb(29, 70, 151);
  font-weight: bolder;
}

* {
  font-family: 'cbnu';

}



</style>