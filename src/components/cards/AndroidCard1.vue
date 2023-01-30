<template>
  <div id="{{cardNumber}}" class="card rounded-5 m-3 custom-card-android"
       @mouseover="addClass(cardNumber)"
       @mouseleave="removeClass(cardNumber)">
    <img src="src/images/unnamed.jpeg" class="card-img-top p-4" alt="...">

    <div class="card-body text-black body-android">
      <h5 class="card-title fs-3">Application for local IT business</h5>
      <p class="card-text">
        Useful tool for workers in IT power company. This app helps collect data and manage records about city areas.
      </p>
    </div>

    <div class="card-footer bg-transparent border-white fs-5">
      <Tooltip>Kotlin</Tooltip>
      <Tooltip>Jetpack Compose</Tooltip>
      <Tooltip>Material Design</Tooltip>
    </div>
  </div>
</template>

<script>
import Tooltip from "@/components/Tooltip.vue";

export default {
  name: "AndroidCard1",
  components: {Tooltip},
  props: {
    cardNumber: String
  },
  methods: {
    addClass: function () {
      this.$el.classList.add("shadow", "bg-body-tertiary", "rounded")
    },
    removeClass: function () {
      this.$el.classList.remove("shadow", "bg-body-tertiary", "rounded")
    }
  }

}
</script>

<style lang="sass">

$android-color: #3ddc84

.custom-card-android
  transition: all ease-in-out 0.15s
  border: 3px solid $android-color

  &:hover
    scale: 1.02

  .body-android
    background-color: $android-color
    height: border-box



</style>