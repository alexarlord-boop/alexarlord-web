<template>
<div>
  <basic-card v-bind:lnk="'https://github.com/alexarlord-boop/union-station'" class="git">
    <template v-slot:image>
      <svg xmlns="http://www.w3.org/2000/svg" width="5rem" height="5rem" fill="#fcd40c"
           class="bi bi-train-freight-front m-3" viewBox="0 0 16 16">
        <path
            d="M5.736 0a1.5 1.5 0 0 0-.67.158L1.828 1.776A1.5 1.5 0 0 0 1 3.118v5.51l2-.6V5a1 1 0 0 1 1-1h8a1 1 0 0 1 1 1v3.028l2 .6v-5.51a1.5 1.5 0 0 0-.83-1.342L10.936.158A1.5 1.5 0 0 0 10.264 0H5.736ZM15 9.672l-5.503-1.65A.5.5 0 0 0 9.353 8H8.5v8h4a2.5 2.5 0 0 0 2.5-2.5V9.672ZM7.5 16V8h-.853a.5.5 0 0 0-.144.021L1 9.672V13.5A2.5 2.5 0 0 0 3.5 16h4Zm-1-14h3a.5.5 0 0 1 0 1h-3a.5.5 0 0 1 0-1ZM12 5v2.728l-2.216-.665A1.5 1.5 0 0 0 9.354 7H8.5V5H12ZM7.5 5v2h-.853a1.5 1.5 0 0 0-.431.063L4 7.728V5h3.5Zm-4 5a.5.5 0 1 1 0 1 .5.5 0 0 1 0-1Zm9 0a.5.5 0 1 1 0 1 .5.5 0 0 1 0-1ZM5 13a1 1 0 1 1-2 0 1 1 0 0 1 2 0Zm7 1a1 1 0 1 1 0-2 1 1 0 0 1 0 2Z"/>
      </svg>
    </template>
    <template v-slot:small-icon>
      <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="#fcd40c" class="bi bi-github"
           viewBox="0 0 16 16">
        <path
            d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"/>
      </svg>
    </template>
    <template v-slot:title>Team Project</template>
    <template v-slot:text>My team and I created a complex application for train stations around the country. The goal was to work in a team and create mvp, better than competitor's.
    </template>

    <template v-slot:tooltips>
      <tool-tip>Github Projects</tool-tip>
      <tool-tip>Java Spring</tool-tip>
      <tool-tip>PostgreSql</tool-tip>
      <tool-tip>Scrum</tool-tip>
    </template>
  </basic-card>
</div>
</template>

<script>
import BasicCard from "@/components/cards/BasicCard.vue";
import Tooltip from "@/components/Tooltip.vue";

export default {
  name: "AgileCard",
  components: {
    'basic-card': BasicCard,
    'tool-tip': Tooltip
  }
}
</script>

<style scoped>

</style>