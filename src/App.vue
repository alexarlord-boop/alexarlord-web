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
</script>

<template>

  <header>
    <Navbar></Navbar>
  </header>

  <h1 class="display-1 mt-3">My projects</h1>

  <div class="col mt-5 custom-grid">



    <div id="devops-projects" class="row align-items-sm-start">
      <div class="col">
        <WebSiteCard/>
      </div>
            <div class="col">
              <h1 class="display-6 text-center m-5">Cloud</h1>
              <ApkCard/>
            </div>
    </div>

    <div id="android-projects" class="row align-items-center cards-content-left-over-right">
      <div class="col">
        <h1 class="display-6 text-center m-5">Software</h1>
        <ApiCard/>
      </div>
      <div class="col">
        <AndroidCard/>
      </div>

    </div>

    <h1 class="display-6 text-center m-5">Basics</h1>
    <div id="uni-basics-projects" class="cards-content-right-over-left">
      <div class="col">
        <RequestCard/>
      </div>
      <div class="col">
        <AgileCard/>
        <StructureCard/>
      </div>
    </div>
  </div>

  <p class="row"></p>
  <p class="row"></p>
  <p class="row"></p>
  <p class="row"></p>
  <p class="row"></p>
  <p class="row"></p>
  <p class="row"></p>


  <div id="contact-section" class="text-center" @mouseover="initLink"
       @mouseleave="ejectLink">

    <div class=" custom-more-info custom-grid">

      <div class="row">
        <div class="col-6 align-self-center text-end">
          <FooterLinks>
            <FooterLink id="clicked" class="clicked">github</FooterLink>
            <FooterLink>linkedin</FooterLink>
          </FooterLinks>
        </div>
        <div class="col-6 text-start">
          <FooterLinks>
            <FooterLink>telegram</FooterLink>
          </FooterLinks>
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

</style>
