<template>
       <section id="about" class="about reveal">
        <div class="container about_container">
          <div class="about_content reveal">
            <div
              class="about_content-img"
            >
              <img
                src="../assets/webDeveloper.gif"
                class="img-fluid"
                alt=""
                data-aos="zoom-in"
              />
            </div>
            <div class="about_content-phrase">
              <h3 data-aos="fade-up">Sobre mim</h3>
              <div class="about_content-phrase-typography" >
                <p data-aos="fade-up" data-aos-delay="90">
                  Atualmente estou atuando como Desenvolvedor front-end React JS/Next JS.
                </p>
                <p data-aos="fade-up" data-aos-delay="90">
                  Cursando Ciência da Computação na Anhembi Morumbi, formado
                  em Desenvolvimento de Sistemas pela Etec de Embu.
                </p>

                <p data-aos="fade-up" data-aos-delay="90">
                  Em meu dia-a-dia utilizo estas tecnologias
                </p>

                <p data-aos="fade-up" data-aos-delay="90">
                  <strong
                    >React, Next, SASS, Styled-Components, JavaScript, Cypress, Hotjar
                    Google Analytics, Redux, Sagas, Context api, Git e Figma.
                  </strong>
                </p>

                <p data-aos="fade-up" data-aos-delay="10">
                  <a
                    href="https://drive.google.com/file/d/19E0j-auJzk7HD1xvrK_0rGLUQ1R_kjFu/view"
                    class="btn-get-cv"
                    target="_blank"
                  >
                    Confira meu CV
                  </a>
                </p>
              </div>
            </div>
          </div>
        </div>
      </section>
</template>

<script>
  export default {
    name: 'AboutSection',
  }
  window.addEventListener('scroll', reveal);

  function reveal() {
    let reveals = document.querySelectorAll('.reveal');
    console.log(reveals)
    for(var i = 0; reveals.length; i++){
      let windowheight = window.innerHeight;
      let revealTop = reveals[i].getBoundingClientRect().top
      let revealPoint = 150;
      if(revealTop < windowheight - revealPoint){
        reveals[i].classList.add('active');
      }else{
        reveals[i].classList.remove('active');

      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  #about .btn-get-cv {
    font-family: 'Ubuntu', sans-serif;
    font-weight: 500;
    font-size: 16px;
    letter-spacing: 1px;
    display: inline-block;
    padding: 8px 28px;
    border-radius: 3px;
    transition: 0.5s;
    color: #fff;
    margin-top:10px;
    background: #6b4798;
    text-decoration: none;
  }
  #about .btn-get-cv:hover {
    background: #6b4798b8;
    transform: scale(1.2);
  }
  .about h3 {
    font-weight: 700;
    font-size: 34px;
    color: #4e4039;
  }

  .about p {
    font-size: 17px;
    color: #5a6570;
  }
  
  .about_content {
    margin-top: 70px;
    display: flex;
    justify-content: space-around;
    margin-bottom: 50px;
    gap: 140px;
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

  @media (max-width: 991px) {
    .about .about-img img {
      max-width: 70%;
    }
  }

  @media (max-width: 767px) {
    .about .about-img img {
      max-width: 90%;
    }
  }

</style>
