<template>
  <!-- six  -->
  <div class="container py-5 my-5">
    <div class="SelfImprovementSubTitle">
      Lorem, ipsum dolor sit amet consectetur adipisicing elit.
    </div>
    <h1 class="Self-improvement fw-bolder">Self-improvement.ugh.</h1>

    <div class="textWrapper">
      <div class="row m-5 py-3 d-flex">
        <div class="col-md-4 p-2 TimelineMedia">
          <!-- timeline code starts here  -->
          <div class="cd-main-content journey-style">
            <div class="timeline fadeIn">
              <div class="line text-muted"></div>

              <article class="panel panel-default panel-outline date-extend">
                <div class="panel-heading icon"></div>
                <div class="panel-body">
                  <h3>
                    <time>December 5,2015</time>
                    <p>
                      Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                      Tempore deleniti recusandae incidunt iste blanditiis autem
                      consequuntur esse, placeat odit natus perferendis
                      perspiciatis? Quibusdam necessitatibus sint ullam ad,
                      quisquam laboriosam voluptatibus.
                    </p>
                  </h3>
                </div>
              </article>

              <article class="panel pael-default panel-outline date-extend1">
                <div class="panel-heading icon"></div>
                <div class="panel-body">
                  <h3>
                    <time>February 26,2016</time>
                    <p>
                      Lorem ipsum dolor sit amet consectetur adipisicing elit.
                      Sed nihil odio iste quam optio quaerat quia perferendis
                      necessitatibus itaque neque, excepturi ex tenetur quae
                      corporis debitis. Facilis, et. Culpa, nisi?
                    </p>
                  </h3>
                </div>
              </article>

              <article class="panel panel-default panel-outline date-extend1">
                <div class="panel-heading icon"></div>
                <div class="panel-body">
                  <h3>
                    <time>December 15,2016</time>
                    <p>
                      Lorem ipsum dolor sit amet consectetur adipisicing elit.
                      Quibusdam sed libero id. Repellendus facilis quas
                      consectetur dignissimos ipsam tempore veniam beatae!
                      Placeat esse deserunt autem dignissimos, impedit ea
                      ducimus ut.
                    </p>
                  </h3>
                </div>
              </article>

              <article class="panel panel-default panel-outline date-extend">
                <div class="panel-heading icon"></div>
                <div class="panel-body">
                  <h3>
                    <time>December 15,2016</time>
                    <p>
                      Lorem ipsum dolor sit amet consectetur adipisicing elit.
                      Praesentium maxime doloribus temporibus ab nesciunt
                      asperiores laboriosam quaerat suscipit, consequuntur
                      nostrum repellat aspernatur enim repudiandae
                      exercitationem recusandae ullam doloremque magnam cumque!
                    </p>
                  </h3>
                </div>
              </article>
            </div>
          </div>
          <!-- timeline code ends here  -->
        </div>
      </div>
    </div>
  </div>
</template>
<style scoped>
* {
  box-sizing: border-box;
  margin: 0px;
  padding: 0px;
}

body,
html {
  background: #2d3244;
}

/*--------------timeline-----------------*/
.journey-style {
  width: 100%;
  margin: 0 auto;
}

.journey-style .timeline {
  position: relative;
  padding: 0px 0px 10px;
  font-family: "Inter", sans-serif;
  margin-bottom: 30px;

  /* animation:fadeIn 15s ; */
}

/* @keyframes fadeIn {
  0% { opacity: 0; }
  100% { opacity: 1; }
} */

.journey-style .timeline .line {
  position: absolute;
  width: 2px;
  display: block;
  background: #6743ef;
  top: 0px;
  bottom: 179px;
  margin-left: 32px;
  color: #6743ef;
}

.journey-style .timeline .separator {
  border-top: 1px solid currentColor;
  padding: 5px;
  padding-left: 40px;
  font-family: "Inter", sans-serif;
  font-size: 0.9em;
  margin-left: 30px;
}

.journey-style .timeline .line::before {
  top: -4px;
}

.journey-style .timeline .panel {
  position: relative;
  margin: 10px 0px 21px 70px;
  clear: both;
}

.journey-style .timeline .panel::before {
  position: absolute;
  display: block;
  top: 8px;
  left: -24px;
  content: "";
  width: 0px;
  height: 0px;
  border: inherit;
  border-width: 12px;
  border-top-color: transparent;
  border-bottom-color: transparent;
  border-left-color: transparent;
}

.hover-color-link span:hover {
  color: #fff;
  background-image: linear-gradient(60deg, #29323c 0%, #485563 100%) !important;
  transition: 0.5s;
  box-shadow: 0 5px 11px 0 rgba(0, 0, 0, 0.18), 0 4px 15px 0 rgba(0, 0, 0, 0.15);
  transition: 0.2s ease-out;
}

.hover-color-link:hover {
  color: #ffffff;
}

.journey-style .timeline .panel .panel-heading.icon * {
  font-size: 20px;
  vertical-align: middle;
  line-height: 40px;
}

.journey-style .timeline .panel .panel-heading.icon {
  position: absolute;
  left: -45px;
  display: block;
  width: 15px;
  height: 15px;
  padding: 0px;
  border-radius: 50%;
  text-align: center;
  float: left;
  border-color: transparent;
  transition: 1.3s;
}

.journey-style .timeline .panel-outline {
  border-color: transparent;
  background: transparent;
  box-shadow: none;
}

.journey-style .journey-style .timeline .panel-outline .panel-body {
  padding: 10px 0px;
}

.journey-style .timeline .panel-outline .panel-heading:not(.icon),
.journey-style .timeline .panel-outline .panel-footer {
  display: none;
}

.journey-style .panel-heading {
  background-color: #6743ef;
  color: #ffffff;
}

.journey-style .date-extend .panel-heading {
  background-color: #6743ef;
}

.journey-style .panel-body {
  padding: 0px;
  cursor: pointer;
}

.journey-style .panel-body h3 {
  margin: 0px;
  text-align: left;
  margin-left: 1em;
  margin-top: -0.3em;
  padding-bottom: 0.5em;
  line-height: 1.3em;
}

.journey-style .panel-body h3 time {
  font-family: "Inter", sans-serif;
  color: #c2c2c2;
  font-size: 1.25rem;
  font-weight: 600;
  font-family: "Inter", sans-serif;
}

.journey-style .panel-body h3 time:hover {
  color: #070707 !important;
}

.journey-style .panel-body h3 p {
  font-size: 1rem;
  color: #c2c2c2 !important;
  font-weight: 400;
  font-family: "Inter", sans-serif;
}

.journey-style .panel-body h3 p:hover {
  color: #070707 !important;
}

.journey-style .panel-outline:hover .panel-heading.icon {
  -webkit-transform: scale(1.7, 1.7) rotate(45deg);
  -moz-transform: scale(1.7, 1.7) rotate(45deg);
  -ms-transform: scale(1.7, 1.7) rotate(45deg);
  -o-transform: scale(1.7, 1.7) rotate(45deg);
  transform: scale(1.7, 1.7) rotate(45deg);
  transition: background 0.5s;
  transition: 0.5s;
}

.journey-style .timeline .year-time {
  position: relative;
  left: -45px;
  color: #fff;
  top: 33px;
  font-size: 16px;
  float: left;
  font-family: "Josefin Sans", sans-serif;
}

.journey-style .timeline .year-time1 {
  position: relative;
  left: -45px;
  color: #fff;
  top: 33px;
  font-size: 16px;
  float: left;
  font-family: "Josefin Sans", sans-serif;
}

.journey-style .panel-body h3 p {
}

.Self-improvement {
  font-weight: 600;
}

/* media queries  */

@media screen and (max-width: 768px) {
  .journey-style .timeline {
    max-width: 95vw;
    padding: 3px;
    color: #070707;
    margin-left: 0px !important;
  }

  .journey-style .timeline .line {
    bottom: 46px;
    margin-top: -7px;
  }
}
.SelfImprovementSubTitle {
  font-size: 1.25rem;
}

@media screen and (min-width: 769px) {
  .journey-style .timeline {
    margin-left: 56px;
    width: 93%;
  }
}

@media screen and (min-width: 350px) and (max-width: 450px) {
  .journey-style .panel-body h3 p {
    color: black !important;
    width: 120%;
  }
  .journey-style .panel-body h3 p:hover{
    color: #c2c2c2;
  }
  .journey-style .panel-body h3 time {
    color: black;
  }
  .SelfImprovementSubTitle {
    text-align: center;
  }
  h1.Self-improvement.fw-bolder {
    text-align: center;
  }
  .journey-style .timeline .line {
    margin-left: -31px;
  }
  .panel-heading.icon {
    margin-left: -62px;
  }
  .journey-style .panel-body h3 {
    margin-left: -3em;
  }
  h1.Self-improvement.fw-bolder {
    margin-top: 10px;
}


  @media screen and (min-width: 750px) and (max-width: 1024px) {
    .panel-body {
      width: 100% !important;
    }
    .SelfImprovementSubTitle {
    text-align: center;
}
h1.Self-improvement.fw-bolder {
    text-align: center;
}
  }
}
@media (min-width: 768px)
{
.col-md-4 {
    flex: 0 0 auto;
    width: 103.333333%;
}
h1.Self-improvement.fw-bolder {
    text-align: center;
}
.SelfImprovementSubTitle {
    text-align: center;
}
}
/* for gradient  */

/* .fadeIn {
	opacity: 0.5;
 transform: translateX(50px, 50px);

	cursor: pointer;
	transition: 0.25s all ease-in-out;
}

.fadeIn:hover {
	opacity: 1;
    transform: translateX(50px, 50px);
} */
</style>
<script>
// for opacity
</script>
