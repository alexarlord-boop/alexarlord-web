<template>
  <div id="{{cardNumber}}" class="card rounded-5 m-3 custom-card-devops"
       @mouseover="addClass(cardNumber)"
       @mouseleave="removeClass(cardNumber)">

    <slot name="image"></slot>



    <div class="card-body text-black body-devops">
      <h5 class="card-title fs-3"><slot name="title"></slot></h5>
      <p class="card-text">
        <slot name="text"></slot>
      </p>
    </div>

    <div class="card-footer bg-transparent border-white fs-5">
      <slot name="tooltips"></slot>
    </div>
  </div>
</template>

<script>
import Tooltip from "@/components/Tooltip.vue";

export default {
  name: "DevopsCard",
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

$android-color: #0cb4fc

.custom-card-devops
  transition: all ease-in-out 0.15s
  border: 3px solid $android-color

  &:hover
    scale: 1.02

  .body-devops
    background-color: $android-color
    height: border-box



</style>