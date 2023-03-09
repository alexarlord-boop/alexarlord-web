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
    box-shadow: rgba(112, 111, 112, 0.58) 3px 3px 5px 2px
</style>