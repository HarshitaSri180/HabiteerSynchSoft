<template>
  <!-- saven  -->

  <div class="container bg-blue p-3 my-3 rounded-4">
    <div class="position-relative overflow-hidden p-3 p-md-5 m-md-3 text-center">
      <div class="col-12 mx-auto my-3">
        <h1 class=" ">Ever wondered what others think of you?</h1>
        <p class="lead fw-normal mt-5">
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. Facere esse
          consectetur sequi ex quaerat ut, eius exercitationem sapiente hic
          tempora.
        </p>
        <PageLink to="/register" class="btn btn-lg btn-outline-primary mt-5">
          Lorem</PageLink>
      </div>
      <div class="product-device shadow-sm"></div>
      <div class="product-device product-device-2 shadow-sm"></div>
    </div>

    <!-- timeline   -->

    <div class="containe" >

      <ul class="timeline mx-auto">
        <li class="nn">
         
        </li>
        <div class="SecImg"></div>
        
        <li class="Secondlist">  </li>
        <div class="SecImg"></div>
        <li> </li>
      </ul>
    </div>
    <!-- timeline text starts here -->
    <div class="container">
    <div class="row text">
      <div class="col-4 text-center">
        Lorem ipsum dolor sit, amet consectetur adipisicing elit.  voluptas aliquam, architecto in sit omnis eaque iusto, laborum ips
      </div>
      <div class="col-4 text-center">
    Lorem ipsum dolor sit, amet consectetur adipisicing elit. voluptas aliquam, architecto in sit omnis eaque iusto, laborum ips
      </div>
      <div class="col-4 text-center">
        Lorem ipsum dolor sit, amet consectetur adipisicing elit.  voluptas aliquam, architecto in sit omnis eaque iusto, laborum ips
      </div>
    </div>
     <!-- timeline text ends here -->
  </div>
    <!-- second timeline 
    <div class="contai mx-auto">
      <ul class="mx-auto">
        <li class="SecondTimeline"><span>Classic</span></li>
        <div class="SecImgg"></div>
        <li class="SecondTimeline"><span>The Burning Crusade</span></li>
        <div class="SecImgg"></div>
        <li class="SecondTimeline"><span>Wrath of </span></li>
        <div class="SecImgg"></div>
        <li class="SecondTimeline"><span>Cataclysm</span></li>
      </ul>
    </div> -->
    <!-- second timeline  -->

    <!-- Content you want to fade in goes here -->
  </div>

  <!-- timeline  -->
</template>
<style scoped>
h2 {
  color: rgb(52, 52, 52);
  font-size: 32px;
  margin: 0 0 10px 0;
}

h3 {
  color: red;
  font-size: 16px;
  margin: 0 0 5px 0;
}

p {
  color: rgb(52, 52, 52);
  font-size: 20px;
  margin: 0 0 20px 0;
}

body,
html {
  background-color: rgb(244, 244, 244);
}

ul,
li {
  margin: 0;
  padding: 0;
}

span::first-letter {
  text-transform: capitalize;
}

body {
  font-family: "Roboto Condensed", serif;
}

ul {
  list-style: none;
  display: flex;
  justify-content: space-around;
  max-width: 86%;
}

.timeline {
  counter-reset: test 0;
  position: relative;

}


/* timeline styling  */
.timeline li:before {
  counter-increment: test;
  content: counter(test);
  width: 50px;
  height: 50px;
  border: 3px solid #e5c477;
  border-radius: 50%;
  display: block;
  text-align: center;
  line-height: 50px;
  margin: 0 auto 10px auto;
  background: #d58f48;
  color: #ffffff;
  transition: all ease-in-out 0.3s;
  cursor: pointer;  
}

/* .timeline li:after{
  content: "";
    position: absolute;
    width: 62%;
    height: 4px;
    background-color: grey;
    top: 23px;
    left: 19%;
    z-index:999;

    transition: all ease-in-out .3s;
 
  
} */

.timeline li:first-child:after {
  content: none;
}

.SecImg {
  height: 4px;
  width: 71%;
  top: 24px;
  left: 0px;
  background-color: #d58f48;
  position: relative;
}

.SecImgg {
  height: 4px;
  width: 71%;
  top: 7px;
  left: 0px;
  background-color: #d58f48;
  position: relative;
}

.timeline {
  max-width: 71%;
}

/* second timeline css  */

ol {
  display: flex;
  justify-content: space-around;
  content: "";
}

/* .SecondTimeline:before {
  content: "";
  width: 17px;
  height: 17px;
left:-17px;

  border-radius: 50%;
  display: block;

  margin: 0 auto 10px auto;
  background: #d58f48;

  cursor: pointer;
}
li.SecondTimeline {
    max-width: 0px;
} */
.contai{
  
    padding: 52px;
    margin-top: 74px;
    background-color: white;
    max-width: 50%;
    border-radius: 1rem;
   
}

.timeline {
  animation:fadee 10s ;
}
@keyframes fadee {
  0% { opacity: 0; }
  100% { opacity: 1; }
}
/* for timeline text  */
.text{
  padding:16px;
  animation: fadee 10s;
}

@media screen and (min-width:350px) and (max-width: 450px){
  .text {
    padding: 0px !important; 
}
.timeline {
    max-width: 85%;
}
.btn.btn-lg.btn-outline-primary.mt-5 {
    margin-top: 15px !important;
}
button.btn.btn-lg.bg-dark.text-white.rounded-5.smallbtntext {
    margin-top: 0.5rem;
}
}
/* summary text is optional and can be anything */</style>

