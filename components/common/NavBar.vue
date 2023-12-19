<template>
  <div>
    <div class="container">
      <header
        class="d-flex flex-wrap align-items-center justify-content-center justify-content-md-between py-3 mb-4"
      >
        <div class="col-md-3 mb-2 mb-md-0">
          <a
            href="/"
            class="d-inline-flex link-body-emphasis text-decoration-none"
          >
            <img
              class="navbar-logo rounded-2"
              alt="logo"
              src="~/assets/images/logo/logo.png"
            />
          </a>
        </div>

        <ul
          class="nav col-12 col-md-auto mb-2 justify-content-center mb-md-0 gap-4"
        >
          <li>
            <a href="#" class="nav-link px-2 text-dark link-secondary"
              >Emotion</a
            >
          </li>
          <li><a href="#" class="nav-link px-2 text-dark">Manifesto</a></li>
          <li>
            <a href="#" class="nav-link px-2 text-dark">Self-awareness test</a>
          </li>
          <li><a href="#" class="nav-link px-2 text-dark">Work with us</a></li>
        </ul>

        <div class="col-md-3 text-end">
          <button
            id="downloadbtn"
            type="button"
            class="btn btn-dark me-2 rounded-5"
          >
            Download app
          </button>
        </div>
      </header>
    </div>
  </div>
</template>

<script>
import anime from "animejs";

export default {
  mounted() {
    // anime({
    //   targets: '.navbar-logo',
    //  translateX: [-200, 0],
    //   easing: 'easeOutExpo',
    //   delay: 1000,
    //   duration: 1000,
    //   opacity: [0, 1],
    // });
    anime({
      targets: "#downloadbtn",
      translateY: [-200, 0],
      easing: "easeOutExpo",
      delay: 1000,
      duration: 1000,
      opacity: [0, 1],
    });
  },
};
</script>

<style scoped>
@media screen and (min-width:350px) and (max-width: 450px) {
  ul.nav.col-12.col-md-auto.mb-2.justify-content-center.mb-md-0.gap-4 {
    display: block;
    text-align: center;
  }
 
}
/* Add your scoped styles here */
</style>
