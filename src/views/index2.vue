<script>

import Navbar from "@/components/navbar";
import Services from "@/components/services";
/* import Features from "@/components/features"; */
//import Pricing from "@/components/pricing";
import Team from "@/components/team";
// import Blog from "@/components/blog";
import Contact from "@/components/contact";
import Footer from "@/components/footer";

export default {
  components: {
    Navbar,
    Services,
   /*  Features, */
   // Pricing,
    Team,
  //  Blog,
    Contact,
    Footer,
  },
  data() {
    return {};
  },
};
</script>

<template>
  <div>
    <Navbar :navcolor="'light'" />
    <div v-scroll-spy>
      <!-- Hero Start -->

      <!-- Hero Start -->
      <section
        class="hero-2 position-relative overflow-hidden"
        :style="{
          'background-image':
            'url(' + require('@/assets/images/hero-2-bg.png') + ')',
        }"  id="home">
        <div class="container">
          <div class="row align-items-center">
            <div class="col-lg-5">
           <!--    <span class="badge badge-soft-primary mb-4">DDarkCoder</span> -->
              <h1 class="font-weight-semibold mb-4 hero-2-title">
                
                Engenharia e soluções tecnológicas
              </h1>
              <p class="mb-5 text-muted">
                Somos uma empresa de desevolvimento de software e prestação de serviços.
              </p>
            </div>
            <div class="col-lg-6 col-sm-10 mx-auto ms-lg-auto me-lg-0">
              <div class="mt-lg-0 mt-4">
                <img
                  src="@/assets/images/hero-2-img.png"
                  alt=""
                  class="img-xl-responsive"
                />
              </div>
            </div>
          </div>
        </div>
      </section>
      <!-- Hero End -->
      <Services />
    <!--   <Features /> -->
     <!--  <Pricing /> -->
      <Team />
     <!--  <Blog /> -->
      <Contact />
      <Footer />
    </div>
  </div>
</template>