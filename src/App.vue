<script setup>
import { RouterLink, RouterView } from "vue-router";
import gameArea from "@/components/gameArea.vue";
</script>

<template>
  <div>
    <nav class="barre">
      <div class="rl1">
        <router-link to="/">HUMAN BENCHMARK</router-link>
        <router-link to="/">DASHBOARD</router-link>
      </div>
      <div class="rl2">
        <router-link to="/">SIGN UP</router-link>
        <router-link to="/">LOGIN</router-link>
      </div>
    </nav>
  </div>
  <gameArea />
  <RouterView />
</template>

<style scoped>
.barre {
  display: flex;
  gap: 20%;
}

.rl1 {
  display: flex;
  gap: 2%;
  margin-left: 20%;
}

.rl2 {
  display: flex;
  gap: 5%;
  margin-right: 20%;
}


a {
 color: black;
text-decoration: none;

}

</style>
