







<template>
  <div class="container bg-purple p-5 rounded-4">

    <div id="top">
      <div class="row my-2 d-flex justify-content-between">
        <div class="col-md-6 top ">
          <div class="headings">
            <h4 class="py-3">Habiteer App</h4>
            <h1 class="py-3 fw-bolder" id="heading">
              Master Your Life by Mastering Your Habbits
            </h1>
          </div>

          <!-- app icon  -->
          <ul class="d-flex py-3 my-3 gap-5 list-unstyled">
            <li class="nav-item">
              <sapn>
                <img class="w-md-75 rounded-2 img-fluid icon" alt="logo" src="~assets/images/get-on-appstore.png" />
              </sapn>
            </li>
            <li class="nav-item">
              <i class="bi bi-star-fill mx-1 text-warning"></i>
              <i class="bi bi-star-fill mx-1 text-warning"></i>
              <i class="bi bi-star-fill mx-1 text-warning"></i>
              <i class="bi bi-star-fill mx-1 text-warning"></i>
              <i class="bi bi-star-half mx-1 text-warning"></i>
              <br />
              <p class="text-body-secondary">100+ Appstore Review</p>
            </li>
          </ul>
        </div>
        <!-- img colum  -->

        <div class="col-md-6 text-center">
         
          
     
        <div class="back">
          <!-- <img src="https://images.pexels.com/photos/848573/pexels-photo-848573.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2" class="img-fluid w-100 " alt=""> -->
        </div>
          
     
        <div class="top">
          <!-- <img src="https://images.pexels.com/photos/848573/pexels-photo-848573.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2" class="img-fluid text-center " alt=""> -->
        </div>
        </div>
      </div>
    </div>
  </div>
</template>


<style>

.back{
  position: absolute;
animation:rotate 4s linear infinite;
}
.top{
  position: relative;
}
@keyframes rotate{
  0%{
    transform: rotate(120deg);
  }
  100%{
    transform:rotate(360deg);
  }
}
@media screen and (min-width:350px) and (max-width: 450px){
  img.w-md-75.rounded-2.img-fluid.icon {
    margin-top: 11px !important;
  }
  .container.bg-purple.p-5.rounded-4 {
    padding: 1.5rem !important;
  }
  .top h1 {
    font-size: 2.9rem !important;
}
img.w-75.rounded-2.img-fluid {
    margin-left: 38px;
}
.w-75 {
    margin-left: 38px;
}
}
@media screen and (min-width:768px) and (max-width:1024px){
  img.w-md-75.rounded-2.img-fluid.icon {
    margin-top: 42px;
  ;
}
.top h1 {
    font-size: 3.9rem;
}
}

</style>


<script >
import anime from 'animejs';

export default {
  mounted() {
    // Wrap every letter in a span
    // Select and animate h1 and h4 elements

    // var textWrappers = document.querySelectorAll('h1, h4');

    // textWrappers.forEach(textWrapper => {
    //   textWrapper.innerHTML = textWrapper.textContent.replace(/\S/g, "<span class='letter'>$&</span>");
    //   anime.timeline({ loop: false })
    //     .add({
    //       targets: textWrapper.querySelectorAll('.letter'),
    //       scale: [4, 1],
    //       opacity: [0, 1],
    //       translateZ: 0,
    //       easing: "easeOutExpo",
    //       duration: 950,
    //       delay: (el, i) => 70 * i
    //     });
    // });

    anime({
      targets: '.headings',
      translateX: [-60, 0],
      easing: 'easeOutExpo',
      delay:  1000,
      duration:   2000,
      opacity: [0, 1],
    });
  }
};
</script>
 