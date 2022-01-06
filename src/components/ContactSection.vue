<template>
  <section id="contact" class="contact">
    <div class="container">
      <div class="section-title reveal" data-aos="fade-up">
        <h2>Contatos</h2>
        <p>Entre em contato para começarmos</p>
      </div>

      <div class="contact__content">
        <div
          class="col-lg-5 d-flex align-items-stretch justify-content-center"
          data-aos="fade-up"
          data-aos-delay="100"
        >
          <div class="info reveal">
            <div class="address">
              <i class="icofont-google-map"></i>
              <h4>Localização:</h4>
              <p>Embu das Artes - SP, Brasil</p>
            </div>

            <div class="email">
              <i class="icofont-envelope"></i>
              <h4>Email:</h4>
              <p>gabrielbrune52@gmail.com</p>
            </div>

            <div class="phone">
              <a href="#" target="_blank"
                ><i class="icofont-whatsapp"></i
              ></a>
              <h4>Telefone:</h4>
              <p>(11) 96018-8549</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'ContactSection',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .contact {
    padding-top: 40px;
    padding-bottom: 80px;
    background-color: #d5cae330;
  }

  .section-title {
    font-weight: 700;
    font-size: 24px;
    color: #4e4039;
    text-align: center;
  }
  .contact .info {
    border-top: 3px solid #6b4798;
    border-bottom: 3px solid #6b4798;
    padding: 30px;
    background: #fff;
    width: 100%;
    box-shadow: 0 0 24px 0 rgba(0, 0, 0, 0.12);
    margin-left: auto;
    margin-right: auto;
    width: 40rem;
  }

  .contact .info i {
    font-size: 20px;
    color: #6b4798;
    float: left;
    width: 44px;
    height: 44px;
    background: #d5cae330;
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 50px;
    transition: all 0.3s ease-in-out;
  }

  .contact .info h4 {
    padding: 0 0 0 60px;
    font-size: 22px;
    font-weight: 600;
    margin-bottom: 5px;
    color: #6b4798;
  }

  .contact .info p {
    padding: 0 0 10px 60px;
    margin-bottom: 20px;
    font-size: 14px;
    color: #5a6570;
  }

  .contact .info .email p {
    padding-top: 5px;
  }

  .contact .info .social-links {
    padding-left: 60px;
  }

  .contact .info .social-links a {
    font-size: 18px;
    display: inline-block;
    background: #333;
    color: #fff;
    line-height: 1;
    padding: 8px 0;
    border-radius: 50%;
    text-align: center;
    width: 36px;
    height: 36px;
    transition: 0.3s;
    margin-right: 10px;
  }

  .contact .info i:hover {
    background: #6b4798;
    color: #fff;
  }

  .reveal{
    position: relative;
    transform: translateY(150px);
    opacity: 0;
    transition: all 2s ease;
  }

  .reveal.active{
    transform: translateY(0px);
    opacity: 1;
  }


  @-webkit-keyframes animate-loading {
    0% {
      transform: rotate(0deg);
    }
    100% {
      transform: rotate(360deg);
    }
  }

  @keyframes animate-loading {
    0% {
      transform: rotate(0deg);
    }
    100% {
      transform: rotate(360deg);
    }
  }
</style>
