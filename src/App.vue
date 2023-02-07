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
        <BasicCard class="api">
          <template v-slot:image>
            <div class="text-center">
              <svg xmlns="http://www.w3.org/2000/svg" width="84" height="84" fill="currenColor" class="bi bi-globe m-2" viewBox="0 0 16 16">
                <path d="M0 8a8 8 0 1 1 16 0A8 8 0 0 1 0 8zm7.5-6.923c-.67.204-1.335.82-1.887 1.855A7.97 7.97 0 0 0 5.145 4H7.5V1.077zM4.09 4a9.267 9.267 0 0 1 .64-1.539 6.7 6.7 0 0 1 .597-.933A7.025 7.025 0 0 0 2.255 4H4.09zm-.582 3.5c.03-.877.138-1.718.312-2.5H1.674a6.958 6.958 0 0 0-.656 2.5h2.49zM4.847 5a12.5 12.5 0 0 0-.338 2.5H7.5V5H4.847zM8.5 5v2.5h2.99a12.495 12.495 0 0 0-.337-2.5H8.5zM4.51 8.5a12.5 12.5 0 0 0 .337 2.5H7.5V8.5H4.51zm3.99 0V11h2.653c.187-.765.306-1.608.338-2.5H8.5zM5.145 12c.138.386.295.744.468 1.068.552 1.035 1.218 1.65 1.887 1.855V12H5.145zm.182 2.472a6.696 6.696 0 0 1-.597-.933A9.268 9.268 0 0 1 4.09 12H2.255a7.024 7.024 0 0 0 3.072 2.472zM3.82 11a13.652 13.652 0 0 1-.312-2.5h-2.49c.062.89.291 1.733.656 2.5H3.82zm6.853 3.472A7.024 7.024 0 0 0 13.745 12H11.91a9.27 9.27 0 0 1-.64 1.539 6.688 6.688 0 0 1-.597.933zM8.5 12v2.923c.67-.204 1.335-.82 1.887-1.855.173-.324.33-.682.468-1.068H8.5zm3.68-1h2.146c.365-.767.594-1.61.656-2.5h-2.49a13.65 13.65 0 0 1-.312 2.5zm2.802-3.5a6.959 6.959 0 0 0-.656-2.5H12.18c.174.782.282 1.623.312 2.5h2.49zM11.27 2.461c.247.464.462.98.64 1.539h1.835a7.024 7.024 0 0 0-3.072-2.472c.218.284.418.598.597.933zM10.855 4a7.966 7.966 0 0 0-.468-1.068C9.835 1.897 9.17 1.282 8.5 1.077V4h2.355z"/>
              </svg>
              <svg xmlns="http://www.w3.org/2000/svg" width="84" height="84" fill="currentColor" class="bi bi-database-lock m-2" viewBox="0 0 16 16">
                <path d="M13 5.698a4.92 4.92 0 0 1-.904.525C11.022 6.711 9.573 7 8 7s-3.022-.289-4.096-.777A4.92 4.92 0 0 1 3 5.698V7c0 .374.356.875 1.318 1.313C5.234 8.729 6.536 9 8 9c.666 0 1.298-.056 1.876-.156-.43.31-.804.693-1.102 1.132A12.31 12.31 0 0 1 8 10c-1.573 0-3.022-.289-4.096-.777A4.92 4.92 0 0 1 3 8.698V10c0 .374.356.875 1.318 1.313C5.234 11.729 6.536 12 8 12h.027a4.548 4.548 0 0 0-.017.8A1.9 1.9 0 0 0 8 13c-1.573 0-3.022-.289-4.096-.777A4.916 4.916 0 0 1 3 11.698V13c0 .374.356.875 1.318 1.313C5.234 14.729 6.536 15 8 15c0 .363.097.704.266.997C8.178 16 8.089 16 8 16c-1.573 0-3.022-.289-4.096-.777C2.875 14.755 2 14.007 2 13V4c0-1.007.875-1.755 1.904-2.223C4.978 1.289 6.427 1 8 1s3.022.289 4.096.777C13.125 2.245 14 2.993 14 4v4.256a4.493 4.493 0 0 0-1.753-.249C12.787 7.654 13 7.289 13 7V5.698Zm-8.682-3.01C3.356 3.124 3 3.625 3 4c0 .374.356.875 1.318 1.313C5.234 5.729 6.536 6 8 6s2.766-.27 3.682-.687C12.644 4.875 13 4.373 13 4c0-.374-.356-.875-1.318-1.313C10.766 2.271 9.464 2 8 2s-2.766.27-3.682.687Z"/>
                <path d="M9 13a1 1 0 0 1 1-1v-1a2 2 0 1 1 4 0v1a1 1 0 0 1 1 1v2a1 1 0 0 1-1 1h-4a1 1 0 0 1-1-1v-2Zm3-3a1 1 0 0 0-1 1v1h2v-1a1 1 0 0 0-1-1Z"/>
              </svg>
              <svg xmlns="http://www.w3.org/2000/svg" width="74" height="74" fill="currentColor" class="bi bi-lightning m-2" viewBox="0 0 16 16">
                <path d="M5.52.359A.5.5 0 0 1 6 0h4a.5.5 0 0 1 .474.658L8.694 6H12.5a.5.5 0 0 1 .395.807l-7 9a.5.5 0 0 1-.873-.454L6.823 9.5H3.5a.5.5 0 0 1-.48-.641l2.5-8.5zM6.374 1 4.168 8.5H7.5a.5.5 0 0 1 .478.647L6.78 13.04 11.478 7H8a.5.5 0 0 1-.474-.658L9.306 1H6.374z"/>
              </svg>
            </div>
            </template>
          <template v-slot:title>API for local IT business</template>
          <template v-slot:text></template>
          <template v-slot:tooltips>
            <Tooltip>Python</Tooltip>
            <Tooltip>Sql Server</Tooltip>
            <Tooltip>something else</Tooltip>
          </template>
        </BasicCard>
      </div>
      <div class="col">
        <BasicCard class="android">
          <template v-slot:image>
            <div class="text-center m-2">
              <svg xmlns="http://www.w3.org/2000/svg" width="184" height="184" fill="#3ddc84" class="bi bi-android" viewBox="0 0 16 16">
                <path d="M2.76 3.061a.5.5 0 0 1 .679.2l1.283 2.352A8.94 8.94 0 0 1 8 5a8.94 8.94 0 0 1 3.278.613l1.283-2.352a.5.5 0 1 1 .878.478l-1.252 2.295C14.475 7.266 16 9.477 16 12H0c0-2.523 1.525-4.734 3.813-5.966L2.56 3.74a.5.5 0 0 1 .2-.678ZM5 10a1 1 0 1 0 0-2 1 1 0 0 0 0 2Zm6 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2Z"/>
              </svg>
            </div>
          </template>
          <template v-slot:title>Mobile App for local IT business</template>
          <template v-slot:text>Useful tool for workers in IT power company. This app helps collect data and manage records about city areas.</template>
          <template v-slot:tooltips>
            <Tooltip>Kotlin</Tooltip>
            <Tooltip>Jetpack Compose</Tooltip>
            <Tooltip>SQLite</Tooltip>
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
