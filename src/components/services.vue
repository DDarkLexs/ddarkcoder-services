<script>
import { LayersIcon, ServerIcon ,LayoutIcon } from "vue-feather-icons";

export default {
  components: { LayersIcon, ServerIcon, LayoutIcon },
  data() {
    return {};
  },
};
</script>

<template>
  <!-- Services start -->
  <section class="section" id="services">
    <div class="container">
      <div class="row justify-content-center mb-5">
        <div class="col-lg-7 text-center">
          <h2 class="fw-bold">Nossos serviços</h2>
          <p class="text-muted">
            Criamos para sí website, sistema de software
            com maior responsabilidade, segunrança e facil
            de utilidade 
          </p>
        </div>
      </div>

      <div class="row">
        <div class="col-lg-4">
          <div class="service-box text-center px-4 py-5 position-relative mb-4">
            <div class="service-box-content p-4">
              <div class="icon-mono service-icon avatar-md mx-auto mb-4">
                <LayoutIcon />
              </div>
              <h4 class="mb-3 font-size-22">website e software desktop </h4>
              <p class="text-muted mb-0">
                Desenvolvemos para sí website dinâmico e software para 
                o computador
              </p>
            </div>
          </div>
        </div>
        <!-- end col -->

        <div class="col-lg-4">
          <div
            class="service-box text-center px-4 py-5 position-relative mb-4 active"
          >
            <div class="service-box-content p-4">
              <div class="icon-mono service-icon avatar-md mx-auto mb-4">
                <layers-icon class=""></layers-icon>
              </div>
              <h4 class="mb-3 font-size-22">Serviços de API</h4>
              <p class="text-muted mb-0">
                criamos serviços de endpoint para solicitação de dados via API
              </p>
            </div>
          </div>
        </div>
        <!-- end col -->

        <div class="col-lg-4">
          <div class="service-box text-center px-4 py-5 position-relative mb-4">
            <div class="service-box-content p-4">
              <div class="icon-mono service-icon avatar-md mx-auto mb-4">
                <server-icon class=""></server-icon>
              </div>
              <h4 class="mb-3 font-size-22">Banco de dados</h4>
              <p class="text-muted mb-0">
                Estruturamos banco de dados para si
              </p>
            </div>
          </div>
        </div>
        <!-- end col -->
      </div>
      <!-- end row -->
    </div>
    <!-- end container -->
  </section>
  <!-- Services end -->
</template>