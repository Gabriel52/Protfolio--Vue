<template>
    <section id="services" class="services">
        <div class="container service">
          <div class="section-title reveal" data-aos="fade-up">
            <h2>Tecnologias</h2>
            <p>Confira as tecnologias que mais utilizo</p>
          </div>

          <div class="service_content-card">
            <div
              class="align-items-stretch reveal"
            >
              <div class="icon-box">
                <a target="_blank" href="https://nextjs.org/">
                  <div class="icon"><i class="fab fa-html5"></i></div>
                  <h4 class="title"><a>Next JS</a></h4>
                  <p class="description">
                    o Next. js é um framework de código aberto, criado com React e permite o desenvolvimento de 
                    aplicações tanto front-end quanto back-end.
                  </p>
                </a>
              </div>
            </div>

            <div
              class="align-items-stretch reveal"
            >
              <div class="icon-box">
                <a target="_blank" href="https://styled-components.com/">
                  <div class="icon"><i class="fab fa-css3-alt"></i></div>
                  <h4 class="title"><a>Styled Components</a></h4>
                  <p class="description">
                    Trata-se de uma biblioteca (lib) que nos permite escrever
                    códigos CSS dentro do JavaScript
                  </p>
                </a>
              </div>
            </div>

            <div
              class="align-items-stretch reveal"
              data-aos="zoom-in"
              data-aos-delay="200"
            >
              <div class="icon-box">
                <a target="_blank" href="https://sass-lang.com/">
                  <div class="icon"><i class="fab fa-sass"></i></div>
                  <h4 class="title"><a>SASS</a></h4>
                  <p class="description">
                    Com ele podemos dar "super poderes" ao nosso CSS
                  </p>
                </a>
              </div>
            </div>

            <div
              class="align-items-stretch reveal"
              data-aos="zoom-in"
              data-aos-delay="100"
            >
              <div class="icon-box">
                <a target="_blank" href="https://devdocs.io/javascript/">
                  <div class="icon"><i class="fab fa-js"></i></div>
                  <h4 class="title"><a>JavaScript</a></h4>
                  <p class="description">
                    Uma das linguagens de programação mais utilizadas hoje em dia
                  </p>
                </a>
              </div>
            </div>

            <div
              class="align-items-stretch reveal"
              data-aos="zoom-in"
              data-aos-delay="300"
            >
              <div class="icon-box">
                <a target="_blank" href="https://pt-br.reactjs.org/docs/getting-started.html">
                  <div class="icon"><i class="fab fa-react"></i></div>
                  <h4 class="title"><a>React JS</a></h4>
                  <p class="description">
                    Biblioteca usada para construir interface de usuário (UI)
                  </p>
                </a>
              </div>
            </div>

            <div
              class="align-items-stretch reveal"
            >
              <div class="icon-box">
                <a target="_blank" href="https://reactnative.dev/docs/getting-started">
                  <div class="icon"><i class="fab fa-react"></i></div>
                  <h4 class="title"><a>React Native</a></h4>
                  <p class="description">
                    Framework para desenvolvimento de aplicativos para Android e
                    iOS de forma nativa
                  </p>
                </a>
              </div>
            </div>

            <div
              class="align-items-stretch reveal"
            >
              <div class="icon-box">
                <a target="_blank" href="https://git-scm.com/docs/git/pt_BR">
                  <div class="icon"><i class="fab fa-git-alt"></i></div>
                  <h4 class="title"><a>Git</a></h4>
                  <p class="description">
                    É um sistema de controle de versões distribuído
                  </p>
                </a>
              </div>
            </div>

            <div
              class="align-items-stretch reveal"
            >
              <div class="icon-box">
                <a href="https://nodejs.org/en/">
                  <h4 class="title"><a>Node JS</a></h4>
                  <p class="description">
                    Com o Node. js é possível criar aplicações Javascript para 
                    rodar como uma aplicação standalone em uma máquina
                  </p>
                </a>
                <div class="icon"><i class="fab fa-figma"></i></div>
              </div>
            </div>
          </div>
        </div>
    </section>
</template>

<script>
  export default {
    name: 'ServicesSection',
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
  .services {
    padding-top: 40px;
    padding-bottom: 80px;
    background-color: #9584ab30;
  }
  a {
    text-decoration: none;
  }
 .services .icon-box {
    padding: 30px;
    position: relative;
    overflow: hidden;
    background: #fff;
    box-shadow: 0 10px 29px 0 rgba(68, 88, 144, 0.1);
    transition: all 0.3s ease-in-out;
    border-radius: 15px;
    text-align: center;
    border-bottom: 3px solid #fff;
    min-height: 200px;
  }
   .section-title{
      font-weight: 700;
      font-size: 24px;
      color: #4e4039;
      text-align: center;
   }
  .service_content-card {
    display: grid;
    grid-template-columns: repeat(3, 300px);
    gap: 50px;
    justify-content: center;
    margin-top: 40px;
  }

  .services .icon-box:hover {
    transform: translateY(-5px);
    border-color: #6b4798;
    transform: scale(1.1);
  }

  .services .icon i {
    font-size: 48px;
    line-height: 1;
    margin-bottom: 15px;
    color: #6b4798;
  }

  .services .title {
    font-weight: 700;
    margin-bottom: 15px;
    font-size: 18px;
  }

  .services .title a {
    color: #111;
  }

  .services .description {
    font-size: 15px;
    line-height: 28px;
    margin-bottom: 0;
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

  @media (min-width: 1700px) {
    .service_content-card {
      grid-template-columns: repeat(4, 300px);
    }
  }
</style>
