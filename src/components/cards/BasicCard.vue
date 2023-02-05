<template>
  <div class="card rounded-5 m-3 basic-card"
       @mouseover="addClass"
       @mouseleave="removeClass"
       @click="goToLNK(lnk)">

    <slot name="image"></slot>

    <div class="card-body text-black basic-card__body">
      <div class="position-relative float-end github-icon" ><img src="src/images/git.svg" alt="github-icon"></div>
      <h5 class="card-title fs-3">
        <slot name="title"></slot>
      </h5>
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
export default {
  name: "BasicCard",
  props: {
    lnk: String
  },
  methods: {
    addClass: function () {
      this.$el.classList.add("shadow", "bg-body-tertiary", "rounded")
    },
    removeClass: function () {
      this.$el.classList.remove("shadow", "bg-body-tertiary", "rounded")
    },

    goToLNK: function (link) {
      window.location.href = link
    }
  }
}
</script>

<style lang="sass">

.basic-card
  cursor: pointer
  transition: all ease-in-out 0.15s

  .github-icon
    opacity: 0

  &:hover
    scale: 1.02
    .github-icon
      opacity: 1
      scale: 1.2

  .basic-card__body
    height: border-box

</style>