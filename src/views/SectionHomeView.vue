<template>
  <section id="sectionOne">
    <div
      class="container-fluid"
      style="
        padding-left: 5%;
        padding-right: 5%;
        padding-top: 3%;
        padding-bottom: 5%;
        background-color: whitesmoke;
      "
    >
      <div class="row">
        <h1 class="title">AULAS PARTICULARES DE INGLÊS & MENTORIA</h1>
        <div class="mobile" style="padding: 5%">
          <img
            class="img_mobile"
            src="../assets/logo2.png"
            alt="image"
            style="width: 50%"
          />
        </div>

        <div class="mainBox col-lg-6">
          <div class="card text">
            <h3 style="margin-bottom: 3%; margin-top: 1%; font-size: 1.5rem">
              Aprenda ou aprimore seu inglês da melhor forma:
            </h3>
            <li>Aulas particulares ao vivo</li>
            <li>Programa de mentoria</li>
            <li style="text-align: left">
              Inglês personalizado de acordo <span>com sua necessidade</span>
            </li>
            <li style="margin-bottom: 1%; text-align: left">
              Inglês para viagens, negócios e etc
            </li>
          </div>
          <button class="btn">
            <a
              href="https://wa.me/5511973741976?text=Tenho%20interesse/aprimorar%20meu%20INGLÊS

"
              >Clique aqui para um plano de ação de Inglês específico para
              você</a
            >
          </button>
        </div>
        <div class="col-lg-6">
          <img
            class="img"
            src="../assets/pana.png"
            alt="image"
            style="width: 90%"
          />
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
        text: " Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis facere nam distinctio consequuntur nulla dolor sint sed odio non quia rem molestias at aut repellat, obcaecati mollitia atque, error quos",
      },
      {
        text: " Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis facere nam distinctio consequuntur nulla dolor sint sed odio non quia rem molestias at aut repellat, obcaecati mollitia atque, error quos",
      },
      {
        text: " Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis facere nam distinctio consequuntur nulla dolor sint sed odio non quia rem molestias at aut repellat, obcaecati mollitia atque, error quos",
      },
    ]);

    return {
      card_texts,
    };
  },
};
</script>
  
  
  <style scoped>
@import url("https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400..700&family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap");

.btn {
  margin-top: 5%;
  background-color: #34a853;
  border-radius: 8px;
  display: inline-block;
  cursor: pointer;
  color: #ffffff;
  font-family: Arial;
  font-size: 14.5px;
  font-weight: bold;
  padding: 13px 32px;
  text-decoration: none;
  text-shadow: 0px 1px 0px #3d768a;
}
.btn a {
  color: whitesmoke;
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
.img_mobile {
  display: none;
}
.mobile {
  display: none;
}

.text {
  display: flex;
  flex-direction: column;
  justify-content: left;
  align-items: baseline;
  margin-top: 5%;
}
.text li {
  margin-top: 2%;
  font-size: 1.3rem;
}

.mainBox {
  font-family: Georgia, "Times New Roman", Times, serif;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}

.title {
  font-weight: 600;
  font-family: Georgia, "Times New Roman", Times, serif;
  margin-top: 8%;
  color: rgb(51, 51, 51);
}

.card {
  padding: 5%;
  background-color: #0077b6;
  font-family: Georgia, "Times New Roman", Times, serif;
  color: white;
}

@media only screen and (max-width: 767px) {
  .title {
    font-size: 1.5rem;
  }

  .text li {
    margin-top: 2%;
    font-size: 0.7rem;
  }

  .btn {
    font-size: 12px;
    margin-bottom: 3%;
  }
}

@media only screen and (min-width: 768px) and (max-width: 1024px) {
  .navbar {
    display: none;
  }
}
</style>