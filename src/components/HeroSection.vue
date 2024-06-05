<template>
  <div style="background-color: #57126c;">
    <div class="hero-section ">
      <!-- Hero Section -->

      <div class="hero-content">
        <h1>Bem-Vindo à IOacademy</h1>
        <p>Prepare-se para o sucesso com a nossa educação de excelência. Na IOacademy, proporcionamos uma formação
          contínua e atualizada para garantir o seu crescimento pessoal e profissional.</p>
      </div>

      <!-- Cards Section -->
      <div class="cards-section row justify-content-center">
        <div class="card col-md-2">
          <i class="fa-solid fa-trophy fa-3x mb-3" style="color: #57126c;"></i>
          <h5 class="card-title">FORMAÇÃO</h5>
          <p class="card-text">Cursos flexíveis e continuamente atualizados, assegurando que os participantes mantenham
            um conhecimento avançado e relevante.</p>
        </div>
        <div class="card col-md-2">
          <i class="fa-solid fa-book fa-3x mb-3" style="color: #57126c;"></i>
          <h5 class="card-title">TECNOLOGIAS EMERGENTES</h5>
          <p class="card-text">Formação prática em tecnologias como Internet das Coisas (IoT) e outras inovações
            tecnológicas.</p>
        </div>
        <div class="card col-md-2">
          <i class="fa-solid fa-briefcase fa-3x mb-3" style="color: #57126c;"></i>
          <h5 class="card-title">PROJETOS INOVADORES</h5>
          <p class="card-text">Aceite o desafio e desenvolva um projeto numa das nossas áreas de ponta. Prove que está
            pronto para a ioAcademy.</p>
        </div>
        <div class="card col-md-2">
          <i class="fa-solid fa-graduation-cap fa-3x mb-3" style="color: #57126c;"></i>
          <h5 class="card-title">MENTORIA ESPECIALIZADA</h5>
          <p class="card-text">Suporte contínuo e personalizado para ajudar a alcançar o máximo potencial e crescer na
            carreira.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HeroSection',
}
</script>

<style scoped>
.hero-section {
  height: 150vh;
  background: linear-gradient(rgba(0, 0, 0, 0.3), rgba(0, 0, 0, 0.1)),
    url('@/assets/img/hero.png') center/cover no-repeat;
  /* Substitua pelo caminho da sua imagem */
  background-size: cover;
  background-position: center;
  position: relative;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;

}

.hero-content {
  position: relative;
  z-index: 2;
  max-width: 900px;
  margin-top: 190px;
}

.cards-section {
  z-index: 2;
  display: flex;
  flex-wrap: wrap;
  margin-top: 300px;
  /* Ajuste conforme necessário */
 
  justify-content: center;
  opacity: 75%;
}

.hero-content h1 {

  font-size: 4rem;
}

.hero-content p {

  font-size: 1.4rem;
}

.card {
  background-color: #fff;
  color: #000;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  text-align: center;
  padding: 25px;
  margin: 10px;
  /* Adiciona espaçamento entre os cards */
  max-width: 100%;
}




.card i {
  margin-bottom: 10px;
}

.card-title {
  font-size: 1.1rem;
  margin-bottom: 15px;
}

.card-text {
  font-size: 1rem;
  margin-bottom: 10px;
}


.row {
  --bs-gutter-x: 0px;
}
</style>
