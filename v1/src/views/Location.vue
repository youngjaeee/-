<template>
  <div class="about-image">
    <img alt="about image" src="../assets/about1.png">
    <figure>
  <div class="about-menu">
      <div class="amtitle">
       <p>사업소개 </p>
     </div>
        <router-link to="/about">
            <p>인사말</p>
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
            <p id="menu-selected">오시는 길</p>
            </router-link> 
  </div>
      </figure>
 <br>
  <div class="context">
    <h1>오시는 길</h1>
    <p><router-link to="/">&#127968;</router-link>
    &nbsp;&nbsp;/&nbsp;&nbsp;사업소개&nbsp;&nbsp;/&nbsp;&nbsp;오시는 길</p>
    <hr>
    <br>
    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2677.246597984334!2d127.45536073368294!3d36.62514379227565!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x356529c6c7ffd017%3A0x4b8649ec6b610e5c!2z7Lap67aB64yA7ZWZ6rWQIO2VmeyXsOyCsOqzteuPmeq4sOyIoOyXsOq1rOybkA!5e0!3m2!1sko!2skr!4v1629608686073!5m2!1sko!2skr" width="960" height="420" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
    
        <br>
    <table border="0" width="800" id="location-info">
	<th>주소</th>
	<th>전화번호</th>
	<tr>
	    <td>충청북도 청주시 서원구 충대로1(개신동) , 학연산공동기술연구원(E9동) 742호</td>
	    <td><a href="tel:043-249-1833"> &#9742;&nbsp;043-249-1833</a></td>
	</tr>
    </table>
  </div>
  <div>
      <div>
      <ul id="transport-select">
          <li><button v-on:click="ShowVal = 1">자가차량</button></li>
          <li><button v-on:click="ShowVal = 2">대중교통</button></li>
      </ul>
      </div>
      <br><br> <br>
      <div id="horizon-line">
      <hr>
      </div>
      <br>
      <div class="location-desc" id="personal-car" v-show="ShowVal == 1">
           
          <strong>경부고속도로 이용시</strong><br>
           ▷&nbsp;청주IC 나와서 왼쪽 청주방향 6.5km 이동 → 산업단지육거리 → 충북대학교 방면 우측도로 500m 이동 → 충북대 정문 도착<br>
           <br>
           <strong>중부고속도로 이용시</strong><br>
            ▷&nbsp;서청주IC 나와서 좌회전(청주방향) 1.5km 이동 → 솔밭공원 사거리 → 시청 방면으로 우회전 200m 이동 후 좌회전 → 1.5km 이동<br>
            &nbsp;&nbsp;→ 산업단지육거리 → 충북대학교 방면 우측도로 500m 이동 → 충북대 정문 도착<br>
            <br>
            <strong>청주-상주간 고속도로 이용시</strong><br>
            ▷&nbsp;청주JC → 경부고속도로 → 남이JC에서 오른쪽 중부고속도로 → 서청주IC 나와서 좌회전(청주방향) 1.5km 이동 → 솔밭공원 사거리<br>
            &nbsp;&nbsp;→ 시청 방면으로 우회전   → 산업단지육거리 → 충북대학교 방면 우측도로 500m 이동 → 충북대 정문 도착
      </div>
      <div class="location-desc" id="public-car" v-show="ShowVal == 2">
          <strong>철도 이용시</strong><br>
           ▷&nbsp;KTX 오송역<br>
           &nbsp;&nbsp; - 오송역 앞에서 청주행(일반511, 517, 520번) 버스 이용
           <br>
            ▷&nbsp;일반철도 : 경부선, 호남선 조치원역<br>
           &nbsp;&nbsp; - 조치원 역 앞에서 청주행(좌석 502번, 일반 511번) 버스 이용
           <br><br>
           <strong>고속버스 이용시</strong><br>
           ▷&nbsp;출발지: 서울, 동서울, 상봉, 대구, 부산, 광주 고속버스 터미널<br>
           ▷&nbsp;도착지: 청주고속버스터미널(가경동)<br>
           ▷&nbsp;시외버스터미널앞 정류장에서 시내버스승차, 충북대학교 입구 정류장 하차 후 도보 이동<br>
           ▷&nbsp;택시 이용 시 약 4,000 ~ 5,000원<br>
            <br>
            <strong>시외버스 이용시</strong><br>
           ▷&nbsp;출발지: 각 도시 시외버스 터미널<br>
           ▷&nbsp;도착지: 청주시외버스터미널(가경동)<br>
           ▷&nbsp;터미널앞 정류장에서 시내버스 승차, 충북대학교 입구 정류장 하차 후 도보 이동<br>
           ▷&nbsp;택시 이용 시 약 4,000 ~ 5,000원<br>
      </div>
  </div>
  </div>
  
</template>

<script>
export default {

name: 'Test',

data: function() {
return {
ShowVal : '1'
}
}
}

</script>


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

#location-info a {
    text-decoration: none;
    color: black;
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

#transport-select {
    list-style: none;
    margin-left: 28em;
}

#transport-select li button {
    float: left;
    margin-right:3em;
    padding: 0.6em;
    text-decoration: none;
    color: rgb(0, 110, 255);
    border : 1px solid lightgray;
    border-radius: 10%;
}

#transport-select li button:active {
    float: left;
    margin-right:3em;
    padding: 0.6em;
    color: black;
    border : 1px solid lightgray;
    border-radius: 10%;
}

.location-desc {
    margin-left: 30em;
    text-align: left;
    line-height: 1.5em;
}

#horizon-line {
    margin-left: 30em;
    width: 60.1em;
}

* {
  font-family: 'cbnu';

}



</style>