
<template>
  <!-- cards  -->

  <div class="container py-5 my-5">
    <div class="IMageSec d-flex">
    <h2 id="cardheading" class="my-5">Does this sound familiar...</h2>
</div>
    <div id="cards" class="row m-5 py-3 d-flex">
      <div class="col-md-3 p-2">
        <div class="card border-0 rounded-4 py-2  CardMedia" :style="{ width: '100%', backgroundColor: '#FCEFD4' }">
          <div class="card-body">
            <h4 class="card-title ">😎</h4>
            <h6 class="card-subtitle mb-2 text-body-secondary">Card subtitle</h6>
            <p class="card-text text-body-secondary">
              Some quick example text to build on the card title and make up the bulk of the card's content.
            </p>
          </div>
        </div>
      </div>


      <div class="col-md-3 p-2">
        <div class="card border-0 rounded-4 py-2 CardMedia" :style="{ width: '100%', backgroundColor: '#EEEBFE' }">
          <div class="card-body">
            <h4 class="card-title ">😎</h4>
            <h6 class="card-subtitle mb-2 text-body-secondary">Card subtitle</h6>
            <p class="card-text text-body-secondary">
              Some quick example text to build on the card title and make up the bulk of the card's content.
            </p>
          </div>
        </div>
      </div>
      <div class="col-md-3 p-2">
        <div id="hovercard" class="card border-0 rounded-4 py-2 shadow-lg CardMedia " :style="{ width: '100%', backgroundColor: '#6441EF' }">
          <div class="card-body">
            <h4 class="card-title ">😎</h4>
            <h6 class="card-subtitle mb-2 text-white">Card subtitle</h6>
            <p class="card-text  text-white">
              Some quick example text to build on the card title and make up the bulk of the card's content.
            </p>
          </div>
        </div>
      </div>
      <div class="col-md-3 p-2">
        <div class="card border-0 rounded-4 py-2 CardMedia" :style="{ width: '100%', backgroundColor: '#D9F2FF' }">
          <div class="card-body">
            <h4 class="card-title ">😎</h4>
            <h6 class="card-subtitle mb-2 text-body-secondary">Card subtitle</h6>
            <p class="card-text text-body-secondary">
              Some quick example text to build on the card title and make up the bulk of the card's content.
            </p>
          </div>
        </div>
      </div>



    </div>
  </div>
</template>


<script>
import anime from 'animejs';

export default {
  mounted() {
    const options = {
      root: null,
      rootMargin: '70px',
      threshold: 0.1,
    };

    const callback = (entries, observer) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          const targets = entry.target;
          anime({
            targets: "#cards",
            translateX: [500, 0],
            easing: 'easeOutExpo',
            delay: 1000,
            duration: 3000,
            opacity: [0, 1],
          });
          anime({
            targets: '#cardheading',
            easing: 'easeOutExpo',
            delay: 500,
            duration: 2000,
            translateX: [-650, 0],
            opacity: [0, 1],
            scale: [0.1, 1]
          });
          observer.unobserve(entry.target);
        }
      });
    };

    const observer = new IntersectionObserver(callback, options);
    const targets = document.querySelector('#cards');
    if (targets) {
      observer.observe(targets);
    }

    //end

    anime({
      targets: 'jellyImage',
      translate: [-360, 0],
      easing: 'easeOutExpo',
      delay:  1000,
      duration:   2000,
      opacity: [0, 1],
    });


  },
};



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


</script>

<style scoped>
.card {
  border: 0;
}

/* Adjust the styles for your card styles */
.card-style1 {
  width: 17rem;
  background-color: #FCEFD4;
}

.card-style2 {
  width: 17rem;
  background-color: #EEEBFE;
}

.card-style3 {
  width: 17rem;
  background-color: #6441EF;
}

.card-style4 {
  width: 17rem;
  background-color: #D9F2FF;
}

/* Adjust the hover styles for your card */
#hovercard {
  margin: 0rem 0.2rem;
  transform: rotate(-7deg);
  color: white;
}

#hovercard:hover {
  margin: 0rem 0.2rem;
  transform: rotate(-7deg);
  color: white;
  box-shadow: 10px 10px 10px 1px;
}
/* @media screen and (min-width: 414px) and (max-width: 1395px) {
  #hovercard {
    background-color: #e52320;
  }
} */
@media screen and (min-width:350px) and (max-width: 450px){
  div#hovercard {
   
    margin-top: 15px !important;
    margin-bottom: 15px !important;
}
h5 {
    text-align: center;
}
.IMageSec.d-flex {
    margin-top: -33px;
}
.container.my-5.py-5 {
    padding-top: 1rem!important;
    padding-bottom: 0rem!important;
}
@media screen and (min-width:758px) and (max-width:1024px){
  .col-md-3.p-2 {
    width: 100% !important;
}

}
@media screen and (min-width:750px) {
  .IMageSec.d-flex {
    margin-top: -9.5rem;
    background-color: red;
}
.IMageSec.d-flex {
    margin-left: 162px;
}
}
}
</style>









