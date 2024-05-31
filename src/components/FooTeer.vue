<template>
  <!-- Footer -->
  <footer class="text-center text-lg-start bg-body-tertiary text-muted">
    <!-- Section: Social media -->

    <!-- Section: Social media -->

    <!-- Section: Links  -->
    <section class="" style="background-color: rgba(0, 0, 0, 0.2);">
      <div class="container text-center text-md-start">
        <!-- Grid row -->
        <div class="row ">
          <!-- Grid column -->
          <div class="col-md-1 col-lg-2 col-xl-3  mb-4 mt-4">
            <!-- Content -->
            <h6 class="text-uppercase fw-bold mb-4 ">
              <i class=" "></i><img src="@/assets/img/ioacadamy.png" width="75%" height="75%"
                class="d-inline-block align-top">
            </h6>
            <p>
              Here you can use rows and columns to organize your footer content. Lorem ipsum
              dolor sit amet, consectetur adipisicing elit.
            </p>
          </div>
          <!-- Grid column -->

          <!-- Grid column -->
          <div class="col-md-1 col-lg-1 mx-auto mb-4 mt-5">
            <!-- Links -->
            <h6 class="text-uppercase fw-bold mb-4">
              Links
            </h6>
            <p>
              <a href="#!" class="text-reset" @click="irParaAboutUs">AboutUs</a>
            </p>
            <p>
              <a href="#!" class="text-reset" @click="irParaGoalDiv">Goal</a>
            </p>
            <p>
              <a href="#!" class="text-reset" @click="irParaChallenge">Challange</a>
            </p>
            <p>
              <a href="#!" class="text-reset" @click="irParaContactos">Contact US</a>
            </p>
          </div>
          <!-- Grid column -->

          <!-- Grid column -->

          <!-- Grid column -->

          <!-- Grid column -->
          <div class="col-md-3 col-lg-4 col-xl-5  mb-md-0 mb-4 mt-5">
            <!-- Links -->
            <h6 class="text-uppercase fw-bold mb-4">Office</h6>
            <p><i class="fas fa-home "></i> Avenida Dom Afonso Henriques 4694, Vila Nova de Famalicão</p>
            <p>
              <i class="fas fa-envelope"></i> info@iotech.pt
            </p>
            <p><i class="fas fa-phone "></i> +351 252 116 943</p>
            <p><i class="fas fa-print "></i> +351 302 002 958</p>
          </div>
          <!-- Grid column -->



        </div>
        <!-- Grid row -->
      </div>
    </section>
    <!-- Section: Links  -->

    <!-- Copyright -->

    <!-- Copyright -->
  </footer>
  <!-- Footer -->

</template>

<script>
export default {
  name: 'FooTeer',

  methods: {
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
    irParaContactos() {
      const aboutUsSection = document.getElementById('Contactos');
      if (aboutUsSection) {
        aboutUsSection.scrollIntoView({ behavior: 'smooth' });
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
