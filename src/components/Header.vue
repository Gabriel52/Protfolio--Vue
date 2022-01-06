<template>
  <header class="header-container">
    <div class="header-container_section-logo">
        <img class="header-container_logo-img" alt="Nome logo" src="../assets/programador.png">
        <h1 class="header-container_logo">Gabriel Brune</h1>
    </div>
    <ul class="header-container_section-page">
        <li class="header-container_section-item">
            <a class="header-container__link" href="/#" >
                Home
            </a>
        </li>
        <li class="header-container_section-item">
            <a class="header-container__link" href="/#about" >
                Sobre mim
            </a>
        </li>
        <li class="header-container_section-item">
            <a class="header-container__link" href="/#services" >
                Tecnologias
            </a>
        </li>
        <li class="header-container_section-item">
            <a class="header-container__link" href="#portfolio" >
                Projetos
            </a>
        </li>
        <li class="header-container_section-item">
            <a class="header-container__link" href="#" >
                Contatos
            </a>
        </li>
        <li class="header-container_section-item--button">
            <a class="header-container__link--button" href="https://drive.google.com/file/d/19E0j-auJzk7HD1xvrK_0rGLUQ1R_kjFu/view" >
                Currículo
            </a>
        </li>
    </ul>
  </header>
</template>

<script>
export default {
  name: 'Header',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    .header-container{
        display: flex;
        justify-content: space-around;
        align-items: center;
        box-shadow: 9px 7px 5px rgb(161 152 152 / 77%);
        padding-top: 10px;
        padding-bottom: 10px;
    }
    .header-container_section-page{
        display: flex;
        list-style-type: none;
        gap: 30px;
        margin: 0px;
    }
    .header-container__link {
        font-family: 'Open Sans', sans-serif;
        text-decoration: none;
        font-weight: normal;
        font-size: 16px;
        line-height: 110%;
        color: #5A6570;
        transition: all 400ms ease;
    }
    .header-container_section-item{
        margin-top: 5px;
    }
    .header-container__link:hover{
        color: #6B4798;
        font-weight:700;
    }
    .header-container_logo {
        font-family: 'Ubuntu', sans-serif;
        margin-top: 5px;
        margin-bottom: 12px;
    }
    .header-container_section-logo{
        display: grid;
        grid-template-columns: 3rem 13rem;
        align-items: center;
    }
    .header-container__link--button {
        background: #6B4798;
        border-radius: 16px;
        box-sizing: border-box;

        font-size: 16px;
        font-family: 'Open Sans', sans-serif;
        color: #fff;
        
        text-decoration: none;
        padding: 4px 20px;
        display: block;
    }
</style>
