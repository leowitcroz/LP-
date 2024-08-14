<template>
  <div>
    <nav class="navbar">
      <div class="container-fluid" style="background-color: #005583">
        <ul>
          <li><a @click="scrollToSection('sectionOne')">Sessão 1</a></li>
          <li><a @click="scrollToSection('sectionTwo')">Sessão 2</a></li>
          <li><a @click="scrollToSection('sectionThree')">Sessão 3</a></li>
          <li><a @click="scrollToSection('sectionFour')">Sessão 4</a></li>
        </ul>
      </div>
    </nav>

    <SectionOneView />
    <SectionTwoView />
    <SectionThreeView />
    <SectionFourView />
  </div>
</template>
  
  <script setup lang="ts">
import SectionOneView from "./SectionOneView.vue";
import SectionTwoView from "./SectionTwoView.vue";
import SectionThreeView from "./SectionThreeView.vue";
import SectionFourView from "./SectionFourView.vue";

function scrollToSection(sectionId: string) {
  const section = document.getElementById(sectionId);
  if (section) {
    section.scrollIntoView({ behavior: "smooth" });
  }
}
</script>
  
  <style scoped>
.navbar {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  background-color: #005583;
  z-index: 1000; /* Garante que a navbar fique acima de outros elementos */
}

nav ul {
  list-style-type: none;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 15px;
  margin-top: 1%;
}

nav ul li {
  margin-right: 10px;
}

nav ul li a {
  text-decoration: none;
  color: white !important  ;
  font-weight: bold;
}

nav ul li a:hover {
  text-decoration: underline !important;
  cursor: pointer;
}
</style>
  