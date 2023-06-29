<template>
  <div class="home">
    <Navbar />
    <Sidebar />
    <Carousel />
    <router-view />

    <a id="quem_somos">
      <div class="quem-somos-container">
        <h1>Quem somos?</h1>
        <p class="descricao">Somos uma empresa de turismo apaixonada por proporcionar jornadas inesquecíveis aos nossos clientes. 
          Com uma abordagem personalizada e atenção aos detalhes, criamos itinerários sob medida que se adaptam às preferências 
          individuais de cada viajante. Nosso diferencial está em oferecer viagens autênticas, parcerias com fornecedores 
          confiáveis e um compromisso com o turismo responsável. Junte-se a nós na <span>Travel</span> e deixe-nos transformar 
          seus sonhos de viagem em realidade!</p>
        <div class="quem-somos-imagem-container">
          <img src="../images/travel-website-favicon-color.png" alt="Imagem da Empresa" />
        </div>
      </div>
    </a>
    
    <hr class="section-divider">

    <a id="projetos">
      <div class="projetos-container">
        <h1>Projetos</h1>
        <p class = "descricao">A <span>Travel</span> faz parte um programa especial de viagens acessíveis em parceria com empresas de turismo e instituições de todo o mundo, oferecendo experiências de viagem de qualidade a 
          preços justos para pessoas com dificuldades financeiras e com desejo de aprender e evoluir como indivíduo. Isso incluirá tarifas negociadas e pacotes com descontos 
          significativos.</p>
        <p>Promoção ações solidárias em destinos turísticos, em conjunto com organizações locais. O que envolve 
          arrecadação de fundos, apoio a projetos comunitários, preservação ambiental e incentivo aos clientes a participarem 
          de atividades solidárias durante as viagens. Contribuindo para o desenvolvimento sustentável e 
          a melhoria das condições das comunidades visitadas!</p>
      </div>
    </a>

    <hr class="section-divider">

    <Footer id="footer" />
  </div>
</template>
<script>
import Navbar from "../components/Navbar";
import Sidebar from "../components/Sidebar";
import Carousel from "../components/Carousel";
import Footer from "../components/Footer";

export default {
  name: "Home",
  components: {
    Navbar,
    Sidebar,
    Carousel,
    Footer,
  },
};
</script>

<style lang="scss">
  html{
    scroll-behavior: smooth;
  }
  body{
    height: 100vh;
    width: 100vw;
  }
  #app{
    height: 100%;
    width: 100%;
    overflow-x: none;
  }
  .quem-somos-container {
    text-align: center;
    margin-top: 80px;
  }
  .quem-somos-container h1 {
    font-size: 60px;
    color: #383961;
  }
  .quem-somos-container p {
    font-size: 25px;
    color: #666;
    margin-top: 40px;
    margin-left: 250px;
    margin-right: 250px;
  }
  .projetos-container{
    margin-top: 60px;
    text-align: center;
  }
  .projetos-container h1{
    font-size: 60px;
    color: #383961;
  }
  .projetos-container p{
    font-size: 25px;
    color: #666;
    margin-top: 40px;
    margin-left: 250px;
    margin-right: 250px
  }
  .descricao span {
    color: #383961; 
    font-weight: bold;
    
}
.projetos-container p::before {
  content: "•";
  display:inline-block;
  margin-right: 5px;
  color: #383961;
  font-size: 35px;
}

.section-divider {
  border-top: 1px dotted #383961;
  opacity: 30%;
  margin: 40px 0;
}

</style>

</script>
