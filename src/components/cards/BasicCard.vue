<template>
  <a class="card rounded-5 m-3 basic-card"
     :href="lnk"
     target="_blank"
       @mouseover="addClass"
       @mouseout="removeClass">

    <div class="d-flex justify-content-evenly">
      <slot name="image"></slot>
    </div>

    <div class="card-body text-black basic-card__body">
      <!--      <div class="position-relative float-end github-icon" ><img src="src/images/git.svg" alt="github-icon"></div>-->
      <div class="position-relative float-end github-icon">
        <slot name="small-icon">
          <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" class="bi bi-github" viewBox="0 0 16 16">
            <path
                d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"/>
          </svg>
        </slot>
      </div>
      <h5 class="card-title fs-3">
        <slot name="title"></slot>
      </h5>
      <p class="card-text fs-5 mt-3">
        <slot name="text"></slot>
      </p>
    </div>
    <div class="card-footer border-white bg-transparent fs-5">
      <slot name="tooltips"></slot>
    </div>
  </a>
</template>

<script>
export default {
  name: "BasicCard",
  props: {
    lnk: String
  },
  // methods: {
  //   addClass: function () {
  //     this.$el.classList.add("shadow-lg", "bg-body-tertiary", "rounded")
  //   },
  //   removeClass: function () {
  //     this.$el.classList.remove("shadow-lg", "bg-body-tertiary", "rounded")
  //   }
  // }
}
</script>

<style lang="sass">
a
  &:active, &:visited
    color: black

.basic-card
  cursor: pointer
  transition: all ease-in-out 0.15s
  border: 1px rgba(182, 180, 180, 0.65) solid
  box-shadow: rgba(182, 180, 180, 0.65) 3px 3px 5px 2px

  .github-icon
    opacity: 0

  &:hover
    scale: 1.02
    box-shadow: rgba(182, 180, 180, 0.65) 12px 12px 20px 2px

    .github-icon
      opacity: 1
      scale: 1.2


</style>