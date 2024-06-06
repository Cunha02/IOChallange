<template>
  <nav class="navbar navbar-expand-lg border-bottom border-body mycontainer" data-bs-theme="dark"
    style="background-color: #57126c ;">
    <a class="navbar-brand" href="#">
      <img src="@/assets/img/iotech.png" width="164" height="64" class="d-inline-block align-top">
    </a>
    <div>
      <button class="navbar-toggler" type="button" @click="toggleNavbar" data-bs-toggle="collapse"
        data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link " aria-current="page" href="#" @click="irParaAboutUs">AboutUs</a>
          </li>
          <li class="nav-item">
            <a class="nav-link " aria-current="page" href="#" @click="irParaGoalDiv">Goal</a>
          </li>
          <li class="nav-item">
            <a class="nav-link " aria-current="page" href="#" @click="irParaChallenge">Challange</a>
          </li>
          <li class="nav-item">
            <a class="nav-link " aria-current="page" href="#"  @click="irParaBenefits" >Benefits</a>
          </li>
        </ul>
      </div>
    </div>

  </nav>
</template>

<script>
export default {
  name: 'NavBar',

  methods: {
    toggleNavbar() {
      // Altera o estado do menu de navegação
      const navbarNav = document.getElementById('navbarNav');
      navbarNav.classList.toggle('show');
    },
    irParaAboutUs() {
      const aboutUsSection = document.getElementById('AboutUs');
      if (aboutUsSection) {
        aboutUsSection.scrollIntoView({ behavior: 'smooth' });
      }
    },
    irParaGoalDiv() {
      const aboutUsSection = document.getElementById('GoalDiv');
      if (aboutUsSection) {
        aboutUsSection.scrollIntoView({ behavior: 'smooth' });
      }
    },
    irParaChallenge() {
      const aboutUsSection = document.getElementById('Challenge');
      if (aboutUsSection) {
        aboutUsSection.scrollIntoView({ behavior: 'smooth' });
      }
    },
    irParaBenefits() {
      const aboutUsSection = document.getElementById('Benefits');
      if (aboutUsSection) {
        aboutUsSection.scrollIntoView({ behavior: 'smooth' });
      }
    }
  }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.mycontainer {
  position: fixed;
  top: 0;
  width: 100%;
  z-index: 1000;
  display: flex;
  justify-content: space-between;
  flex-direction: row;
  padding-left: 15%;
  padding-right: 15%;
}
</style>
