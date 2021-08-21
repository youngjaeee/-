<template>
  <div class="about-image">
    <img alt="about image" src="../assets/about1.png">
    <figure>
  <div class="about-menu">
      <div class="amtitle">
       <p>사업소개 </p>
     </div>
        <a href="https://sw7up.cbnu.ac.kr/organization/greetings">
            <p>인사말</p>
            </a>
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
        <a href="https://sw7up.cbnu.ac.kr/organization/location">
            <p>오시는 길</p>
            </a>
  </div>
      </figure>
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
  bottom: -22em;
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

hr {
  margin:0;
}

* {
  font-family: 'cbnu';

}



</style>