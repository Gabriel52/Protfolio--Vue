<template>
  <footer id="footer">
      <section id="social" class="social">
        <div class="footer-top">
          <div class="container">
            <div
              class="row justify-content-center"
              data-aos="fade-up"
              data-aos-delay="400"
            >
              <div class="footer-links">
                <p>Onde me encontrar:</p>
                <div class="social-links">
                  <a target="_blank" href="https://www.linkedin.com/in/gabriel-brune-dos-santos-032b9717a/">
                    <img src="../assets/linkedin.svg" alt="">
                  </a>
                  <a target="_blank" href="https://api.whatsapp.com/send?phone=5511960188549&text=Ol%C3%A1%2C%20gostaria%20de%20saber%20mais%20sobre%20voc%C3%AA.">
                    <img src="../assets/whatsapp.svg" alt="">
                  </a>
                  <a target="_blank" href="https://github.com/Gabriel52">
                    <img src="../assets/gitHub.svg" alt="">
                  </a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>

      <div class="container py-4">
        <div class="copyright">
          &copy; Copyright <strong><span>Gabriel Brune</span></strong> 2022
        </div>
      </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  #footer {
    padding: 0 0 30px 0;
    color: #212529;
    font-size: 14px;
    background: #d5cae330;
  }

  #footer .footer-top {
    padding: 60px 0 30px 0;
    background: #fff;
  }

  #footer .footer-top p {
    font-size: 32px;
    font-weight: bold;
    color: #4e4039;
    position: relative;
    text-align: center;
  }

  #footer .footer-top .footer-links {
    margin-bottom: 30px;
    text-align: center;
  }

  .social-links {
    display:flex;
    justify-content: center; 
    gap: 36px;
  }

  #footer .copyright {
    text-align: center;
    font-family: 'Open Sans', sans-serif;
    font-weight: 700;
    font-size: 18px;
    line-height: 110%;
    color: #5A6570;
    padding: 20px;
  }

  @media (max-width: 575px) {
    #footer .copyright {
      float: none;
      -moz-text-align-last: center;
      text-align-last: center;
      padding: 3px 0;
    }
  }
</style>
