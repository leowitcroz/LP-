<template>
  <section id="sectionFour">
    <div
      class="container-fluid"
      style="
        padding-left: 5%;
        padding-right: 5%;
        padding-top: 3%;
        padding-bottom: 5%;
        border-top: 2px solid #0077b6;
        border-bottom: 2px solid #0077b6;
        background-color: whitesmoke;
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
          <div class="card" style="margin-top: 10%">
            <p class="card-text">
              O CURSO DE INGLÊS PARA INDÚSTRIA FARMACÊUTICA tem como objetivo
              proporcionar aos profissionais do setor as habilidades necessárias
              para se comunicar efetivamente em Inglês usando a terminologia da
              indústria farmacêutica.
            </p>
          </div>
          <div class="card">
            <p class="card-text">
              Vocabulário de Garantia e Controle da Qualidade, Pesquisa &
              Desenvolvimento, Produção e Embalagem, Assuntos Regulatórios e
              muito mais !
            </p>
          </div>
          <div class="card">
            <p class="card-text">
              O curso aborda vocabulário específico da indústria, expressões
              idiomáticas utilizadas no ambiente de trabalho, revisão de
              gramática, phrasal verbs da área de negócios, entre outros tópicos
              relevantes.
            </p>
          </div>
        </div>
        <div class="col-lg-6">
          <img
            class="img"
            src="../assets/image1.png"
            alt=""
            style="width: 100%"
          />

          <button class="btn">
            <a href="https://chk.eduzz.com/2291402">
              Clique aqui para mais informações sobre o curso</a
            >
          </button>
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
  color: rgb(51, 51, 51);
  text-align: center;
  letter-spacing: 2px;
}

.btn {
  margin-top: 5%;
  font-size: 20px;
  background-color: #34a853;
  border-radius: 8px;
  display: inline-block;
  cursor: pointer;
  color: #ffffff;
  font-weight: bold;
  padding: 13px 32px;
  text-decoration: none;
}

.btn a {
  color: #ffffff;
  text-decoration: none;
}
.btn:hover {
  text-decoration: underline;
  background-color: #3ca558;
  color: #ffffff;
}
.btn:active {
  position: relative;
  top: 1px;
}

.card {
  padding: 3%;
  background-color: #8e44ad;
  margin-bottom: 3%;
  font-family: Georgia, "Times New Roman", Times, serif;
  color: white;
  font-size: 22px;
  text-align: left;
}

@media only screen and (max-width: 767px) {
  .title {
    font-size: 1.2rem;
  }

  .card {
    font-size: 13px;
  }

  .btn {
    font-size: 10px;
    margin-bottom: 3%;
  }
}
</style>