<template>
  <div class="show-case">
    <div class="show-case__presentation">
      <h1 class="show-case__presentation-title">
        Prazer,
      </h1>
      <h1 class="show-case__presentation-title">
        Eu sou o Gabriel!
      </h1>
      <p class="show-case__presentation-occupation">Desenvolvedor Front-end</p>
      <button class="show-case__presentation-button">
        <a class="show-case__presentation-button-link" href="https://mywhats.net/brune" target="_blank">
          Vamos conversar?!
        </a>
      </button>
    </div>
    <div class="show-case__logo">
      <img class="header-container_logo-img" alt="Nome logo" src="../assets/web-developer.svg">
    </div>
  </div>
</template>

<script>
export default {
  name: 'ShowCase',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .show-case{    
    background-color: #9584ab30;
    display: flex;
    justify-content: space-around;
    padding-top: 70px;
    padding-bottom: 100px;
    font-family: 'Ubuntu', sans-serif;
    border-bottom: 1px solid #5a6570;
  }
  .show-case__presentation-button-link{
    text-decoration: none;
    color: white;
  }
  .show-case__presentation-title {
    margin: 0px;
  }
  h1{
    font-size: 48px;
    font-weight: 700;
    line-height: 56px;
    color: #4e4039;
  }
  .show-case__presentation-occupation {
    color: #5a6570;
    margin-bottom: 20px;
    font-size: 26px;
  }
  .show-case__presentation-button {
    border: 0;
    font-weight: 500;
    font-size: 16px;
    letter-spacing: 1px;
    display: inline-block;
    padding: 14px 33px;
    border-radius: 3px;
    transition: 0.5s;
    margin: 10px;
    color: #fff;
    background: #6b4798;
  }
  .show-case__presentation-button:hover {
    background: #6b4798b8;
    transform: scale(1.2);
  }
</style>
