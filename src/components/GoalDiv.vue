<template>
  <!-- Footer -->
  <div class="text-lg-start text-center bg-body-tertiary text-muted" >
    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
      <path fill="#57126c" fill-opacity="1"
        d="M0,128L40,149.3C80,171,160,213,240,218.7C320,224,400,192,480,181.3C560,171,640,181,720,197.3C800,213,880,235,960,229.3C1040,224,1120,192,1200,176C1280,160,1360,160,1400,160L1440,160L1440,320L1400,320C1360,320,1280,320,1200,320C1120,320,1040,320,960,320C880,320,800,320,720,320C640,320,560,320,480,320C400,320,320,320,240,320C160,320,80,320,40,320L0,320Z">
      </path>
    </svg>
    <div class="radialGradient mycontainer text-white row" id="GoalDiv" style="padding-bottom: 40px;">
      <div class="row  " style="" >
        <h1 class="title ">Goal</h1>
      </div>
      <div class="wrapper-cards">
        <div class="row wrapper-card-line">
          <div class="col-md-6 goal-item mb-5">
            <div class="icon-container">
              <i class="fa-solid fa-award fa-4x "></i>
            </div>
            <h2>ORIENTAÇÃO PARA O SUCESSO:</h2>
            <p>Na IOacademy, acreditamos que o sucesso está ligado ao esforço, dedicação e apreciação da vida.
              Valorizamos uma abordagem holística para alcançar o sucesso em todas as áreas da vida.</p>
          </div>
          <div class="col-md-6 goal-item mb-5">
            <div class="icon-container">
              <i class="fa-solid fa-graduation-cap fa-4x"></i>
            </div>
            <h2>EDUCAÇÃO EM PRIMEIRO LUGAR:</h2>
            <p>Priorizamos a educação contínua e valorizamos os resultados académicos dos nossos alunos. Acreditamos que
              a educação é fundamental para o crescimento pessoal e profissional.</p>
          </div>
        </div>
        <div class="row wrapper-card-line" st>
          <div class="col-md-6 goal-item mb-5">
            <div class="icon-container">
              <i class="fa-solid fa-briefcase fa-4x"></i>
            </div>
            <h2>DESAFIOS PROFISSIONAIS:</h2>
            <p>Oferecemos desafios profissionais aos nossos alunos mais talentosos. Acreditamos que enfrentar desafios é
              essencial para o crescimento e desenvolvimento profissional.</p>
          </div>
          <div class="col-md-6 goal-item mb-5" >
            <div class="icon-container">
              <i class="fa-solid fa-chalkboard-user fa-4x d-flex"></i>
            </div>
            <h2>FORMAÇÃO CONTÍNUA:</h2>
            <p>Promovemos uma cultura de aprendizagem contínua. Acreditamos que a educação não termina após a formação
              académica inicial e incentivamos a busca por oportunidades de aprendizagem ao longo da vida.</p>
          </div>
        </div>
      </div>
    </div>
    
  </div>
  <!-- Footer -->

</template>

<script>
export default {
  name: 'GoalDiv',


}



</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.row{
  --bs-gutter-x:0px;
}

.radialGradient {
  background: rgb(87, 18, 108);

}

.mycontainer {
  display: flex;
  justify-content: space-between;
  flex-direction: row;
  padding-left: 15%;
  padding-right: 15%;
  
}

.wrapper-cards {
  display: flex;
  flex-wrap: wrap;
  flex-direction: row;
  
}
.wrapper-card-line{
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  gap: 50px;
  
}

.goal-item {
  padding: 2rem;
  border-radius: 20px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.5);
}

.goal-item h2 {
  font-size: 1.5rem;
  margin-bottom: 1rem;
  display: flex;
  justify-content: center;

}


.title  {

  font-weight: bold;
  text-align: center;
  transition: color 0.3s ease;
  padding: 0% 0% 5% 0%;
}
.goal-item p {
  font-size: 1rem;
}

.icon-container {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: rem;
}
</style>
