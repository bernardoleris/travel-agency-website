<template>
    <!-- Footer -->
    <MDBFooter :text="['center', 'lg-start', 'muted']">
      <!-- Section: Social media -->
      <section class="" style="margin-top: 50px;">
        <!-- Left -->
        <div class="me-5-d-none d-lg-block" style="color: #383961; text-align: center; font-size: 36px; margin-top: 40px;">
          <h1><span>Quer nos conhecer melhor? Contate-nos!</span></h1>
        </div>

      </section>
      <section class="">
        <MDBContainer class="text-center text-md-start mt-5">
          <MDBRow class="mt-3">
            <MDBCol md="2" lg="2" xl="2" class="mx-auto mb-4">
              <h6 style="color: #383961; margin-top: 15px; font-size: 26px;">Nossas redes sociais:</h6>
              <p>
                <a href="https://www.facebook.com/compjunior/?locale=pt_BR" target="_blank" class="text-reset" style="font-size: 18px; color: black;">Facebook</a>
              </p>
              <p>
                <a href="https://www.instagram.com/compjunior/" target="_blank" class="text-reset" style="font-size: 18px;">Instagram</a>
              </p>
            </MDBCol>
            <MDBCol md="4" lg="3" xl="3" class="mx-auto mb-md-0 mb-4">
              <!-- Links -->
              <h6 class="" style="font-size: 26px; color: #383961;">Contato:</h6>
              <p style="font-size: 18px; color: black;"><b-icon icon="geo" font-scale="1.0"></b-icon>
                <i class="fas fa-home me-3"></i> Rua Maurício de Souza, 330, Vila Flores, Lavras-MG
              </p>
              <p style="font-size: 18px; color: black;"><b-icon icon="envelope" font-scale="1.0"></b-icon>
                <i class="fas fa-envelope me-3"></i>
                travel.comunicacao@gmail.com
              </p>
              <p style="font-size: 18px; color: black;"><b-icon icon="phone" font-scale="1.0"></b-icon>
                <MDBIcon icon="phone" class="me-3" /> + 35 3829 1923
              </p>
              <p style="font-size: 18px; color: black;"><b-icon icon="phone" font-scale="1.0"></b-icon>
                <MDBIcon icon="print" class="me-3" /> + 35 99833 9121
              </p>
            </MDBCol>
          </MDBRow>
        </MDBContainer>
      </section>
      <div class="text-center p-4" style="background-color: #383961; opacity: 90%; color: white;">
        © 2023 Copyright:
        <a class="text-reset fw-bold">Travel Turismo</a>
      </div>
    </MDBFooter>
  </template>

