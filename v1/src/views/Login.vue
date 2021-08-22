<template>
  <div class="about-image">
    <img alt="about image" src="../assets/about1.png">
    <figure>
  <div class="about-menu">
      <div class="amtitle">
       <p> 로그인 </p>
     </div>
        <router-link to="/about">
            <p id="menu-selected">로그인</p>
            </router-link> 
  <hr>
        <a href="https://sw7up.cbnu.ac.kr/organization/objective">
            <p>회원가입</p>
            </a>
 <hr>
        <a href="https://sw7up.cbnu.ac.kr/organization/vision">
            <p>추진방향</p>
            </a>
 <hr>
        <a href="https://sw7up.cbnu.ac.kr/organization/member">
            <p>계정 찾기</p>
            </a>
 <hr>
        <a href="https://sw7up.cbnu.ac.kr/organization/facility">
            <p>비밀번호 찾기</p>
            </a>
  </div>
      </figure>
 <br>
  <div class="context">
    <h1>로그인</h1>
    <p><router-link to="/">&#127968;</router-link>
    &nbsp;&nbsp;/&nbsp;&nbsp;사업단회원&nbsp;&nbsp;/&nbsp;&nbsp;로그인</p>
    <hr>
    <br>  <br>
            <form>
            <div id="signin">
                <div class="align-right">
                 <a href="#">아이디 찾기</a>
                <input class="userinfo-input" id="email" name="email" type="email" placeholder="학번/교번 또는 아이디"><br><br>
                </div>
                <div class="align-right">
                 <a href="#">비밀번호 찾기</a>
                <input class="userinfo-input" id="pass" name="pass" type="password" placeholder="비밀번호"><br>
                <br>
                 <input id="keep_login" name="keep_login" type="checkbox" value="Y">
                 <label for="keep_login">로그인 상태 유지</label><br>
                </div>
                <br>
                <button id="login-align-right" type="submit">로그인</button><br>
                <div class="align-left">
                 아직도 계정이 없으신가요?
                 <a href="join_agree.html">회원가입</a><br>
                </div>
            </div>                   
        </form>
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
  height: 27em;
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


#signin {
    width: 10em;
    margin-left: 13em;
}

.userinfo-input {
    width: 35em;
    height: 3em;
    background-color: rgb(209, 242, 255);
    border:0px;
    border-radius:5px;
}

.checkbox-area {
    height:3em;
    width: 30em;
    margin-top:1em;
    padding-left: 21em;
}

.align-right {
        width: 30em;
        text-align: right;
        right: 10em;
}

.align-right a {
            text-decoration: none;
        color: gray;
}

#login-align-right {
    width: 8em;
    height: 3em;
    background-color: rgb(32, 128, 255);
    color: white;
    font-size: 14px;
    border-radius: 5px;
    margin-left: 26em;
}

.align-left {
position:absolute;
width: 30em;
text-align: left;
right: 25em;
bottom: 0.5em;
}

* {
  font-family: 'cbnu';

}



</style>