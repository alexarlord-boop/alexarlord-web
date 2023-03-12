<template>

    <span class="badge custom-badge bg-black rounded-pill m-1">
    <slot></slot>
    </span>

</template>

<script>
export default {
  name: "Tooltip"
}
</script>

<style lang="sass">
  .custom-badge
    box-shadow: rgba(182, 180, 180, 0.65) 3px 3px 5px 2px
</style>