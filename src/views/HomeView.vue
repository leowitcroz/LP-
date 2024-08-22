<template>
  <div>
    <nav class="navbar">
      <div class="container-fluid" style="background-color: #005583">
        <div class="row">
          <div class="col-11" style="display: flex; justify-content: center;">
            <ul>
              <li>
                <a @click="scrollToSection('sectionOne')"
                  >AULAS PARTICULARES DE INGLÊS
                </a>
              </li>
              <li>
                <a @click="scrollToSection('sectionTwo')"
                  >PROGRAMAS DE ACELERAÇÃO DE INGLÊS</a
                >
              </li>
              <li>
                <a @click="scrollToSection('sectionFour')"
                  >INGLÊS PARA PROFISSIONAIS DA INDÚSTRIA FARMACÊUTICA
                </a>
              </li>
              <li>
                <a @click="scrollToSection('sectionFive')"
                  >GLOSSÁRIO DE INGLÊS
                </a>
              </li>
              <li><a @click="scrollToSection('sectionThree')">TRADUÇÃO </a></li>
            </ul>
          </div>
          <div class="col-1">
            <img
              width="70%"
              src="../assets/Logo.png"
              alt=""
              style="margin-top: 7px; margin-right: 10px; margin-bottom: 7px"
            />
          </div>
        </div>
      </div>
    </nav>

    <SectionHomeView />
    <SectionCursoView />
    <SectionAceleracaoView />
    <SectionGlossarioView />
    <SectionTraducaoView />
    <SectionSobreMimView />

    <footer style="background-color: #005583">
      <p class="copyrights">
        Icon made by Pixel perfect from
        <a href="https://storyset.com/work" style="color: whitesmoke;">Work illustrations by Storyset</a>
      </p>
      <p class="copyrights">
        <a style="color: whitesmoke;"
          href="https://www.freepik.com/free-vector/tiny-pharmacist-with-pills-vitamins-flat-vector-illustration-doctors-writing-prescriptions-antibiotics-working-together-helping-patients-cure-pharmacy-business-drugstore-concept_24644990.htm#query=pharmacy%20illustration&position=9&from_view=keyword&track=ais_hybrid&uuid=a399f5fb-3c8c-4c54-93d9-8cc26387ac94"
          >Image by pch.vector</a
        >
        on Freepik
      </p>
    </footer>
  </div>
</template>
  
  <script setup lang="ts">
import SectionHomeView from "./SectionHomeView.vue";
import SectionAceleracaoView from "./SectionAceleracaoView.vue";
import SectionTraducaoView from "./SectionTraducaoView.vue";
import SectionCursoView from "./SectionCursoView.vue";
import SectionGlossarioView from "./SectionGlossarioView.vue";
import SectionSobreMimView from "./SectionSobreMimView.vue";

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
  font-size: 13px;
}

nav ul li a:hover {
  text-decoration: underline !important;
  cursor: pointer;
}

footer {
  padding: 1%;
}

.copyrights {
  margin: 0 !important;
  color: whitesmoke;
}

@media only screen and (max-width: 767px) {
  .navbar {
    display: none;
  }

  .copyrights{
    font-size: 10px;
  }
}


@media only screen and (min-width: 768px) and (max-width: 1024px){
  .navbar {
    display: none;
  }
}

@media only screen and (min-width: 1024px) and (max-width: 1420px){

nav ul li a {
text-decoration: none;
color: white !important  ;
font-weight: bold;
font-size: 12px;
}
}
</style>

  