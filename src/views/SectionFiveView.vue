<template>
  <section id="sectionFive">
    <div
      class="container-fluid"
      style="
        padding-left: 5%;
        padding-right: 5%;
        padding-top: 3%;
        padding-bottom: 5%;
      "
    >
      <div class="row">
        <h1 class="title">GLOSSÁRIO – INGLÊS PARA INDÚSTRIA FARMACÊUTICA</h1>
        <div class="mainBox col-lg-6">
          <img src="../assets/image4.png" alt="" style="width: 100%" />
        </div>
        <div class="col-lg-6">
          <div class="card text">
            <p>
              Que tal um e-book no formato de glossário com
              <b>todos os termos importantes da indústria farmacêutica em Inglês?</b>
            </p>
            <p>Parece algo bom demais para ser verdade, não é?!</p>
            <p>
              Pois esse e-book GLOSSÁRIO já existe e você pode adquiri-lo
              clicando no link abaixo:
            </p>
          </div>
          <button class="btn">
            e-book GLOSSÁRIO DE TERMOS EM INGLÊS PARA INDÚSTRIA FARMACÊUTICA
          </button>
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

.logo {
  border: 1px solid red;
  padding: 20px;
  border-radius: 100%;
}
.logomainBox {
  font-size: 5rem;
}

.btn {
  margin-top: 5%;
  background-color: #34a853;
  border-radius: 8px;
  display: inline-block;
  cursor: pointer;
  color: #ffffff;
  font-family: Arial;
  font-size: 15.5px;
  font-weight: bold;
  padding: 13px 32px;
  text-decoration: none;
  text-shadow: 0px 1px 0px #3d768a;
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

.text {
  display: flex;
  flex-direction: column;
  justify-content: left;
  text-align: left;
  font-size: 20px; 
  margin-top: 15%;
}

.mainBox {
  font-family: Georgia, "Times New Roman", Times, serif;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  padding: 3%;
  margin-top: 1%;
}

.title {
  font-weight: 600;
  font-family: Georgia, "Times New Roman", Times, serif;
  margin-top: 3%;
}

.card {
  padding: 5%;
  background-color: #8e44ad;
  font-family: Georgia, "Times New Roman", Times, serif;
  color: white;
}
</style>