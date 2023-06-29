<template>
  <div>
    <b-navbar toggleable="lg">
      <b-navbar-brand href="#">
        <div class="logo-container">
          <b-button v-b-toggle.sidebar-menu>
            <b-icon icon="list-ul" font-scale="1"></b-icon>
          </b-button>
          <img src="../images/travel-2.png" alt="Logo" height="60" class="logo">
        </div>
      </b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
          <b-nav-item class = "escritas_navBar" href="#quem_somos">Quem somos?</b-nav-item>
          <b-nav-item class = "escritas_navBar" href="#projetos">Projetos</b-nav-item>
          <b-nav-item class = "escritas_navBar" href="#footer">Contato</b-nav-item>
        </b-navbar-nav>

        <b-navbar-nav class="ml-auto">
          <b-nav-form>
            <b-form-input size="sm" class="mr-sm-2" placeholder="Digite aqui seu destino..."></b-form-input>
            <b-button size="sm" class="my-2 my-sm-0" type="submit">Busca</b-button>
          </b-nav-form>
          <b-nav-item-dropdown right>
            <!-- Using 'button-content' slot -->
            <template #button-content>
              <em>Entrar</em>
            </template>
            <b-dropdown-item href="#">Login</b-dropdown-item>
            <b-dropdown-item href="#">Minhas reservas</b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
export default {
  name: "Navbar",
};
</script>

<style>

button.btn.btn-secondary.collapsed{
  background-color: #383961;
  border: none;
}
div.logo-container{
  background-color: rgb(255, 255, 255);
}

button.btn.my-2.my-sm-0.btn-secondary.btn-sm{
  background-color: #383961;
}
.logo{
  margin-left: 20px;
}

.escritas_navBar{
  color: rgb(255, 255, 255) !important;;
}

div#nav-collapse.navbar-collapse.collapse a.nav-link{
  color: #383961;
  font-size: 20px;
}
</style>
