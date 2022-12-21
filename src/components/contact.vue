<script>
import {
  MailIcon,
  PhoneIcon,
  FacebookIcon,
  TwitterIcon,
  InstagramIcon,
  MapPinIcon
} from "vue-feather-icons";

export default {
  components: { MailIcon, PhoneIcon, FacebookIcon, TwitterIcon, InstagramIcon,MapPinIcon },
  data() {
    return {
      contact:{
        tel:'+244 937 781 157',
        email:'antoniolexis2001@gmail.com',
      },


    };
  },
  methods:{
    enviarEmail(){
      alert('ok')

    }
  }

};
</script>

<template>
  <!-- Contact us start -->
  <section class="section" id="contact">
    <div class="container">
      <div class="row">
        <div class="col-lg-6">
          <h2 class="fw-bold mb-4">Entre em contacto</h2>
          <p class="text-muted mb-5">
            Envie nós o seu email o ligue para nós para mais informações
          </p>

          <div>
            <form method="post"
            
            @submit.prevent="enviarEmail"
            name="myForm" onsubmit="return validateForm()">
              <p id="error-msg"></p>
              <div id="simple-msg"></div>
              <div class="row">
                <div class="col-lg-6">
                  <div class="mb-4">
                    <label for="name" class="text-muted form-label">Nome</label>
                    <input
                      name="name"
                      id="name"
                      type="text"
                      class="form-control"
                      placeholder="informe o nome*"
                    />
                  </div>
                </div>
                <div class="col-lg-6">
                  <div class="mb-4">
                    <label for="email" class="text-muted form-label">
                      Email
                    </label>
                    <input
                      name="email"
                      id="email"
                      type="email"
                      class="form-control"
                      placeholder="informe email*"
                    />
                  </div>
                </div>
                <div class="col-md-12">
                  <div class="mb-4">
                    <label for="subject" class="text-muted form-label"
                      >Titulo</label>
                    <input
                      type="text"
                      class="form-control"
                      id="subject"
                      name="subject"
                      placeholder="informe o titulo.."
                    />
                  </div>

                  <div class="mb-4 pb-2">
                    <label for="comments" class="text-muted form-label"
                      >Mensagem</label
                    >
                    <textarea
                      name="comments"
                      id="comments"
                      rows="4"
                      class="form-control"
                      placeholder="informe a mensage..."
                    ></textarea>
                  </div>

                  <button
                    type="submit"
                    id="submit"
                    name="send"
                    class="btn btn-primary"
                  >
                    Enviar o email
                  </button>
                </div>
              </div>
            </form>
          </div>
        </div>
        <!-- end col -->

        <div class="col-lg-5 ms-lg-auto">
          <div class="mt-5 mt-lg-0">
            <img
              src="@/assets/images/contact.png"
              alt=""
              class="img-fluid d-block"
            />
            <p class="text-muted mt-5 mb-3">
              <mail-icon class="me-2 text-muted icon icon-xs"></mail-icon>
              {{ contact.email }}
            </p>
            <p class="text-muted mb-3">
              <phone-icon class="me-2 text-muted icon icon-xs"></phone-icon>
              {{ contact.tel }}
            </p>
            <p class="text-muted mb-3">
              <map-pin-icon
                class="me-2 text-muted icon icon-xs"
              ></map-pin-icon>
              Angola, luanda
            </p>
            <ul class="list-inline pt-4">
              <li class="list-inline-item me-3">
                <a
                  href="javascript: void(0);"
                  class="social-icon icon-mono avatar-xs rounded-circle"
                  ><facebook-icon class="icon-xs"></facebook-icon
                ></a>
              </li>
              <li class="list-inline-item me-3">
                <a
                  href="javascript: void(0);"
                  class="social-icon icon-mono avatar-xs rounded-circle"
                  ><twitter-icon class="icon-xs"></twitter-icon
                ></a>
              </li>
              <li class="list-inline-item">
                <a
                  href="javascript: void(0);"
                  class="social-icon icon-mono avatar-xs rounded-circle"
                  ><instagram-icon class="icon-xs"></instagram-icon
                ></a>
              </li>
            </ul>
          </div>
        </div>
        <!-- end col -->
      </div>
      <!-- end row -->
    </div>
    <!-- end container -->
  </section>
  <!-- Contact us end -->
</template>