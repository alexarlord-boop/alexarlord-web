<script setup>

import Navbar from "@/components/Navbar.vue";

import Tooltip from "@/components/Tooltip.vue";
import BasicCard from "@/components/cards/BasicCard.vue";
import FooterLink from "@/components/FooterLink.vue";
import FooterHead from "@/components/FooterHead.vue";
import FooterLinks from "@/components/FooterLinks.vue";
import Avatar from "@/components/Avatar.vue";
</script>

<template>

  <header>
    <Navbar></Navbar>
  </header>


  <h1 class="display-1 mt-3">My projects</h1>

  <div class="col mt-5 custom-grid">
    <div id="devops-projects" class="row align-items-sm-start">
      <div class="col">
        <BasicCard v-bind:lnk="'https://github.com/alexarlord-boop/alexarlord-web'" class="golographic">
          <template v-slot:image>
            <svg xmlns="http://www.w3.org/2000/svg" width="9rem" height="9rem"
                 class="bi bi-infinity rota m-0 animated" viewBox="0 0 16 16">
              <path
                  d="M5.68 5.792 7.345 7.75 5.681 9.708a2.75 2.75 0 1 1 0-3.916ZM8 6.978 6.416 5.113l-.014-.015a3.75 3.75 0 1 0 0 5.304l.014-.015L8 8.522l1.584 1.865.014.015a3.75 3.75 0 1 0 0-5.304l-.014.015L8 6.978Zm.656.772 1.663-1.958a2.75 2.75 0 1 1 0 3.916L8.656 7.75Z"/>
            </svg>
          </template>
          <template v-slot:small-icon>
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="#fff" class="bi bi-github"
                 viewBox="0 0 16 16">
              <path
                  d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"/>
            </svg>
          </template>
          <template v-slot:title>This Website</template>
          <template v-slot:text>
            This site is dedicated to my multidisciplinary personality. I have tried and excelled in many different
            areas of IT. On this page you can find my main projects that I really enjoyed working on and would like to
            share with you.
            <br>
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
              <h1 class="display-6 text-center m-5">Cloud</h1>
              <BasicCard class="devops">
                <template v-slot:image>
                  <div class="card-img-top p-4"/>
                </template>
                <template v-slot:title>APK Builder</template>
                <template v-slot:text>CI/CD configuration in cloud. The general purpose is to automate APK building for Android app.
                </template>
                <template v-slot:tooltips>
                  <Tooltip>GitHub Actions</Tooltip>
                  <Tooltip></Tooltip>
                </template>
              </BasicCard>
              <BasicCard class="devops">
                <template v-slot:image>
                  <div class="card-img-top p-4"/>
                </template>
                <template v-slot:title>Cool Project</template>
                <template v-slot:text>CI/CD configuration in cloud. The general purpose is to automate APK building for Android app.
                </template>
                <template v-slot:tooltips>
                  <Tooltip>AWS</Tooltip>
                </template>
              </BasicCard>
            </div>
    </div>

    <div id="android-projects" class="row align-items-center cards-content-left-over-right">
      <div class="col">
        <h1 class="display-6 text-center m-5">Software</h1>
        <BasicCard class="api">
          <template v-slot:image>

            <svg xmlns="http://www.w3.org/2000/svg" width="5rem" height="5rem" fill="black" class="bi bi-globe m-3"
                 viewBox="0 0 16 16">
              <path
                  d="M0 8a8 8 0 1 1 16 0A8 8 0 0 1 0 8zm7.5-6.923c-.67.204-1.335.82-1.887 1.855A7.97 7.97 0 0 0 5.145 4H7.5V1.077zM4.09 4a9.267 9.267 0 0 1 .64-1.539 6.7 6.7 0 0 1 .597-.933A7.025 7.025 0 0 0 2.255 4H4.09zm-.582 3.5c.03-.877.138-1.718.312-2.5H1.674a6.958 6.958 0 0 0-.656 2.5h2.49zM4.847 5a12.5 12.5 0 0 0-.338 2.5H7.5V5H4.847zM8.5 5v2.5h2.99a12.495 12.495 0 0 0-.337-2.5H8.5zM4.51 8.5a12.5 12.5 0 0 0 .337 2.5H7.5V8.5H4.51zm3.99 0V11h2.653c.187-.765.306-1.608.338-2.5H8.5zM5.145 12c.138.386.295.744.468 1.068.552 1.035 1.218 1.65 1.887 1.855V12H5.145zm.182 2.472a6.696 6.696 0 0 1-.597-.933A9.268 9.268 0 0 1 4.09 12H2.255a7.024 7.024 0 0 0 3.072 2.472zM3.82 11a13.652 13.652 0 0 1-.312-2.5h-2.49c.062.89.291 1.733.656 2.5H3.82zm6.853 3.472A7.024 7.024 0 0 0 13.745 12H11.91a9.27 9.27 0 0 1-.64 1.539 6.688 6.688 0 0 1-.597.933zM8.5 12v2.923c.67-.204 1.335-.82 1.887-1.855.173-.324.33-.682.468-1.068H8.5zm3.68-1h2.146c.365-.767.594-1.61.656-2.5h-2.49a13.65 13.65 0 0 1-.312 2.5zm2.802-3.5a6.959 6.959 0 0 0-.656-2.5H12.18c.174.782.282 1.623.312 2.5h2.49zM11.27 2.461c.247.464.462.98.64 1.539h1.835a7.024 7.024 0 0 0-3.072-2.472c.218.284.418.598.597.933zM10.855 4a7.966 7.966 0 0 0-.468-1.068C9.835 1.897 9.17 1.282 8.5 1.077V4h2.355z"/>
            </svg>
            <svg xmlns="http://www.w3.org/2000/svg" width="5rem" height="5rem" fill="black" class="bi bi-lightning m-3"
                 viewBox="0 0 16 16">
              <path
                  d="M5.52.359A.5.5 0 0 1 6 0h4a.5.5 0 0 1 .474.658L8.694 6H12.5a.5.5 0 0 1 .395.807l-7 9a.5.5 0 0 1-.873-.454L6.823 9.5H3.5a.5.5 0 0 1-.48-.641l2.5-8.5zM6.374 1 4.168 8.5H7.5a.5.5 0 0 1 .478.647L6.78 13.04 11.478 7H8a.5.5 0 0 1-.474-.658L9.306 1H6.374z"/>
            </svg>
            <svg xmlns="http://www.w3.org/2000/svg" width="5rem" height="5rem" fill="black"
                 class="bi bi-database-lock m-3" viewBox="0 0 16 16">
              <path
                  d="M13 5.698a4.92 4.92 0 0 1-.904.525C11.022 6.711 9.573 7 8 7s-3.022-.289-4.096-.777A4.92 4.92 0 0 1 3 5.698V7c0 .374.356.875 1.318 1.313C5.234 8.729 6.536 9 8 9c.666 0 1.298-.056 1.876-.156-.43.31-.804.693-1.102 1.132A12.31 12.31 0 0 1 8 10c-1.573 0-3.022-.289-4.096-.777A4.92 4.92 0 0 1 3 8.698V10c0 .374.356.875 1.318 1.313C5.234 11.729 6.536 12 8 12h.027a4.548 4.548 0 0 0-.017.8A1.9 1.9 0 0 0 8 13c-1.573 0-3.022-.289-4.096-.777A4.916 4.916 0 0 1 3 11.698V13c0 .374.356.875 1.318 1.313C5.234 14.729 6.536 15 8 15c0 .363.097.704.266.997C8.178 16 8.089 16 8 16c-1.573 0-3.022-.289-4.096-.777C2.875 14.755 2 14.007 2 13V4c0-1.007.875-1.755 1.904-2.223C4.978 1.289 6.427 1 8 1s3.022.289 4.096.777C13.125 2.245 14 2.993 14 4v4.256a4.493 4.493 0 0 0-1.753-.249C12.787 7.654 13 7.289 13 7V5.698Zm-8.682-3.01C3.356 3.124 3 3.625 3 4c0 .374.356.875 1.318 1.313C5.234 5.729 6.536 6 8 6s2.766-.27 3.682-.687C12.644 4.875 13 4.373 13 4c0-.374-.356-.875-1.318-1.313C10.766 2.271 9.464 2 8 2s-2.766.27-3.682.687Z"/>
              <path
                  d="M9 13a1 1 0 0 1 1-1v-1a2 2 0 1 1 4 0v1a1 1 0 0 1 1 1v2a1 1 0 0 1-1 1h-4a1 1 0 0 1-1-1v-2Zm3-3a1 1 0 0 0-1 1v1h2v-1a1 1 0 0 0-1-1Z"/>
            </svg>

          </template>
          <template v-slot:small-icon>
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="#fff" class="bi bi-github"
                 viewBox="0 0 16 16">
              <path
                  d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"/>
            </svg>
          </template>
          <template v-slot:title>API for local IT business</template>
          <template v-slot:text>
            This API is created to help gathering and updating data from the power company server. The API is a
            complementary software, which is used via android application.
          </template>
          <template v-slot:tooltips>
            <Tooltip>Python</Tooltip>
            <Tooltip>Sql Server</Tooltip>
            <Tooltip>Stoplight</Tooltip>
          </template>
        </BasicCard>
      </div>
      <div class="col">
        <BasicCard class="android">
          <template v-slot:image>
            <div class="text-center m-2">
              <svg xmlns="http://www.w3.org/2000/svg" width="184" height="184" fill="#3ddc84" class="bi bi-android"
                   viewBox="0 0 16 16">
                <path
                    d="M2.76 3.061a.5.5 0 0 1 .679.2l1.283 2.352A8.94 8.94 0 0 1 8 5a8.94 8.94 0 0 1 3.278.613l1.283-2.352a.5.5 0 1 1 .878.478l-1.252 2.295C14.475 7.266 16 9.477 16 12H0c0-2.523 1.525-4.734 3.813-5.966L2.56 3.74a.5.5 0 0 1 .2-.678ZM5 10a1 1 0 1 0 0-2 1 1 0 0 0 0 2Zm6 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2Z"/>
              </svg>
            </div>
          </template>
          <template v-slot:title>Mobile App for local IT business</template>
          <template v-slot:text>Useful tool for workers in IT power company. This app helps collect data and manage
            records about city areas.
          </template>
          <template v-slot:tooltips>
            <Tooltip>Android</Tooltip>
            <Tooltip>Kotlin</Tooltip>
            <Tooltip>SQLite</Tooltip>
          </template>
        </BasicCard>
      </div>

    </div>

    <h1 class="display-6 text-center m-5">Basics</h1>
    <div id="uni-basics-projects" class="cards-content-right-over-left">
      <div class="col">
        <BasicCard v-bind:lnk="'https://github.com/alexarlord-boop/python_au/tree/main/requests'" class="git"
                   :card-number="'card2'">
          <template v-slot:image>
            <svg xmlns="http://www.w3.org/2000/svg" width="5rem" height="5rem" fill="#fcd40c" class="bi bi-tools m-3"
                 viewBox="0 0 16 16">
              <path
                  d="M1 0 0 1l2.2 3.081a1 1 0 0 0 .815.419h.07a1 1 0 0 1 .708.293l2.675 2.675-2.617 2.654A3.003 3.003 0 0 0 0 13a3 3 0 1 0 5.878-.851l2.654-2.617.968.968-.305.914a1 1 0 0 0 .242 1.023l3.27 3.27a.997.997 0 0 0 1.414 0l1.586-1.586a.997.997 0 0 0 0-1.414l-3.27-3.27a1 1 0 0 0-1.023-.242L10.5 9.5l-.96-.96 2.68-2.643A3.005 3.005 0 0 0 16 3c0-.269-.035-.53-.102-.777l-2.14 2.141L12 4l-.364-1.757L13.777.102a3 3 0 0 0-3.675 3.68L7.462 6.46 4.793 3.793a1 1 0 0 1-.293-.707v-.071a1 1 0 0 0-.419-.814L1 0Zm9.646 10.646a.5.5 0 0 1 .708 0l2.914 2.915a.5.5 0 0 1-.707.707l-2.915-2.914a.5.5 0 0 1 0-.708ZM3 11l.471.242.529.026.287.445.445.287.026.529L5 13l-.242.471-.026.529-.445.287-.287.445-.529.026L3 15l-.471-.242L2 14.732l-.287-.445L1.268 14l-.026-.529L1 13l.242-.471.026-.529.445-.287.287-.445.529-.026L3 11Z"/>
            </svg>
          </template>
          <template v-slot:small-icon>
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="#fcd40c" class="bi bi-github"
                 viewBox="0 0 16 16">
              <path
                  d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"/>
            </svg>
          </template>
          <template v-slot:title>Github Requests</template>
          <template v-slot:text>
            This project is about using Github API to improve the teamwork experience.<br> You can use it to check the
            naming of commits, pull requests, and comments.<br>
            <br>
            30+ developers used this project.
          </template>
          <template v-slot:tooltips>
            <Tooltip>Git</Tooltip>
            <Tooltip>Python</Tooltip>
            <Tooltip>Github-API</Tooltip>
          </template>
        </BasicCard>
      </div>
      <div class="col">
        <BasicCard v-bind:lnk="'https://github.com/alexarlord-boop/union-station'" class="git">
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
          <template v-slot:text>My team and I created a complex application for train stations around the country. <br>
            We united as a team and used the Agile Scrum approach.
          </template>

          <template v-slot:tooltips>
            <Tooltip>Github Projects</Tooltip>
            <Tooltip>Java Spring</Tooltip>
            <Tooltip>PostgreSql</Tooltip>
            <Tooltip>Scrum</Tooltip>
          </template>
        </BasicCard>
        <BasicCard v-bind:lnk="'https://github.com/alexarlord-boop/java-au'" class="sideproject">
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
            <Tooltip>Git</Tooltip>
            <Tooltip>Markdown</Tooltip>
            <Tooltip>Java</Tooltip>
          </template>
        </BasicCard>
      </div>
    </div>
  </div>

  <p class="row"></p>
  <p class="row"></p>
  <p class="row"></p>
  <p class="row"></p>
  <p class="row"></p>
  <p class="row"></p>
  <p class="row"></p>


  <div id="contact-section" class="text-center" @mouseover="initLink"
       @mouseleave="ejectLink">

    <div class=" custom-more-info custom-grid">

      <div class="row">
        <div class="col-6 align-self-center text-end">
          <FooterLinks>
            <FooterLink id="clicked" class="clicked">github</FooterLink>
            <FooterLink>linkedin</FooterLink>
          </FooterLinks>
        </div>
        <div class="col-6 text-start">
          <FooterLinks>
            <FooterLink>telegram</FooterLink>
          </FooterLinks>
        </div>
      </div>
      <!--      <div class="col m-5 float-end"-->
      <!--           data-bs-toggle="popover" data-bs-placement="right"-->
      <!--           data-bs-custom-class="custom-popover"-->
      <!--           data-bs-title="Custom popover"-->
      <!--           data-bs-content="This popover is themed via CSS variables."-->
      <!--      >-->
      <!--        <div class="animation shadow-lg rounded-3">-->
      <!--          <svg xmlns="http://www.w3.org/2000/svg" width="6rem" height="6rem" fill="currentColor" class="bi bi-arrows-fullscreen align-self-center" viewBox="-2 -2 20 20">-->
      <!--            <path fill-rule="evenodd" d="M5.828 10.172a.5.5 0 0 0-.707 0l-4.096 4.096V11.5a.5.5 0 0 0-1 0v3.975a.5.5 0 0 0 .5.5H4.5a.5.5 0 0 0 0-1H1.732l4.096-4.096a.5.5 0 0 0 0-.707zm4.344 0a.5.5 0 0 1 .707 0l4.096 4.096V11.5a.5.5 0 1 1 1 0v3.975a.5.5 0 0 1-.5.5H11.5a.5.5 0 0 1 0-1h2.768l-4.096-4.096a.5.5 0 0 1 0-.707zm0-4.344a.5.5 0 0 0 .707 0l4.096-4.096V4.5a.5.5 0 1 0 1 0V.525a.5.5 0 0 0-.5-.5H11.5a.5.5 0 0 0 0 1h2.768l-4.096 4.096a.5.5 0 0 0 0 .707zm-4.344 0a.5.5 0 0 1-.707 0L1.025 1.732V4.5a.5.5 0 0 1-1 0V.525a.5.5 0 0 1 .5-.5H4.5a.5.5 0 0 1 0 1H1.732l4.096 4.096a.5.5 0 0 1 0 .707z"/>-->
      <!--          </svg>-->
      <!--        </div>-->
      <!--      </div>-->

    </div>
    <div id="page-bottom"></div>
  </div>

</template>

<script>
export default {
  methods: {
    initLink() {
      // let pageBottom = document.querySelector("#page-bottom")
      // setTimeout(() => {
      //   pageBottom.scrollIntoView({behavior: "smooth"})
      // }, 500)
      //

      let clickedLnk = document.querySelector("#clicked")
      setTimeout(() => {
        clickedLnk.classList.remove("clicked")
      }, 500)
    },
    ejectLink() {
      let clickedLnk = document.querySelector("#clicked")

      setTimeout(() => {
        clickedLnk.classList.add("clicked")
      }, 500)
    }
  }
}

</script>

<style lang="sass">

.animated
  stroke-dasharray: 200
  stroke-dashoffset: 100
  pointer-events: none
  animation: animateDash 5s linear forwards infinite

@keyframes animateDash
  to
    stroke-dashoffset: 50


.animation
  width: 6rem
  height: 6rem
//border: 1px solid #000

</style>
