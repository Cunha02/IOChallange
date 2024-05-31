<template>
  <!-- Footer -->
  <div class="text-center text-lg-start bg-body-tertiary text-muted " style="  font-family: 'Roboto', sans-serif;">
    <div class="radialGradient ">
      <div class="text-white" >
        <!-- 1 linha -->
        <div class="row  wrapper" style="padding-top: 8%;" id="AboutUs">
          <h1 class="title ">About US</h1>
        </div>
        <!-- 2 linha -->
        <div class="row  d-flex justify-content-center align-items-center wrapper" style="padding-bottom: 3%;">
          <div class="col-md-6" style="padding-right: 1.5%;" >
            <h2>IOACADEMY: Educação e Formação de Excelência</h2>
            <p>A empresa iotech criou a ioAcademy, uma academia de formação e investigação destinada a estudantes do
              ensino superior, com o objetivo de captar, formar e reter talentos. A ioAcademy oferece uma oportunidade
              única para os melhores alunos que desejam enfrentar desafios e adquirir experiência profissional durante o
              ano académico.</p>
          </div>
          <div class="col-md-6 " style="padding-left: 1.5%;">
            <img class="imagess" src="@/assets/img/mentoring.png" width="100%" height="100%">
          </div>
        </div>
        <!-- 3 linha -->
        <div class="row text-white justify-content-center align-items-center wrapper" style="padding-bottom: 8%;">
          <div class="col-md-6 " style="padding-right: 1.5%;">
            <img class="imagess" src="@/assets/img/key.png" width="100%" height="100%">
          </div>
          <div class="col-md-6" style="padding-left: 1.5%;">
            <h2>Uma Academia de Formação para os Melhores Alunos</h2>
            <p>Na ioAcademy, acreditamos que a educação deve ser contínua, atualizada e acessível. A nossa missão é
              proporcionar aos estudantes uma formação de alta qualidade, alinhada com as necessidades do mercado, proporcionando lhes a chave para o sucesso</p>
          </div>
        </div>
      </div>
    </div>
    <div class="d-flex justify-content-center align-items-center" style="padding:1%;">
      <h1>O que temos para oferecer</h1>
    </div>

    <div class="card-container" >
      <div class="card">
        <i class="fas fa-graduation-cap fa-4x " style="padding-bottom: 7%; padding-top: 5%;"></i>
        <h3>Formação (Training)</h3>
        <p>Formação Contínua e Atualizada</p>
        <ul>
          
         <li><span style="font-weight: bold;">Contínua:</span> Cursos que promovem aprendizagem contínua.</li> 
         <li><span style="font-weight: bold;">Online:</span> Flexibilidade para aprender ao próprio ritmo, em qualquer lugar.</li> 
         <li><span style="font-weight: bold;">Atualizada:</span> Conteúdos revistos e atualizados com as últimas tendências e tecnologias.</li> 

        </ul>
      </div>
      <div class="card">
        <i class="fa-solid fa-magnifying-glass fa-4x " style="padding-bottom: 7%;  padding-top: 5%;"></i>
        <h3>Investigação (Research)</h3>
        <p>Investigação Aplicada e Inovadora</p>
        <ul>
          <li><span style="font-weight: bold;">Estudos de Caso:</span> Análise de situações reais para desenvolver competências analíticas.</li> 
          <li><span style="font-weight: bold;">Experiências de Laboratório:</span> Testar hipóteses e validar teorias em ambiente controlado.</li> 
          <li><span style="font-weight: bold;">Benchmarking:</span> Comparação com os melhores da indústria para identificar áreas de melhoria.</li> 
 
        </ul>
      </div>
      <div class="card">
        <i class="fa-solid fa-puzzle-piece fa-4x " style="padding-bottom: 7%;  padding-top: 5%;"></i>
        <h3>Experiências (Experiences)</h3>
        <p>Desenvolvimento Prático em Áreas de Ponta</p>
        <ul>
          <li><span style="font-weight: bold;">Desenvolvimento Web (PWA): </span> Criação de aplicações web progressivas.</li> 
          <li><span style="font-weight: bold;">Ciência de Dados:</span>Análise de grandes volumes de dados para insights valiosos.</li> 
          <li><span style="font-weight: bold;">Inteligência Artificial:</span> Desenvolvimento de soluções inteligentes para automação e decisão.</li> 
 
        </ul>
      </div>
      <div class="card">
        <i class="fas fa-user-graduate fa-4x " style="padding-bottom: 7%;  padding-top: 5%;"></i>
        <h3>Mentoria (Mentoring)</h3>
        <p>Apoio Académico e Profissional</p>
        <ul>
          <li><span style="font-weight: bold;">Suporte Académico:</span> Acompanhamento personalizado para superar desafios académicos.</li> 
          <li><span style="font-weight: bold;">Exercícios Motivacionais:</span>Atividades para manter a motivação e o foco.</li> 
          <li><span style="font-weight: bold;">Desafios Profissionais:</span>Projetos reais que preparam para o mercado de trabalho.</li> 
 
        </ul>
      </div>
    </div>


  </div>
  <!-- Footer -->

</template>

<script>
export default {
  name: 'AboutUs',


}



</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.radialGradient {
  
  background: linear-gradient(180deg, rgba(87, 18, 108, 1) 0%, rgba(224, 140, 250, 1) 80%, rgba(224, 140, 250, 0) 100%);
}

.card-container {
  display: flex;
  justify-content: space-evenly;
  padding: 5% 5% 0% 5%;
}

.justifyy {
  display: flex;
  justify-content: space-evenly;
}

.card {
  width: 23%;
  padding: 20px;
  border: 1px solid #ccc;
  border-radius: 5px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  text-align: center;
}

.card h2 {
  margin-top: 0;
}

.card p {
  font-weight: bold;
}

.card i {
  font-size: 24px;
  margin-bottom: 10px;
}

.card li {
  text-align: justify;
}

.wrapper{
  display: flex;
  justify-content: space-between;
  flex-direction: row;
  padding-left: 15%;
  padding-right: 15%;
}

.title  {
  color: #ffffff;
  font-weight: bold;
  text-align: center;
  transition: color 0.3s ease;
  padding-bottom: 5%;
}

.title:hover {
  color: #9c9c9c;
  /* Darker blue on hover for interactivity */
}

.imagess{


border-radius: 10%;
box-shadow: 0 10px 10px rgba(0, 0, 0, 0.1);

}


.row{
  --bs-gutter-x:0px;
}
</style>
