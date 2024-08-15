<template>
  <section id="sectionFour">
    <div
      class="container-fluid"
      style="
        padding-left: 5%;
        padding-right: 5%;
        padding-top: 3%;
        padding-bottom: 5%;
        background-color: #0077b6;
        padding: 5%;
      "
    >
      <div class="row">
        <h1 class="title">
          CURSO DE INGLÊS PARA PROFISSIONAIS DA INDÚSTRIA FARMACÊUTICA
        </h1>
        <div
          class="col-lg-6"
          style="
            display: flex;
            align-items: center;
            justify-content: center;
            flex-direction: column;
          "
        >
          <div class="card">
            <p class="card-text">
              O CURSO DE INGLÊS PARA INDÚSTRIA FARMACÊUTICA tem como objetivo
              proporcionar aos profissionais do setor as habilidades necessárias
              para se comunicar efetivamente em Inglês usando a terminologia da
              indústria farmacêutica.
            </p>
          </div>
          <img src="../assets/image1.png" alt="" style="width: 80%" />
          <div class="card">
            <p class="card-text">
              Vocabulário de Garantia e Controle da Qualidade, Pesquisa &
              Desenvolvimento, Produção e Embalagem, Assuntos Regulatórios e
              muito mais !
            </p>
          </div>
        </div>
        <div class="col-lg-6">
          <img
            src="../assets/Pharmacy-Illustration.png"
            alt=""
            style="width: 80%;"
          />
          <div class="card">
            <p class="card-text">
              O curso aborda vocabulário específico da indústria, expressões
              idiomáticas utilizadas no ambiente de trabalho, revisão de
              gramática, phrasal verbs da área de negócios, entre outros tópicos
              relevantes.
            </p>
          </div>
          <img src="../assets/tiny.png" alt="" width="80%" />
        </div>
      </div>
    </div>
  </section>
</template>

<script lang="ts">
import { ref } from "vue";

export default {
  setup() {},
};
</script>


<style scoped>
.title {
  font-weight: 600;
  font-family: Georgia, "Times New Roman", Times, serif;
  color: whitesmoke;
  text-align: center;
  letter-spacing: 2px;
}

.card {
  padding: 3%;
  background-color: #8e44ad;
  margin-top: 7%;
  margin-bottom: 3%;
  font-family: Georgia, "Times New Roman", Times, serif;
  color: white;
  font-size: 22px;
  text-align: left;
}
</style>