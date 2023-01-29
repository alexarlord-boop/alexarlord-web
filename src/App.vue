<script setup>

import Navbar from "@/components/Navbar.vue";

import AndroidCard1 from "@/components/cards/AndroidCard1.vue";
</script>

<template>

  <header>
    <Navbar></Navbar>
  </header>

  <h1 class="display-1">My projects</h1>

  <div id="cards-content-L-R">
    <AndroidCard1 :card-number="'card1'"/>
    <AndroidCard1 :card-number="'card2'"/>
  </div>

  <div id="cards-content-R-L">
    <AndroidCard1 :card-number="'card1'"/>
    <AndroidCard1 :card-number="'card2'"/>
  </div>


</template>

<style scoped>

</style>
