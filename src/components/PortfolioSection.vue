<template>
      <section id="portfolio" class="portfolio">
        <div class="container">
          <div class="section-title reveal" data-aos="fade-up">
            <h2>Projetos Pessoais</h2>
            <p>Confira meus projetos</p>
          </div>
          <div
            class="portfolio-container"
            data-aos="fade-up"
            data-aos-delay="200"
          >
            <div class="col-lg-4 col-md-6 portfolio-item filter-react reveal">
              <div class="portfolio-wrap">
                <img
                  src="../assets/screen-alura.png"
                  class="img-fluid"
                  alt="Alura Quiz - Git Hub"
                />
                <div class="portfolio-links">
                  <a
                    href="https://github.com/Gabriel52/imersao_alura"
                    class="venobox"
                    title="Alura Quiz - Git Hub"
                    ><i class="icofont-plus-circle"></i
                  ></a>
                  <a
                    href="https://imersao-alura-pi.vercel.app/"
                    title="Alura Quiz - Hospedagem"
                    target="_blank"
                    ><i class="fab fa-github"></i
                  ></a>
                </div>
                <div class="portfolio-info">
                  <h4>Alura Quiz</h4>
                  <p>Next JS</p>
                </div>
              </div>
            </div>
            <div class="col-lg-4 col-md-6 portfolio-item filter-react reveal">
              <div class="portfolio-wrap">
                <img
                  src="../assets/screen-relogio.png"
                  class="img-fluid"
                  alt=""
                />
                <div class="portfolio-links">
                  <a
                    href="https://github.com/Gabriel52/Projetos_JS/tree/master/Relogio"
                    title="Hora do dia"
                    target="_blank"
                    ><i class="fab fa-github"></i
                  ></a>
                </div>
                <div class="portfolio-info">
                  <h4>Hora do dia</h4>
                  <p>Javascript</p>
                </div>
              </div>
            </div>

            <div class="col-lg-4 col-md-6 portfolio-item filter-html reveal">
              <div class="portfolio-wrap">
                <img
                  src="../assets/screen-be-the-hero.png"
                  class="img-fluid"
                  alt=""
                />
                <div class="portfolio-links">
                  <a
                    href="https://github.com/Gabriel52/Be-The-Hero"
                    data-gall="portfolioGallery"
                    class="venobox"
                    title="Be the hero"
                    ><i class="icofont-plus-circle"></i
                  ></a>
                </div>
                <div class="portfolio-info">
                  <h4>Be The Hero</h4>
                  <p>React JS</p>
                </div>
              </div>
            </div>

            <div class="col-lg-4 col-md-6 portfolio-item filter-html reveal">
              <div class="portfolio-wrap">
                <img
                  src="../assets/screen-proffy.png"
                  class="img-fluid"
                  alt=""
                />
                <div class="portfolio-links">
                  <a
                    href="https://github.com/Gabriel52/Proffy"
                    data-gall="portfolioGallery"
                    class="venobox"
                    title="Proffy - Git Hub"
                    ><i class="icofont-plus-circle"></i
                  ></a>
                  <a
                    href="https://stupefied-turing-6a35f2.netlify.app/"
                    title="Proffy - Hospedagem"
                    target="_blank"
                    ><i class="fab fa-github"></i
                  ></a>
                </div>
                <div class="portfolio-info">
                  <h4>Proffy</h4>
                  <p>React JS</p>
                </div>
              </div>
            </div>

            <div class="col-lg-4 col-md-6 portfolio-item filter-next reveal">
              <div class="portfolio-wrap">
                <img
                  src="../assets/screen-ecoleta.png"
                  class="img-fluid"
                  alt=""
                />
                <div class="portfolio-links">
                </div>
                <div class="portfolio-info">
                  <h4>Ecoleta</h4>
                  <p>React JS</p>
                </div>
              </div>
            </div>

          </div>
        </div>
      </section>
</template>

<script>
  export default {
    name: 'PortfolioSection',
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
  .portfolio .portfolio-item {
    margin-bottom: 30px;
  }

  .portfolio #portfolio-flters {
    padding: 0;
    margin: 0 0 35px 0;
    list-style: none;
    text-align: center;
  }
  .section-title {
    font-weight: 700;
    font-size: 24px;
    color: #4e4039;
    text-align: center;
  }
  .portfolio #portfolio-flters li {
    cursor: pointer;
    margin: 0 15px 15px 0;
    display: inline-block;
    padding: 5px;
    font-size: 16px;
    font-weight: 600;
    line-height: 20px;
    color: #212529;
    margin-bottom: 5px;
    transition: all 0.3s ease-in-out;
  }

  .portfolio #portfolio-flters li:hover,
  .portfolio #portfolio-flters li.filter-active {
    color: #6b4798;
  }

  .portfolio #portfolio-flters li:last-child {
    margin-right: 0;
  }

  .portfolio .portfolio-wrap {
    transition: 0.3s;
    position: relative;
    overflow: hidden;
    border-radius: 8px;
    z-index: 1;
  }

  .portfolio .portfolio-wrap::before {
    content: "";
    background: rgba(112, 96, 122, 0.6);
    position: absolute;
    left: 100%;
    right: 0;
    top: 0;
    bottom: 0;
    transition: all ease-in-out 0.3s;
    z-index: 2;
  }

  .portfolio .portfolio-wrap img {
    transition: 0.3s;
    position: relative;
    z-index: 1;
    width: 450px;
  }

  .portfolio .portfolio-wrap .portfolio-links {
    opacity: 0;
    left: 0;
    right: 0;
    top: calc(50% - 32px);
    text-align: center;
    z-index: 3;
    position: absolute;
    transition: all ease-in-out 0.3s;
  }

  .portfolio .portfolio-wrap .portfolio-links a {
    color: #6b4798;
    margin: 0 4px;
    font-size: 18px;
    line-height: 1;
    background-color: #fff;
    padding-top: 6px;
    padding-right: 1px;
    border-radius: 50px;
    text-align: center;
    width: 32px;
    height: 32px;
    display: inline-block;
    transition: 0.3s;
  }

  .portfolio-container {
    display: grid;
    grid-template-columns: repeat(2, 450px);
    justify-content: center;
    gap: 50px
  }

  .portfolio .portfolio-wrap .portfolio-links a i {
    line-height: 1;
  }

  .portfolio .portfolio-wrap .portfolio-links a:hover {
    background: #6b4798;
    color: #fff;
  }

  .portfolio .portfolio-wrap .portfolio-info {
    opacity: 0;
    position: absolute;
    bottom: -20px;
    left: 0;
    right: 0;
    text-align: center;
    z-index: 3;
    transition: all ease-in-out 0.3s;
  }

  .portfolio .portfolio-wrap .portfolio-info h4 {
    font-size: 20px;
    color: #fff;
    font-weight: 600;
  }

  .portfolio .portfolio-wrap .portfolio-info p {
    color: #ffffff;
    font-size: 14px;
    text-transform: uppercase;
  }

  .portfolio .portfolio-wrap:hover::before {
    left: 0;
  }

  .portfolio .portfolio-wrap:hover .portfolio-links {
    opacity: 1;
    top: calc(50% - 16px);
  }

  .portfolio .portfolio-wrap:hover .portfolio-info {
    opacity: 1;
    bottom: 0;
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

</style>
