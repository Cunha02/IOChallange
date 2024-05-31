<template>




  <div>


    <div class="mycontainer" style="font-family: 'Roboto', sans-serif; padding: 5% 0%;">


      <!-- Introdução -->
      <div class="introduction-container" style="padding: 5%;">
        <!-- Título -->
        <div class="title" id="Challenge">
          <h1>Bem-vindo ao Challenge!</h1>
        </div>

        <!-- Texto explicativo sobre o desafio -->
        <div class="challenge-description">
          <p>O Challenge é uma oportunidade emocionante para expandir os seus horizontes, desenvolver novas habilidades
            e fazer parte de uma comunidade vibrante de aprendizagem.</p>
          <p>Durante o desafio, os participantes serão desafiados a explorar temas diversos e relevantes, enfrentar
            tarefas estimulantes e crescer pessoal e profissionalmente.</p>
        </div>

        <!-- Pergunta "Estás pronto para o desafio?" -->
        <div class="ready-question">
          <h3>Estás pronto para o desafio?</h3>
        </div>

        <!-- Texto encorajador para escolher um dos temas -->
        <div class="choose-theme">
          <p>Para começar, escolha um dos quatro temas apresentados abaixo. Cada tema oferece uma jornada única e
            desafiadora, repleta de oportunidades de aprendizagem e crescimento.</p>
        </div>

        <!-- Container para a introdução do challenge -->
        <div id="carouselExampleRide" class="carousel slide temascontainer cori" data-bs-ride="true">
          <div class="carousel-inner">
            <div class="carousel-item active">
              <img src="@/assets/img/challange1.png" class="d-block w-100" alt="...">
            </div>
            <div class="carousel-item">
              <img src="@/assets/img/challange2.png" class="d-block w-100" alt="...">
            </div>
            <div class="carousel-item">
              <img src="@/assets/img/challange3.png" class="d-block w-100" alt="...">
            </div>
            <div class="carousel-item">
              <img src="@/assets/img/challange4.png" class="d-block w-100" alt="...">
            </div>
          </div>
          <button class="carousel-control-prev temascontainer" type="button" data-bs-target="#carouselExampleRide"
            data-bs-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Previous</span>
          </button>
          <button class="carousel-control-next temascontainer" type="button" data-bs-target="#carouselExampleRide"
            data-bs-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Next</span>
          </button>
        </div>



      </div>
    </div>











    <div class="timeline">

      <div class=" mycontainer d-flex justify-content-center align-items-center"
        style="padding:5%; font-family: 'Roboto', sans-serif; ">
        <h1>Challenge Timeline</h1>
      </div>


      <div class="row ">
        <div class="col-5">


          <div class="row" style="justify-content: flex-end; padding-bottom:200px;">
            <div class="expandable-card" style=" display: flex; justify-content: flex-end; align-items: center; "
              @mouseover="hoverFirst = true; setProgress(20);" @mouseleave="hoverFirst = false;">
              <div class="card-content leftt">
                <h2>Registration</h2>
                <p>Are you interested in participating?</p>
              </div>
              <div class="card-expanded left" v-if="hoverFirst">
                <h3>Mais Informações</h3>
                <p style="text-align: center;">Submit your application and be ready!</p>
              </div>
            </div>
          </div>


          <div class="row" style=" justify-content: flex-end;">
            <div class="expandable-card " style=" display: flex; justify-content: flex-end; align-items: center;"
              @mouseover="hoverFirst = true; setProgress(70);" @mouseleave="hoverFirst = false;">
              <div class="card-content leftt">
                <h2>PROJECT (30 days)</h2>
                <p>You must develop a solution for the challenge presented.</p>
              </div>
              <div class="card-expanded left" v-if="hoverFirst">
                <h3>Mais Informações</h3>
                <ul>
                  <li>The challenge/project is by area/subject selected.</li>
                  <li>Selected students will receive an email to schedule the presentation date.</li>
                  <li>June, 3 to 7 - Presentation.</li>
                </ul>
              </div>
            </div>
          </div>


        </div>


        <div class="col-2">
          <div class="progress-bar-container">
            <div class="progress-bar" :style="{ height: progressHeight + '%', top: '0' }"></div>
          </div>
        </div>




        <div class="col-5">
          <div class="row" style="justify-content: flex-start; padding-top:250px;">
            <div class="expandable-card" style=" display: flex; justify-content: flex-start; align-items: center; "
              @mouseover="hoverFirst = true; setProgress(40)" @mouseleave="hoverFirst = false;">
              <div class="card-content rightt">
                <h2>Application (online)</h2>
                <p>You must show your skills (soft and technical) and answer two simple questions:</p>
              </div>
              <div class="card-expanded right" v-if="hoverFirst">
                <h3>Mais Informações</h3>
                <ul>
                  <li>Why are you interested in being a member of ioAcademy?</li>
                  <li>How do you hope to make a difference?</li>
                </ul>
                <p>Students will receive an email indicating if they will proceed to the second phase.</p>
              </div>
            </div>
          </div>
          <div class="row" style=" justify-content: flex-start; padding-top:250px;">
            <div class="expandable-card " style=" display: flex; justify-content: flex-start; align-items: center;"
              @mouseover="hoverFirst = true; setProgress(100)" @mouseleave="hoverFirst = false; resetProgress();">
              <div class="card-content rightt">
                <h2>ioAcademy (7 months)*</h2>
                <p>Have you completed all phases successfully? Are you chosen?</p>
              </div>
              <div class="card-expanded right" v-if="hoverFirst">
                <h3>Mais Informações</h3>
                <p>Congratulations, you are now an ioAcademy member. Welcome!</p>
                <p>*Can be renewed at the beginning of each academic semester.</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="titlee" id="Benefits">
      <h1>Beneficios</h1>
    </div>

    <div class="container">
      <div class="section">
        <div class="icon-container">
          <div class="icon ">  <i class="fas fa-user-graduate icon mentoring-icon"></i> <!-- Font Awesome Icon --></div>
        </div>
        <h2>Mentoring</h2>
        <p class="duration">7 Months</p>
        <p>Support for the development of soft and technical skills. Experimenting professional challenges.</p>
      </div>
      <div class="section">
        <div class="icon-container">
          <div class="icon ">  <i class="fas fa-chalkboard-teacher icon training-icon"></i>  <!-- Font Awesome Icon --></div>
        </div>
        <h2>Training</h2>
        <p class="duration">7 Months</p>
        <p>Continuous formation through online-learning platforms.</p>
      </div>
      <div class="section">
        <div class="icon-container">
          <div class="icon ">   <i class="fa-solid fa-laptop-code icon internship-icon "></i> <!-- Google Material Icon --></div>
        </div>
        <h2>Summer Internship*</h2>
        <p class="duration">2 Months</p>
        <p>The possibility of having access to a Summer internship. * Internship is limited to 1 or 2 people and it is attributed according to the results achieved by the student during the training process.</p>
      </div>
    </div>

  </div>




</template>

<script>
export default {
  name: 'ChallengeDiv',
  data() {
    return {
      hoverFirst: false,
      hoverSecond: false,
      progressHeight: 0,
    };
  },
  methods: {
    setProgress(percentage) {
      this.progressHeight = percentage;
    },
    resetProgress() {
      this.progressHeight = 0;
    }
  }
};
</script>

<style scoped>
.mycontainer {
  display: flex;
  flex-direction: column;
  align-items: start;
  padding: 2.5% 15%;
}

.temascontainer {
  display: flex;
  flex-direction: column;
  align-items: start;
  padding: 0% 5%;
  
  
}

.cori{

  border: 3px solid #57126c;
  margin: 5%  15% 0% 15% ;
}


.expandable-card {
  width: 300px;
  height: 300px;
  background: #ffffff;
  border: 1px solid #e0e0e0;
  border-radius: 10px;
  overflow: hidden;
  position: relative;
  transition: width 0.3s ease, box-shadow 0.3s ease;
  font-family: 'Roboto', sans-serif;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  margin: 20px;

}

.expandable-card:hover {
  width: 650px;
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);

}

.expandable-card:hover .rightt {
  padding-right: 410px;

}

.expandable-card:hover .leftt {
  padding-left: 410px;
}

.card-content,
.card-expanded {
  padding: 20px;
  display: flex;
  flex-direction: column;
  justify-content: center;

}



.card-content h2 {
  margin: 0;
  font-size: 1.5em;
  color: #333;
}

.card-content p {
  margin: 10px 0 0;
  font-size: 1em;
  color: #666;
}

.card-expanded {
  position: absolute;
  top: 0;
  height: 100%;
  background: #f9f9f9;
  transition: opacity 0.3s ease;
  opacity: 0;
  text-align: justify;
}

.card-expanded.right {
  right: 0;
  width: 200px;
  border-left: 1px solid #e0e0e0;

}

.card-expanded.left {
  left: 0;
  width: 200px;
  border-right: 1px solid #e0e0e0;
}

.expandable-card:hover .card-expanded {
  opacity: 1;

}

.expandable-card:hover .card-expanded.right,
.expandable-card:hover .card-expanded.left {
  width: 400px;

}

.card-expanded h3 {
  font-size: 1.2em;
  color: #333;
  font-family: 'Roboto', sans-serif;
  text-align: center
}

.card-expanded p {
  margin: 0;
  font-size: 1em;
  color: #666;
  font-family: 'Roboto', sans-serif;
}

.progress-bar-container {
  width: 30px;
  height: 1050px;
  background-color: #f3f3f3;
  border-radius: 20px;
  margin: auto;
  position: relative;
}

.progress-bar {
  width: 100%;
  height: 0;
  background-color: #57126c;
  position: absolute;
  bottom: 0;
  border-radius: 20px;
  transition: height 0.9s ease;
}


.timeline {

  border: 3px solid #57126c;
  border-radius: 15px;
  box-shadow: 0 10px 10px rgba(0, 0, 0, 0.1);
  margin: 0 7%;
}


/* General container styling */
.introduction-container {
  width: 80%;
  margin: auto;
  padding: 20px;
  background-color: #f9f9f9;
  /* Light background for contrast */
  border-radius: 8px;
  /* Rounded corners for a softer look */
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  /* Subtle shadow for depth */
  overflow: hidden;
  /* Ensures the content doesn't overflow the rounded corners */
}

/* Title styling */
.title h1 {
  color: #891caa;
  /* Blue color for emphasis */
  font-weight: bold;
  /* Bold font weight for impact */
  text-align: center;
  /* Centered title */
  transition: color 0.3s ease;
  /* Smooth color transition effect */
  padding-bottom: 3%
}

.titlee h1 {
  color: #891caa;
  /* Blue color for emphasis */
  font-weight: bold;
  /* Bold font weight for impact */
  text-align: center;
  /* Centered title */
  transition: color 0.3s ease;
  /* Smooth color transition effect */
  padding: 5% 0%
}

.title h1:hover {
  color: #57126c;
  /* Darker blue on hover for interactivity */
}

.titlee h1:hover {
  color: #57126c;
  /* Darker blue on hover for interactivity */
}

/* Challenge description styling */
.challenge-description p {
  color: #333;
  /* Slightly darker text for readability */
  font-size: 16px;
  /* Smaller font size for better readability */
  line-height: 1.75;
  /* Increased line height for spaciousness */
  text-align: justify;
  /* Justified text for a formal look */
  margin-bottom: 15px;
  /* Reduced bottom margin for tighter spacing */
}

/* Ready question styling */
.ready-question h3 {
  color: #666;
  /* Softer color for less emphasis than the title */
  font-style: italic;
  /* Italicized text for a subtle difference */
  text-align: center;
  /* Centered question */
  margin-top: 25px;
  /* Adjusted top margin for better spacing */
}

/* Choose theme styling */
.choose-theme p {
  color: #555;
  /* Even softer color for the encouragement text */
  font-style: normal;
  /* Normal font style to differentiate from the question */
  text-align: justify;
  /* Justified text for consistency */
  margin-bottom: 25px;
  /* Adjusted bottom margin for consistency */
}

/* Hover Effect for Encouragement Text */
.choose-theme p:hover {
  color: #777;
  /* Lighter color on hover for a subtle effect */
}









.container {
  display: flex;
  justify-content: space-around;
  text-align: center;
  padding: 8% 0% 5% 0%;
  font-family: 'Roboto', sans-serif;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.5);
}

.section {
  width: 30%;
}

.icon-container {
  width: 80px;
  height: 80px;
  margin: 0 auto 10px;
}

.icon {
  width: 100%;
  height: 100%;
  border-radius: 50%;
  background-size: cover;
  animation: spin 5s linear infinite;
}

.mentoring-icon {
  background-color: #ce6ee6;
  /* Altere o caminho conforme necessário */
}

.training-icon {
  background-color: #ce6ee6;
  /* Altere o caminho conforme necessário */
}

.internship-icon {
  background-color: #ce6ee6;
 /* Altere o caminho conforme necessário */
}

@keyframes spin {
  0% { transform: rotateY(0deg); }
  100% { transform: rotateY(360deg); }
}

h2 {
  font-size: 1.5em;
  margin: 10px 0;
  color: #4A4A4A;
}

.duration {
  font-size: 1.2em;
  font-weight: bold;
  color: #333;
}
</style>
