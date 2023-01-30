<script setup>

import Navbar from "@/components/Navbar.vue";

import AndroidCard1 from "@/components/cards/AndroidCard1.vue";
import AlgorithmCard from "@/components/cards/AlgorithmCard.vue";
import Tooltip from "@/components/Tooltip.vue";
import DevopsCard from "@/components/cards/DevopsCard.vue";
</script>

<template>

  <header>
    <Navbar></Navbar>
  </header>

  <h1 class="display-1">My projects</h1>

  <div id="devops-projects" class="cards-content-R-L">
    <DevopsCard>
      <template v-slot:image><div class="card-img-top p-4">PENDING</div></template>
      <template v-slot:title>This Website</template>
      <template v-slot:text></template>
      <template v-slot:tooltips>
        <Tooltip>node.js</Tooltip>
        <Tooltip>Vue.js</Tooltip>
        <Tooltip>Bootstrap</Tooltip>
        <Tooltip>DevOps</Tooltip>
      </template>
    </DevopsCard>
    <DevopsCard>
      <template v-slot:image><div class="card-img-top p-4">PENDING</div></template>
      <template v-slot:title>IaS</template>
      <template v-slot:text></template>
      <template v-slot:tooltips>
        <Tooltip>Terraform</Tooltip>
        <Tooltip>Linux</Tooltip>
      </template>
    </DevopsCard>
    <DevopsCard class="">
      <template v-slot:image><div class="card-img-top p-4">PENDING</div></template>
      <template v-slot:title>CI/CD</template>
      <template v-slot:text></template>
      <template v-slot:tooltips>
        <Tooltip>Docker</Tooltip>
        <Tooltip>Jenkins</Tooltip>
        <Tooltip>AWS</Tooltip>
      </template>
    </DevopsCard>
    <DevopsCard class="start-10">
      <template v-slot:image><div class="card-img-top p-4">PENDING</div></template>
      <template v-slot:title>CI/CD</template>
      <template v-slot:text></template>
      <template v-slot:tooltips>
        <Tooltip>Docker</Tooltip>
        <Tooltip>Jenkins</Tooltip>
        <Tooltip>AWS</Tooltip>
      </template>
    </DevopsCard>
  </div>

  <div id="android-projects" class="cards-content-L-R">
      <div class="col">
        <AndroidCard1 :card-number="'card1'"/>
      </div>
    <div class="row align-items-center">
      <div class="col">
        <AndroidCard1 :card-number="'card2'"/>
      </div>
    </div>
  </div>

  <div id="uni-basics-projects" class="cards-content-even">

    <div class="row align-items-center">
      <div class="col">
        <AlgorithmCard :card-number="'card2'">
          <template v-slot:image>
            <div class="card-img-top p-4" alt="..."></div>
          </template>
          <template v-slot:title>Github Requests</template>
          <template v-slot:tooltips>
            <Tooltip>Git</Tooltip>
            <Tooltip>Python</Tooltip>
            <Tooltip>Github-API</Tooltip>
          </template>
        </AlgorithmCard>
        <AlgorithmCard :card-number="'card2'">
          <template v-slot:image>
            <div class="card-img-top p-4" alt="..."></div>
          </template>
          <template v-slot:title>Team Project</template>
          <template v-slot:text>My team and I worked on a complex project...</template>

          <template v-slot:tooltips>
            <Tooltip>Github Projects</Tooltip>
            <Tooltip>Java Spring</Tooltip>
            <Tooltip>PostgreSql</Tooltip>
            <Tooltip>Scrum</Tooltip>
          </template>
        </AlgorithmCard>
      </div>
    </div>

    <div class="row align-items-center">
      <div class="col">

        <AlgorithmCard  :card-number="'card1'">
          <template v-slot:image><div class="card-img-top p-4" alt="..."></div></template>
          <template v-slot:title>Algorithms & Data structures</template>
          <template v-slot:text>Leetcode solutions with nice-looking boxing. <br> I created Markdown generator to wrap
            up my solutions and related test cases.
          </template>
          <template v-slot:tooltips>
            <Tooltip>Git</Tooltip>
            <Tooltip>Markdown</Tooltip>
            <Tooltip>Python</Tooltip>
            <Tooltip>Java</Tooltip>
          </template>
        </AlgorithmCard>

      </div>
    </div>

  </div>


</template>

<style scoped>

</style>
