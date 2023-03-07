<template>
  <div class="custom-lnk__text flex-wrap ">
    <a class="display-6 custom-lnk"> <slot></slot></a>
  </div>
</template>

<script>
export default {
  name: "FooterLink"
}
</script>

<style lang="sass">

.custom-lnk
  font-family: monospace
  cursor: pointer
  color: #000


  &:after
    opacity: 0.4
    content: "\2197"

  &:hover
    color: var(--bs-primary)
    &:after
      scale: 1.5
      opacity: 1


.clicked
  .custom-lnk
    color: var(--bs-primary)

    scale: 1.5
    opacity: 1

</style>