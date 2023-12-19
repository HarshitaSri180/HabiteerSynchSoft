<template>
  <!-- Open Vacancies -->
  <div class="container py-4 my-5">
    <div class="row py-3 mt-3 d-flex">
      <h2 class="Open-Vacancies">Open Vacancies</h2>
    </div>

    <!-- all cards  -->
    <div class="cards">
      <div class="row  py-3 d-flex">
        <!-- card  -->
        <div class="col-md-4 p-2 text-body-secondary">
          <div class="card card-btn-hover shadow bg-light-yellow rounded-4 border-0" @mouseenter="hoverIn" @mouseleave="hoverOut">
            <div class="card-body">
              <h5 class="card-title ps-3 py-2">Special title</h5>
              <ul>
                <li class="my-1">lorem</li>
                <li class="my-1">lorem</li>
                <li class="my-1">lorem</li>
              </ul>
              <center>
                <button class="btn btn-dark rounded-5">Click me</button>
              </center>
            </div>
            
            
          </div>
        </div>
        <div class="col-md-4 p-2 text-body-secondary">
          <div class="card card-btn-hover shadow bg-light-yellow rounded-4 border-0" @mouseenter="hoverIn" @mouseleave="hoverOut">
            <div class="card-body">
              <h5 class="card-title ps-3 py-2">Special title</h5>
              <ul>
                <li class="my-1">lorem</li>
                <li class="my-1">lorem</li>
                <li class="my-1">lorem</li>
              </ul>
              <center>
                <button class="btn btn-dark rounded-5">Click me</button>
              </center>
            </div>
            
            
          </div>
        </div>
        <div class="col-md-4 p-2 text-body-secondary">
          <div class="card card-btn-hover shadow bg-light-yellow rounded-4 border-0" @mouseenter="hoverIn" @mouseleave="hoverOut">
            <div class="card-body">
              <h5 class="card-title ps-3 py-2">Special title</h5>
              <ul>
                <li class="my-1">lorem</li>
                <li class="my-1">lorem</li>
                <li class="my-1">lorem</li>
              </ul>
              <center>
                <button class="btn btn-dark rounded-5">Click me</button>
              </center>
            </div>
            
            
          </div>
        </div>
        <!-- Add the rest of your cards here -->
        <!-- second card  -->
        <!-- third card  -->
      </div>
    </div>
  </div>
</template>

<script>
import anime from 'animejs';

export default {
  methods: {
    hoverIn(event) {
      const button = event.currentTarget.querySelector('.btn');
      anime({
        targets: button,
        translateY: [-10, -20],
        easing: 'easeInOutQuart', // Change easing function
        duration: 30, // Increase duration
        delay: 60,
        opacity: [0, 1],
        scale: [0, 1],
      });
    },
    hoverOut(event) {
      const button = event.currentTarget.querySelector('.btn');
      anime({
        targets: button,
        translateY: [-20, -10],
        easing: 'easeInOutQuart', // Change easing function
        duration: 20, // Adjust duration
        opacity: 0,
      });
    },
  },
};
</script>

<style scoped>
/* Add your scoped styles here */
.bg-light-yellow {
  background-color: #fefbec;
}
.card-btn-hover:hover {
  height: 13rem;
  transition: height 0.5s ease; /* Add a transition for smoother size change */
}
.card {
  height: 10rem !important;
  transition: height 0.5s ease; /* Add a default transition */
}
.card:hover {
  height: 13rem !important;
}

.btn {
  position: relative;
  bottom: 10px;
  margin-top: 20px;
  transform: translateX(-50%);
  opacity: 0;
  transition: opacity 0.5s ease, transform 0.5s ease; /* Add transitions for opacity and transform */
}
@media screen and (min-width:350px) and (max-width: 450px){
h2.Open-Vacancies {
    text-align: center;
}}

</style>
