<script>
import { ArrowRightIcon } from "vue-feather-icons";

export default {
  components: { ArrowRightIcon },
  data() {
    return {};
  },
};
</script>

<template>
  <div>
    <!-- Features start -->
    <section class="section bg-light" id="features">
      <div class="container">
        <div class="row justify-content-center mb-5">
          <div class="col-lg-7 text-center">
            <h2 class="fw-bold">Nossos Recursos</h2>
            <p class="text-muted">
              Sed ut perspiciatis unde omnis iste natus error sit voluptatem
              accusantium doloremque laudantium totam rem ab illo inventore.
            </p>
          </div>
        </div>

        <div class="row align-items-center mb-5">
          <div class="col-md-5 order-2 order-md-1 mt-md-0 mt-5">
            <h2 class="mb-4">Solução Perfeita para micro empresa <!-- Perfect Solution For Small Businesses --></h2>
            <p class="text-muted mb-5">
              Sed ut perspiciatis unde omnis iste natus error sit voluptatem
              accusantium doloremque laudantium totam rem aperiam eaque ipsa
              quae ab illo inventore veritatis..
            </p>
          
          </div>
          <div class="col-md-6 ms-md-auto order-1 order-md-2">
            <div class="position-relative">
              <div class="ms-5 features-img">
                <img
                  src="@/assets/images/features-1.jpg"
                  alt=""
                  class="img-fluid d-block ms-auto rounded shadow"
                />
              </div>
              <img
                src="@/assets/images/dot-img.png"
                alt=""
                class="dot-img-left"
              />
            </div>
          </div>
        </div>
        <!-- end row -->
        <div class="row align-items-center section pb-0">
          <div class="col-md-6">
            <div class="position-relative mb-md-0 mb-5">
              <div class="me-5 features-img">
                <img
                  src="@/assets/images/features-2.jpg"
                  alt=""
                  class="img-fluid d-block ms-auto rounded shadow"
                />
              </div>
              <img
                src="@/assets/images/dot-img.png"
                alt=""
                class="dot-img-right"
              />
            </div>
          </div>
          <div class="col-md-5 ms-md-auto">
            <h2 class="mb-4">
              Build community & conversion with our suite of social tool
            </h2>
            <p class="text-muted mb-5">
              Sed ut perspiciatis unde omnis iste natus error sit voluptatem
              accusantium doloremque laudantium totam rem aperiam eaque ipsa
              quae ab illo inventore veritatis..
            </p>
            <a href="javascript: void(0);" class="btn btn-primary"
              >Find out more
              <arrow-right-icon class="icon-xs ms-2"></arrow-right-icon
            ></a>
          </div>
        </div>
        <!-- end row -->
      </div>
      <!-- end container -->
    </section>
    <!-- Features end -->

    <section class="section bg-gradient-primary">
      <div
        class="bg-overlay-img"
        :style="{
          'background-image':
            'url(' + require('@/assets/images/demos.png') + ')',
        }"
      ></div>
      <div class="container">
        <div class="row justify-content-center">
          <div class="col-lg-8">
            <div class="text-center">
              <h1 class="text-white mb-4">Build your dream website today</h1>
              <p class="text-white mb-5 font-size-16">
                Sed perspiciatis unde omnis iste natus error sit voluptatem
                accusantium doloremque laudantium totamrem aperiam eaque
                inventore veritatis quasi.
              </p>
              <a href="#" class="btn btn-lg btn-light">Ask for Demonstration</a>
            </div>
          </div>
          <!-- end col -->
        </div>
        <!-- end row -->
      </div>
      <!-- end container -->
    </section>
    <!-- Cta end -->
  </div>
</template>