<template>
  <section id="sectionOne">
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
        <div class="title col-lg-6">
          <h1>
            Domine o Inglês para Impulsionar Sua Carreira na Indústria
            Farmacêutica
          </h1>
        </div>
        <div class="col-lg-6">
          <img
            src="../assets/Tiny pharmacist with pills and vitamins flat vector illustration.jpg"
            alt=""
            style="width: 100%; margin-top: 10%"
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

.logo {
  border: 1px solid red;
  padding: 20px;
  border-radius: 100%;
}
.logoTitle {
  font-size: 5rem;
}

.title {
  font-family: Georgia, "Times New Roman", Times, serif;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}

.card {
  padding: 3%;
  background-color: #8e44ad;
  margin-top: 5%;
  font-family: Georgia, "Times New Roman", Times, serif;
  color: white;
}
</style>