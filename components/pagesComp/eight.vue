<template>
  <!-- saven  -->
  <div class="container bg-white p-5 rounded-4">
    <div class=" p-3 p-md-5 m-md-3 text-center" >
      <div class="col-12 mx-auto">
        <p class="lead mb-2"> We take privacy seriously </p>
      </div>
      <div class="mb-2">
        <h2>Before you get started</h2>
      </div>
      <div class="col-12 mx-auto">
        <p class="lead my-2">
          "We won't share your answers with anyone (and won't ever tell
          <br />you which friends said what about you )"
        </p>
      </div>

      <div class="col-12 mx-auto">
        <p class="lead my-3">With love,hhh</p>
      </div>

      <button class="btn btn-lg bg-dark text-white rounded-5 smallbtntext"> Start a Test</button>
      <p class="text-muted my-2">Take only five minutes</p>
    </div>
  </div>
  </template>


<style>
.smallbtntext{
    font-size: 0.9rem;
}

</style>







<script>
import anime from 'animejs';

export default {
  mounted() {
    const options = {
      root: null,
      rootMargin: '10px',
      threshold: 0.1,
    };

    const callback = (entries, observer) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          const targets = entry.target;
          anime({
      targets: '.smallbtntext',
      translateY: [20, 0],
      easing: 'easeOutExpo',
      delay:  1000,
      duration:   2000,
      opacity: [0, 1],
    });
          observer.unobserve(entry.target);
        }
      });
    };

    const observer = new IntersectionObserver(callback, options);
    const targets = document.querySelector('.smallbtntext');
    if (targets) {
      observer.observe(targets);
    }

    //end

  },
};
</script>
 