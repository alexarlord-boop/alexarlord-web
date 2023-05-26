<script setup>

import Navbar from "@/components/Navbar.vue";


import FooterLink from "@/components/FooterLink.vue";
import FooterLinks from "@/components/FooterLinks.vue";
import WebSiteCard from "@/components/cards/WebSiteCard.vue";
import ApkCard from "@/components/cards/ApkCard.vue";
import ApiCard from "@/components/cards/ApiCard.vue";
import AndroidCard from "@/components/cards/AndroidCard.vue";
import RequestCard from "@/components/cards/RequestCard.vue";
import AgileCard from "@/components/cards/AgileCard.vue";
import StructureCard from "@/components/cards/StructureCard.vue";
import IconCommunity from "@/components/icons/IconCommunity.vue";
import IconEcosystem from "@/components/icons/IconEcosystem.vue";
</script>

<template>

  <header>
    <Navbar class="fixed-top navbar-light bg-white"></Navbar>
  </header>


  <div class="col mt-5 custom-grid">

    <div class="container mt-2">
      <h1 @mouseover="startAnimation"
          @mouseleave="stopAnimation" class="card-title mb-3 text-center display-3">Hi there, I'm Alex <span class="hand-container"> <p class="hand-icon" style="transition: transform 4.5s;">👋</p></span>
      </h1>

      <h5 class="mb-5 display-6 text-center"><br>The software engineer, experienced in Android, WEB, ML,
        <br/>Cloud computing.</h5>

      <div class="col-md-12 mx-auto" style="display: flex; justify-content: center; align-items: center; flex-wrap: wrap;">
        <div class="card col-md-8">
          <div class="card-body">

            <h3 class="display-6 text-center">🔧 Technologies</h3>
            <ul class="fs-5">
              <li><strong>Programming Languages:</strong> Java, Kotlin, Python, JavaScript</li>
              <li><strong>Android Development:</strong> Android Studio, Kotlin, Android SDK, Jetpack Compose</li>
              <li><strong>Web Development:</strong> HTML5, CSS3, JavaScript, Vue, Node.js, RESTful APIs</li>
              <li><strong>CI/CD:</strong> Jenkins, GitHub Actions & Pages</li>
              <li><strong>Version Control:</strong> Git, GitHub</li>
              <br>
              <span class="rounded-pill text-bg-warning p-1"> in progress</span>
              <li><strong>Cloud Computing:</strong> AWS, Docker, Kubernetes</li>
              <li><strong>Machine Learning:</strong> TensorFlow, PyTorch, scikit-learn, Jupyter Notebook</li>
            </ul>

          </div>
        </div>
        <div class="card col-md-8 mt-3">
          <div class="card-body">
            <div >
              <h2 class="display-6 text-center">🌱 Learning</h2>
              <ul>
                <li><p class="fs-5">AWS cloud platform to develop scalable and robust applications. </p></li>
                <li><p class="fs-5">Machine learning algorithms and frameworks like <strong>TensorFlow</strong> and
                  <strong>PyTorch</strong> to leverage the power of artificial intelligence in my projects.</p></li>
              </ul>
            </div>
          </div>
        </div>
      </div>

    </div>


    <p id="cloud-projects" class="row"></p>
    <p class="display-6 mt-5 text-center">Welcome to my <span style="">InfoHub!</span> </p>
    <div class="row align-items-sm-start">
      <div class="col">
        <WebSiteCard/>
      </div>
      <div class="col">
        <h1 class="display-6 text-center m-4">DevOps</h1>
        <ApkCard/>
      </div>
    </div>

    <p id="software-projects" class="row"></p>
    <div class="row align-items-center cards-content-left-over-right">
      <div class="col">
        <h1 class="display-6 text-center m-5">Software</h1>
        <ApiCard/>
      </div>
      <div class="col">
        <AndroidCard/>
      </div>

    </div>

    <p id="uni-basics-projects" class="row"></p>
    <div class="cards-content-left-over-right">
      <div class="col">
        <h1 class="display-6 text-center m-5">First Steps</h1>
        <AgileCard/>
        <StructureCard/>
      </div>
      <div class="col">
        <RequestCard/>
      </div>
    </div>
  </div>

  <p class="row"></p>
  <p class="row"></p>
  <p class="row"></p>
  <p class="row"></p>
  <p class="row"></p>


  <div id="contact-section" class="text-center mt-5" @mouseover="initLink"
       @mouseleave="ejectLink">

    <div class=" custom-more-info custom-grid">

      <div class="row">

        <h2 class="display-6">
          <icon-community/>
          Let's Connect
        </h2>
        <h5>Feel free to reach out to me via email at <a href="mailto:petrunina602@gmail.com">petrunina602@gmail.com</a>
          or connect with me here: </h5>


        <FooterLinks>
          <FooterLink id="clicked" class="clicked" v-bind:lnk="'https://github.com/alexarlord-boop'">github</FooterLink>
          <FooterLink v-bind:lnk="'https://www.linkedin.com/in/aleksandr-petrunin-b4b720259/'">linkedin</FooterLink>
          <FooterLink v-bind:lnk="'https://t.me/alexarlord'">telegram</FooterLink>
        </FooterLinks>


        <p class="row"></p>
        <p class="row"></p>
        <p class="row"></p>
        <p class="row"></p>
        <p class="row"></p>
        <div class="position-absolute fixed-bottom text-end row" style="color: rgba(183,182,182,0.85)">
          <div class="col">© Aleksandr Petrunin, 2023. <br/> All rights reserved</div>
        </div>
      </div>
      <!--      <div class="col m-5 float-end"-->
      <!--           data-bs-toggle="popover" data-bs-placement="right"-->
      <!--           data-bs-custom-class="custom-popover"-->
      <!--           data-bs-title="Custom popover"-->
      <!--           data-bs-content="This popover is themed via CSS variables."-->
      <!--      >-->
      <!--        <div class="animation shadow-lg rounded-3">-->
      <!--          <svg xmlns="http://www.w3.org/2000/svg" width="6rem" height="6rem" fill="currentColor" class="bi bi-arrows-fullscreen align-self-center" viewBox="-2 -2 20 20">-->
      <!--            <path fill-rule="evenodd" d="M5.828 10.172a.5.5 0 0 0-.707 0l-4.096 4.096V11.5a.5.5 0 0 0-1 0v3.975a.5.5 0 0 0 .5.5H4.5a.5.5 0 0 0 0-1H1.732l4.096-4.096a.5.5 0 0 0 0-.707zm4.344 0a.5.5 0 0 1 .707 0l4.096 4.096V11.5a.5.5 0 1 1 1 0v3.975a.5.5 0 0 1-.5.5H11.5a.5.5 0 0 1 0-1h2.768l-4.096-4.096a.5.5 0 0 1 0-.707zm0-4.344a.5.5 0 0 0 .707 0l4.096-4.096V4.5a.5.5 0 1 0 1 0V.525a.5.5 0 0 0-.5-.5H11.5a.5.5 0 0 0 0 1h2.768l-4.096 4.096a.5.5 0 0 0 0 .707zm-4.344 0a.5.5 0 0 1-.707 0L1.025 1.732V4.5a.5.5 0 0 1-1 0V.525a.5.5 0 0 1 .5-.5H4.5a.5.5 0 0 1 0 1H1.732l4.096 4.096a.5.5 0 0 1 0 .707z"/>-->
      <!--          </svg>-->
      <!--        </div>-->
      <!--      </div>-->

    </div>
    <div id="page-bottom"></div>
  </div>

</template>

<script>
import * as d3 from "d3"

export default {

  methods: {
    startAnimation() {
      const handIcon = document.querySelector('.hand-icon');
      handIcon.classList.add('animate');
    },
    stopAnimation() {
      const handIcon = document.querySelector('.hand-icon');
      handIcon.classList.remove('animate');
    },
    initLink() {
      // let pageBottom = document.querySelector("#page-bottom")
      // setTimeout(() => {
      //   pageBottom.scrollIntoView({behavior: "smooth"})
      // }, 500)
      //

      let clickedLnk = document.querySelector("#clicked")
      setTimeout(() => {
        clickedLnk.classList.remove("clicked")
      }, 500)
    },
    ejectLink() {
      let clickedLnk = document.querySelector("#clicked")

      setTimeout(() => {
        clickedLnk.classList.add("clicked")
      }, 500)
    }
  }
}

</script>

<style lang="sass">

.animated
  stroke-dasharray: 200
  stroke-dashoffset: 100
  pointer-events: none
  animation: animateDash 5s linear forwards infinite

@keyframes animateDash
  to
    stroke-dashoffset: 50

.animation
  width: 6rem
  height: 6rem
//border: 1px solid #000

.animate
  animation: wave 1s infinite


@keyframes wave
  0%
    transform: rotate(0deg)

  25%
    transform: rotate(-15deg)

  75%
    transform: rotate(15deg)

  100%
    transform: rotate(0deg)

</style>
