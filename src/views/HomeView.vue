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
          <li><a @click="scrollToSection('sectionFour')">PROFISSIONAIS DA INDÚSTRIA FARMACÊUTICA </a></li>
          <li><a @click="scrollToSection('sectionFive')">GLOSSÁRIO </a></li>
          <li><a @click="scrollToSection('sectionThree')">TRADUÇÃO </a></li>
        </ul>
      </div>
    </nav>

    <SectionHomeView />
    <SectionCursoView />
    <SectionAceleracaoView />
    <SectionGlossarioView/>
    <SectionTraducaoView />

    <footer style="background-color: #005583">
      <p class="copyrights" >Icon made by Pixel perfect from <a href="https://storyset.com/work">Work illustrations by Storyset</a></p>
      <p class="copyrights" ><a href="https://www.freepik.com/free-vector/tiny-pharmacist-with-pills-vitamins-flat-vector-illustration-doctors-writing-prescriptions-antibiotics-working-together-helping-patients-cure-pharmacy-business-drugstore-concept_24644990.htm#query=pharmacy%20illustration&position=9&from_view=keyword&track=ais_hybrid&uuid=a399f5fb-3c8c-4c54-93d9-8cc26387ac94">Image by pch.vector</a> on Freepik</p>
    </footer>
  </div>
</template>
  
  <script setup lang="ts">
import SectionHomeView from "./SectionHomeView.vue";
import SectionAceleracaoView from "./SectionAceleracaoView.vue";
import SectionTraducaoView from "./SectionTraducaoView.vue";
import SectionCursoView from "./SectionCursoView.vue";
import SectionGlossarioView from "./SectionGlossarioView.vue";

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

footer{
  padding: 1%;
}

.copyrights{
  margin: 0!important;
  color: whitesmoke;
}
</style>
  