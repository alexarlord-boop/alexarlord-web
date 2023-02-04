<template>
  <div class="card rounded-5 m-3 basic-card"
       @mouseover="addClass"
       @mouseleave="removeClass">

    <slot name="image"></slot>


    <div class="card-body text-black basic-card__body">
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

.basic-card
  transition: all ease-in-out 0.15s

  &:hover
    scale: 1.02

  .basic-card__body
    height: border-box

</style>