<template>
<div>
  <basic-card v-bind:lnk="'https://github.com/alexarlord-boop/java-au'" class="sideproject">
    <template v-slot:image>
      <svg xmlns="http://www.w3.org/2000/svg" width="5rem" height="5rem" fill="black" class="bi bi-bricks m-3"
           viewBox="0 0 16 16">
        <path
            d="M0 .5A.5.5 0 0 1 .5 0h15a.5.5 0 0 1 .5.5v3a.5.5 0 0 1-.5.5H14v2h1.5a.5.5 0 0 1 .5.5v3a.5.5 0 0 1-.5.5H14v2h1.5a.5.5 0 0 1 .5.5v3a.5.5 0 0 1-.5.5H.5a.5.5 0 0 1-.5-.5v-3a.5.5 0 0 1 .5-.5H2v-2H.5a.5.5 0 0 1-.5-.5v-3A.5.5 0 0 1 .5 6H2V4H.5a.5.5 0 0 1-.5-.5v-3zM3 4v2h4.5V4H3zm5.5 0v2H13V4H8.5zM3 10v2h4.5v-2H3zm5.5 0v2H13v-2H8.5zM1 1v2h3.5V1H1zm4.5 0v2h5V1h-5zm6 0v2H15V1h-3.5zM1 7v2h3.5V7H1zm4.5 0v2h5V7h-5zm6 0v2H15V7h-3.5zM1 13v2h3.5v-2H1zm4.5 0v2h5v-2h-5zm6 0v2H15v-2h-3.5z"/>
      </svg>
    </template>
    <template v-slot:title>Algorithms & Data structures</template>
    <template v-slot:text>Leetcode solutions with nice-looking boxing. <br> I created Markdown generator to wrap
      up my solutions and related test cases.
    </template>
    <template v-slot:tooltips>
      <tool-tip>Git</tool-tip>
      <tool-tip>Markdown</tool-tip>
      <tool-tip>Java</tool-tip>
    </template>
  </basic-card>

</div>
</template>

<script>
import BasicCard from "@/components/cards/BasicCard.vue";
import Tooltip from "@/components/Tooltip.vue";

export default {
  name: "StructureCard",
  components: {
    'basic-card': BasicCard,
    'tool-tip': Tooltip
  }
}
</script>

<style scoped>

</style>