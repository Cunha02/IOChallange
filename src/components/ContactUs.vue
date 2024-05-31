<template>


<div>
  <h1 class="title " id="Contactos">Contact Us</h1>
</div>



  <div class="mycontainer">
    <div class="mb-3 ">
      <label for="exampleFormControlInput1" class="form-label">Nome Completo</label>
      <input type="text" class="form-control" id="from_name" placeholder="Nome" required>
    </div>
    <div class="mb-3 ">
      <label for="exampleFormControlInput1" class="form-label">Email </label>
      <input type="email" class="form-control" id="email_id" placeholder="name@example.com" required>
    </div>
    <div class="mb-3">
      <label for="exampleFormControlTextarea1" class="form-label">Messege</label>
      <textarea class="form-control" id="message" rows="3" required></textarea>
    </div>
    <a class="btn" @click="sendMail()">Enviar</a>
  </div>







</template>

<script>

import emailjs from '@emailjs/browser';
export default {
  name: 'ContactUs',
  methods: {

    sendMail() {
      (function () {
        emailjs.init('c_dO9xnSkiuIGG9OL');
      })();


      var params = {

        from_name: document.getElementById("from_name").value,
        email_id: document.getElementById("email_id").value,
        message: document.getElementById("message").value,
      };

      var ServiceID = "service_wwns16l";
      var templateID = "template_zv2c13a";

      emailjs.send(ServiceID, templateID, params)
      .then(
          () => {
            alert('SUCCESS!');
          },
          (error) => {
            alert('FAILED...', error.text);
          },
        );
    },




  }

}






</script>




<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.mycontainer {
  display: flex;
  flex-direction: column;

  padding: 6% 15%;
}

.title  {
  color: #000000;
  font-weight: bold;
  text-align: center;
  transition: color 0.3s ease;
  padding: 6% 0% 0% 0%;
}
</style>
