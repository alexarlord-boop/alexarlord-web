<script setup>

import Navbar from "@/components/Navbar.vue";

import Tooltip from "@/components/Tooltip.vue";
import BasicCard from "@/components/cards/BasicCard.vue";
</script>

<template>

  <header>
    <Navbar></Navbar>
  </header>


  <h1 class="display-1 mt-3">My projects</h1>

  <div id="cards-column" class="col mt-5">

    <div id="devops-projects" class="row align-items-sm-start cards-content-even">
      <div class="col">
        <BasicCard v-bind:lnk="'https://github.com/alexarlord-boop/alexarlord-web'" class="golographic">
          <template v-slot:image>
            <img src="src/images/infinity.png" alt="devops-card" class="card-img-top p-0 rounded-5"/>
          </template>
          <template v-slot:title>This Website</template>
          <template v-slot:text>This site is about my multiskill personality. <br> I tried myself and succeed in many different IT fields. Here you can find my essential projects, which I personally enjoyed working on and would like to share with you.
            <br>I strive for elegant solution!
          </template>
          <template v-slot:tooltips>
            <Tooltip>Vue.js</Tooltip>
            <Tooltip>Bootstrap</Tooltip>
            <Tooltip>Github Pages</Tooltip>
          </template>
        </BasicCard>
      </div>
      <div class="col">
        <h1 class="display-6 text-center">DevOps</h1>
        <BasicCard class="devops">
          <template v-slot:image>
            <div class="card-img-top p-4"/>
          </template>
          <template v-slot:title>IaC</template>
          <template v-slot:text>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum aliquet metus
            auctor, vehicula turpis a, vehicula metus.
          </template>
          <template v-slot:tooltips>
            <Tooltip>Terraform</Tooltip>
            <Tooltip>Ansible</Tooltip>
          </template>
        </BasicCard>
        <BasicCard class="devops">
          <template v-slot:image><div class="card-img-top p-4"/></template>
          <template v-slot:title>CI/CD</template>
          <template v-slot:text>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum aliquet metus
            auctor, vehicula turpis a, vehicula metus.
          </template>
          <template v-slot:tooltips>
            <Tooltip>Docker</Tooltip>
            <Tooltip>Jenkins</Tooltip>
            <Tooltip>AWS</Tooltip>
          </template>
        </BasicCard>
      </div>
    </div>

    <h1 class="display-6 text-center">Software</h1>
    <div id="android-projects" class="row align-items-center cards-content-left-over-right">
      <div class="col">
        <BasicCard class="android">
          <template v-slot:image><img src="src/images/unnamed.jpeg" alt="android-card" class="card-img-top p-4"/></template>
          <template v-slot:title>Application for local IT business</template>
          <template v-slot:text>Useful tool for workers in IT power company. This app helps collect data and manage records about city areas.</template>
          <template v-slot:tooltips>
            <Tooltip>Kotlin</Tooltip>
            <Tooltip>Vanilla Android</Tooltip>
          </template>
        </BasicCard>
      </div>
      <div class="col">
        <BasicCard class="android">
          <template v-slot:image><img src="src/images/android.png" alt="android-card" class="card-img-top p-4"/></template>
          <template v-slot:title>Application for local IT business</template>
          <template v-slot:text>Useful tool for workers in IT power company. This app helps collect data and manage records about city areas.</template>
          <template v-slot:tooltips>
            <Tooltip>Kotlin</Tooltip>
            <Tooltip>Jetpack Compose</Tooltip>
            <Tooltip>Material Design</Tooltip>
          </template>
        </BasicCard>
      </div>

    </div>

    <h1 class="display-6 text-center">Basics</h1>
    <div id="uni-basics-projects" class="row cards-content-even">

      <div class="col">
        <BasicCard v-bind:lnk="'https://github.com/alexarlord-boop/python_au/tree/main/requests'" class="sideproject" :card-number="'card2'">
          <template v-slot:image>
            <div class="card-img-top p-4"></div>
          </template>
          <template v-slot:title>Github Requests</template>
          <template v-slot:tooltips>
            <Tooltip>Git</Tooltip>
            <Tooltip>Python</Tooltip>
            <Tooltip>Github-API</Tooltip>
          </template>
        </BasicCard>
        <BasicCard v-bind:lnk="'https://github.com/alexarlord-boop/union-station'" class="sideproject" :card-number="'card2'">
          <template v-slot:image>
            <div class="card-img-top p-4"></div>
          </template>
          <template v-slot:title>Team Project</template>
          <template v-slot:text>My team and I worked on a complex project...</template>

          <template v-slot:tooltips>
            <Tooltip>Github Projects</Tooltip>
            <Tooltip>Java Spring</Tooltip>
            <Tooltip>PostgreSql</Tooltip>
            <Tooltip>Scrum</Tooltip>
          </template>
        </BasicCard>
      </div>
      <div class="col">
        <BasicCard v-bind:lnk="'https://github.com/alexarlord-boop/java-au'" class="sideproject" :card-number="'card1'">
          <template v-slot:image>
            <div class="card-img-top p-4"></div>
          </template>
          <template v-slot:title>Algorithms & Data structures</template>
          <template v-slot:text>Leetcode solutions with nice-looking boxing. <br> I created Markdown generator to wrap
            up my solutions and related test cases.
          </template>
          <template v-slot:tooltips>
            <Tooltip>Git</Tooltip>
            <Tooltip>Markdown</Tooltip>
            <Tooltip>Java</Tooltip>
          </template>
        </BasicCard>
      </div>

    </div>
  </div>

</template>

<style scoped>

</style>
