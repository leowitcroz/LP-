<template>
  <div>
    <nav class="navbar">
      <div class="container-fluid" style="background-color: #005583">
        <ul>
          <li>
            <a @click="scrollToSection('sectionOne')"
              >AULAS PARTICULARES
            </a>
          </li>
          <li><a @click="scrollToSection('sectionTwo')">PROGRAMAS DE ACELERAÇÃO</a></li>
          <li><a @click="scrollToSection('sectionThree')">TRADUÇÃO </a></li>
          <li><a @click="scrollToSection('sectionFour')">PROFISSIONAIS DA INDÚSTRIA FARMACÊUTICA </a></li>
          <li><a @click="scrollToSection('sectionFour')">GLOSSÁRIO </a></li>
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
  font-size: 14px;
}

nav ul li a:hover {
  text-decoration: underline !important;
  cursor: pointer;
}
</style>
  