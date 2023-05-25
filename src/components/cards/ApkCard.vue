<template>
<div>
  <basic-card id="d1" class="devops" v-bind:lnk="'https://github.com/alexarlord-boop/app/blob/main/.github/workflows/generate-apk-aab-debug-release.yml'">
    <template v-slot:image>
      <svg xmlns="http://www.w3.org/2000/svg" width="9rem" height="9rem"
           class="bi bi-infinity rota m-0 animated" viewBox="0 0 16 16">
        <path
            d="M5.68 5.792 7.345 7.75 5.681 9.708a2.75 2.75 0 1 1 0-3.916ZM8 6.978 6.416 5.113l-.014-.015a3.75 3.75 0 1 0 0 5.304l.014-.015L8 8.522l1.584 1.865.014.015a3.75 3.75 0 1 0 0-5.304l-.014.015L8 6.978Zm.656.772 1.663-1.958a2.75 2.75 0 1 1 0 3.916L8.656 7.75Z"/>
      </svg>
    </template>
    <template v-slot:small-icon>
<!--      <svg xmlns="http://www.w3.org/2000/svg" width="25" height="25" fill="currentColor" class="bi bi-hammer" viewBox="0 0 16 16">-->
<!--      <path d="M9.972 2.508a.5.5 0 0 0-.16-.556l-.178-.129a5.009 5.009 0 0 0-2.076-.783C6.215.862 4.504 1.229 2.84 3.133H1.786a.5.5 0 0 0-.354.147L.146 4.567a.5.5 0 0 0 0 .706l2.571 2.579a.5.5 0 0 0 .708 0l1.286-1.29a.5.5 0 0 0 .146-.353V5.57l8.387 8.873A.5.5 0 0 0 14 14.5l1.5-1.5a.5.5 0 0 0 .017-.689l-9.129-8.63c.747-.456 1.772-.839 3.112-.839a.5.5 0 0 0 .472-.334z"/>-->
<!--    </svg>-->
    </template>
    <template v-slot:title>APK Builder</template>
    <template v-slot:text>CI pipeline that automates Android APK building.
      <br> This pipeline generates debug and release APKs, which you can download right after a code base has changed.

    </template>
    <template v-slot:tooltips>
      <tool-tip>GitHub Actions</tool-tip>
      <tool-tip>Gradle</tool-tip>
    </template>
  </basic-card>
</div>
</template>

<script>
import BasicCard from "@/components/cards/BasicCard.vue";
import Tooltip from "@/components/Tooltip.vue";

export default {
  name: "ApkCard",
  components: {
    'basic-card': BasicCard,
    'tool-tip': Tooltip
  }
}
</script>

<style scoped>

</style>