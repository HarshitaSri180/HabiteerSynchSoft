<template>
  <!-- fouth   -->
  <!-- image  -->
  <img class="meetthehbtr" src="" alt="">
  <!-- image  -->
  <div class="container bg-orange p-5 my-5 rounded-4">
    <div id="back">

      <!-- <div class="row  d-flex position-absolute">
          <div class="col-md-6">
            <h4 class="py-3">Habiteer App</h4>
            <h1 class="py-3">Master Your Life by Mastering Your Habbits</h1>

            <ul class="d-flex  py-3 my-3 gap-5 list-unstyled">
              <li class="nav-item ">
                <sapn> <img class=" w-md-75 rounded-2 img-fluid" alt="logo" src="~assets/images/get-on-appstore.png"> </sapn>
              </li>
              <li class="nav-item">
                <i class="bi bi-star-fill mx-1 text-warning"></i>
                <i class="bi bi-star-fill mx-1 text-warning"></i>
                <i class="bi bi-star-fill mx-1 text-warning"></i>
                <i class="bi bi-star-fill mx-1 text-warning"></i>
                <i class="bi bi-star-half mx-1 text-warning"></i>
                <br>
                <p class="text-body-secondary">100+ Appstore Review</p>
              </li>

            </ul>
          </div>
          <div class="col-md-6">

           <img src="~assets/images/right.png" class="img-fluid w-50" alt="">
          
          </div>
        </div> -->

    </div>

    <div id="top ">
      <div class="row my-2 d-flex justify-content-between aling-self-center">
        <div class="col-md-6 top">
     
          <h5 class=" BuildOut">Build out of frustation</h5>
          <h1 class=" fw-bolder meetThehabiteer ">Meet the Habiteer</h1>

          <!-- <span> <img class=" w-md-75 rounded-2 img-fluid" alt="logo" src="~assets/images/get-on-appstore.png"></span> -->
 

  
        </div>
        <!-- right col  -->
        <div class="col-md-6  right-col d-flex justify-content-center align-items-center">
        <img class=" rotatingImg " src=" ">
        </div>

      </div>
      <!-- buttom row -->
      <div class="row my-2 d-flex justify-content-between aling-self-center">
        <div class="col-md-6 top">
         

     <img class=" w-75 rounded-2 img-fluid mTHImage" alt="" src="https://images.pexels.com/photos/848573/pexels-photo-848573.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2">
          

        </div>
        <!-- right col  -->
        <div class="col-md-6  right-col d-flex justify-content-center align-items-center">
          <div class=" w-75">
           
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sapiente odio reprehenderit adipisci non rerum
              deleniti temporibus corporis quas accusamus consectetur accusantium qui blanditiis asperiores?</p>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sapiente odio reprehenderit adipisci non rerum
              deleniti temporibus corporis quas accusamus consectetur accusantium qui blanditiis asperiores, nobis unde
              ipsam eveniet doloremque nihil ea vel. Modi ipsa ipsum sit tempora sunt debitis delectus?</p>
          </div>
        </div>

      </div>
    </div>
</div></template>
<style>
/* image styling  */
img.meetthehbtr {
    margin-right: 109px;
    float: right;
    margin-top: -20px;
    height: 51px;
    animation: mymove 4s linear infinite;
}
@keyframes mymove{
  0%{
    transform:rotate(120deg);
  }
  100%{
    transform: rotate(360deg);
  }
}

img.rotatingImg {
    height: 34px;
    animation:rotateImg 3s linear infinite;
    margin-left: 261px;
}
@keyframes rotateImg{
  0%{
    transform: rotate(120deg);
  }
  100%{

    transform:rotate(360deg);
  }
}
@media screen and (min-width:350px) and (max-width: 450px){
  .meetThehabiteer{
    text-align: center;
  }
  .BuildOut{
    text-align: center;  
  }
  h1.fw-bolder.meetThehabiteer {
    font-size: 2.5rem !important;
}
img.w-75.rounded-2.img-fluid {
    margin-bottom: 2.5rem;
} 
}
@media screen and (min-width:760px ) and (max-width:1050px){
  img.w-75.rounded-2.img-fluid.mTHImage {
    margin-left: 53px;
}
}
</style>