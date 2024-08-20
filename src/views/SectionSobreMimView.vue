<template>
  <section id="sectionThree">
    <div
      class="container-fluid"
      style="
        padding-left: 5%;
        padding-right: 5%;
        padding-top: 3%;
        padding-bottom: 5%;
        border-bottom: 2px solid #0077b6;
        background-color: whitesmoke;
      "
    >
      <div class="row">
        <h1 class="title">Sobre a SC Idiomas</h1>
        <div class="col-lg-6" style="margin-top: 3%">
          <div class="box">
            <div class="card">
              <p class="card-text">
                Eu sou a Simone Cunha - Teacher, Farmacêutica Industrial e
                Tradutora.
              </p>
              <p class="card-text">Sou a Fundadora da SC Idiomas.</p>
              <p class="card-text">
                Tenho vivência internacional, participação em reuniões e
                eventos, além de aplicar treinamentos em países da América
                Latina, EUA, Inglaterra, Nova Zelândia, Singapura e outros.
                Cursos de Inglês na Califórnia e Austrália, onde morei e atuei
                como Farmacêutica, tendo a oportunidade de aprimorar meus
                conhecimentos de Inglês.
              </p>
              <p class="card-text">
                Ao voltar da Austrália, em 2015, fundei a SC Idiomas e desde
                então sou empreendedora na área de idiomas, atuando como
                professora particular de Inglês e tradutora técnica.
              </p>
              <p class="card-text">
                Lembro-me da minha jornada para aprender Inglês, o quanto foram
                desgastantes os cursos padronizados oferecidos, e o quanto essa
                jornada poderia ter sido encurtada e com melhores resultados
                através aulas particulares. Com esse objetivo, criei a SC
                Idiomas em 2015, com o intuito de oferecer Aulas Particulares a
                um Preço Acessível.
              </p>
              <p class="card-text">
                Após alguns anos, já tendo concluído minha formação em Tradução,
                dei início aos trabalhos de tradução e versão em Português –
                Inglês – Espanhol.
              </p>
              <p class="card-text">
                A cada novo pedido de tradução, sinto que tenho novamente a
                oportunidade de colocar meus conhecimentos em prática e oferecer
                um trabalho confiável.
              </p>
              <p class="card-text">
                Sinto-me realizada em proporcionar aulas e cursos de Inglês de
                acordo com a necessidade específica de cada pessoa.
              </p>
              <p class="card-text">
                Para mim, cada cliente é um desafio que se transforma em uma
                jornada gratificante por poder levar minha contribuição às
                conquistas profissionais e pessoais dessa pessoa.
              </p>
            </div>
          </div>
        </div>
        <div
          class="col-lg-6"
          style="
            margin-top: 3.5%;
            display: flex;
            flex-direction: column;
            align-items: center;
          "
        >
          <img
            src="../assets/profile.jpeg"
            alt=""
            style="
              width: 60%;
              margin-top: 4%;
              border-radius: 10px;
              border: 3px solid #8e44ad;
            "
          />
          <div class="card" style="background-color: #3ca558; width: 60%; padding: 10px;">
           <h5 style="padding-top: 5px;"> Você me encontra nos canais abaixo:</h5>
           <ul style="text-align: left; margin-top: 5%;">
            <li><a style="color: whitesmoke;" href="https://www.linkedin.com/in/teachersimone/">https://www.linkedin.com/in/teachersimone/</a></li>
            <li><a style="color: whitesmoke;" href="https://www.instagram.com/sc_idiomas/">https://www.instagram.com/sc_idiomas/</a> </li>
            <li>WhatsApp: (11) 97374-1976</li>
            <li>sc.inglespanhol@hotmail.com</li>
           </ul>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
  
  <script lang="ts">
import { ref } from "vue";

export default {
  setup() {
    const card_texts = ref([
      {
        text: "",
      },
      {
        text: "Traduções e versão confiáveis, feitas por profissionais com formação, competência e experiência para garantir a adaptabilidade, mas sem perder a fidelidade ao texto original. ",
      },
      {
        text: "Prazo de entrega e qualidade levados muito a sério. Fique tranquilo em relação à qualidade do serviço e prazo de entrega.",
      },
    ]);

    return {
      card_texts,
    };
  },
};
</script>
  
  
  <style scoped>
.title {
  font-weight: 600;
  font-family: Georgia, "Times New Roman", Times, serif;
  margin-top: 3%;
}

.card {
  padding: 3%;
  background-color: #8e44ad;
  margin-top: 5%;
  font-family: Georgia, "Times New Roman", Times, serif;
  color: white;
}
.card-text {
  font-size: 18px;
  text-align: left;
}
</style>