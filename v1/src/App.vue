<template>
<div>
<div class="top-menu">
  <div class = "userinfo">
   <router-link id = "login" to="/about">로그인</router-link> &nbsp; &nbsp; &nbsp; &nbsp;
   <router-link id = "register" to="/about">회원가입</router-link> 
</div>
<br>
  <div>
    
    <router-link class = "nav" to="/"><img alt="Vue logo" src="./assets/logo.png"></router-link>
    <router-link  class = "nav" to="/about">사업소개</router-link> 
    <router-link  class = "nav" to="/about">SW교육</router-link> 
    <router-link class = "nav" to="/about">산학협력</router-link>
    <router-link class = "nav" to="/about">SW가치확산</router-link> 
    <router-link class = "nav" to="/about">공지사항</router-link>
    <router-link class = "nav" id="manageproject" to="/about">프로젝트 관리</router-link>
    <br><br>
    <hr>
  </div>
    </div>

   
  <router-view/>
  <br><br>
    <div class="footer">
    <div class="footer-basic">
      <a href="https://sw7up.cbnu.ac.kr/policy/privacy">개인정보처리방침&nbsp;&nbsp;&nbsp;&nbsp;|</a>
      <a href="https://sw7up.cbnu.ac.kr/policy/sitemap">&nbsp;&nbsp;&nbsp;&nbsp;사이트맵&nbsp;&nbsp;&nbsp;&nbsp;|</a> 
      <a href="https://sw7up.cbnu.ac.kr/policy/clean">&nbsp;&nbsp;&nbsp;&nbsp;클린신고센터</a> 
    </div>
    <div class="footer-linklist">
      <form>
      <select onchange="if(this.value) window.open(this.value);">
        <option value="https://www.cbnu.ac.kr">충북대학교</option>
        <option value="http://fole.chungbuk.ac.kr/index.do">창의융합본부</option>
        <option value="https://www.swuniv.kr/">SW중심대학</option>  
      </select>
      </form>
          </div>
    <div class="footer-info">
      <a href="http://kko.to/5XVmbe4f0">충청북도 청주시 서원구 충대로1(개신동) 학연산공동기술연구원(E9동) 742호&nbsp;&nbsp;&nbsp;&nbsp;|</a>
      <a href="tel:043-249-1833"> &#9742;043-249-1833</a>
    </div>
    <div class="footer-copyright">
      <small>© 2020 충북대학교 SW중심대학사업단. All rights reserved.</small>
    </div>

    </div>
</div>
</template>



<style>

.userinfo {

  position: absolute;
  right: 200px;
  z-index: 1;
}

.userinfo a {
text-decoration: none;
color: black;
}

.userinfo a:hover {
  color:blue;
}

#login a:hover {
  color: blue;
}



.nav {
  margin-left: 5em;
  font-size: 1.2em;
  text-decoration: none;
  color: black;
}

#manageproject {
  border: 3px solid;
  border-top: 5px solid;
  border-bottom: 5px solid;
  padding: 2px;
  padding-top: 4px;
  padding-bottom: 4px;
  border-radius: 3px;
  border-width: 2px;;
  border-color: rgb(0, 183, 255);
  color: rgb(0, 183, 255);
  font-size: 1em;
}


@font-face {
    font-family: 'cbnu';
    src: url('/assets/fonts/cbnu.woff2') format('woff2'),
        url('/assets/fonts/cbnu.woff') format('woff');
        font-weight: normal;
        font-style:normal;
        font-display: swap;
}


* {
  font-family: 'cbnu';

}

#app {
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}

.top-menu {
  position: fixed;
  top: 0;
  width: 100%;
  z-index: 2;
  background-color: white;

}

.footer {
  width: 100%;
  height: 10em;
  background-color: rgb(77, 77, 77);
  margin-top: 5em;
}

.footer a {
  text-decoration: none;
  color: white;
}

.footer-basic {
  padding-top: 2em;
  margin-left: 15em;
  width: 20em;
}

.footer-linklist {
  margin-left: 60em;
}

.footer-info {
    padding-top: 2em;
    margin-left: -27.5em;
}
.footer-copyright {
  padding-top: 1em;
  color: rgb(170, 170, 170);
  margin-left: -47em;
}
</style>





