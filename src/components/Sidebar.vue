<template>
  <div>
    <b-sidebar
      class="custom-sidebar"
      id="sidebar-menu"
      aria-labelledby="sidebar-no-header-title"
      no-header
      shadow
      bg-variant="dark"
      text-variant="light"
      backdrop
    >
      <template #default="{ hide }">
        <div class="p-3">
          <div class="d-flex align-items-center flex-column">
            <img
              src="../images/travel-website-favicon-white.png"
              alt="Logo"
              class="mb-3 mt-3"
              style="width: 5rem; height: 5rem"
            />
            <h4 id="sidebar-no-header-title">Feito para você!</h4>
          
          </div>

          <nav class="mb-3">
            <b-nav vertical>
              <b-nav-item active @click="hide"
                ><b-icon icon="arrow-up-square" font-scale="1.5"></b-icon>
                Destinos mais procurados</b-nav-item
              >
              <b-nav-item href="#link-1" @click="hide"
                ><b-icon icon="cash" font-scale="1.5"></b-icon>
                Ofertas</b-nav-item
              >
              <b-nav-item href="#link-2" @click="hide"
                ><b-icon icon="arrow-left-right" font-scale="1.5"></b-icon>
                Monte sua viagem</b-nav-item
              >
              <b-nav-item href="#link-2" @click="hide"
                ><b-icon icon="person" font-scale="1.5"></b-icon>
                Avaliações</b-nav-item
              >
            </b-nav>
          </nav>
          <b-button variant="primary" block @click="hide">Fechar</b-button>
          <p class="text-center">Desenvolvido por Bernardo Leris</p>
        </div>
      </template>
    </b-sidebar>
  </div>
</template>

<script>
export default {
  name: "Sidebar",
};
</script>

<style scoped>
.nav-item > .nav-link {
  color: rgb(255, 255, 255);
}
.nav-item > .nav-link:hover {
  color: rgb(219, 219, 219);
}
.divider-menu {
  border: 1px solid rgb(255, 255, 255);
  width: 100%;
}
.text-center {
  position: absolute;
  bottom: 0;
  left: 0;
  padding: 1rem;
  width: 100%;
  font-size: 13px;
  text-align: center;
  color: white;
  font-weight: bold;
  background-color: #383961;
}
.b-sidebar-body{
  color: rgb(224, 224, 224);
}

</style>

<style>
div#sidebar-menu.b-sidebar.shadow.bg-dark.text-light{
  background-color: #383961 !important;
}

button.btn.btn-primary.btn-block{
  border-color: white;
  margin-top: 470px !important;
  background-color: rgb(255, 255, 255);
  color:#383961
}

</style>
