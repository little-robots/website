<template>
  <!-- eslint-disable -->
  <div>
    <!-- MODAL -->
    <div class="col-md-4">
      <modal
        :show.sync="showModal"
        :gradient="modalType"
        modal-classes="modal-danger modal-dialog-centered"
      >
        <!-- <h6
          slot="header"
          class="modal-title"
          id="modal-title-notification"
        >Your attention is required</h6>-->

        <div class="py-3 text-center">
          <i class="ni ni-bell-55 ni-3x"></i>
          <h4 class="heading mt-4">{{ modalTitle }}</h4>
          <p>{{ modalBody }}</p>
        </div>

        <template slot="footer">
          <!-- <base-button type="white">Ok, Got it</base-button> -->
          <base-button
            type="link"
            text-color="white"
            class="ml-auto"
            @click="showModal = false"
          >Cerrar</base-button>
        </template>
      </modal>
    </div>

    <div class="position-relative">
      <!-- shape Hero -->
      <section class="section-shaped my-0">
        <!-- <div class="shape shape-style-1 shape-default shape-skew" style="background-image: url('img/board.png'); background-size: cover;"> -->
        <div class="shape shape-style-1 shape-default shape-skew">
          <span></span>
          <span></span>
          <span></span>
          <span></span>
          <span></span>
          <span></span>
          <span></span>
          <span></span>
          <span></span>
        </div>
        <div class="container shape-container d-flex">
          <div class="col px-0">
            <div class="row">
              <div class="col-lg-6">
                <h1 class="display-3 text-white">
                  Cursos de robótica
                  <span>para principiantes</span>
                </h1>
                <p
                  class="lead text-white"
                >Aprendé a trabajar sobre las plataformas de hardware y software más populares de la actualidad.</p>
                <!-- <div class="btn-wrapper">
                                    <base-button tag="a"
                                                 href="https://demos.creative-tim.com/argon-design-system/docs/components/alerts.html"
                                                 class="mb-3 mb-sm-0"
                                                 type="info"
                                                 icon="fa fa-code">
                                        Conocé más
                                    </base-button>
                                    <base-button tag="a"
                                                 href="https://www.creative-tim.com/product/argon-design-system"
                                                 class="mb-3 mb-sm-0"
                                                 type="white"
                                                 icon="ni ni-cloud-download-95">
                                        Quiero anotarme
                                    </base-button>
                </div>-->
              </div>
            </div>
          </div>
        </div>
      </section>
      <!-- 1st Hero Variation -->
    </div>
    <section class="section section-lg pt-lg-0 mt--200">
      <div class="container">
        <div class="row justify-content-center">
          <div class="col-lg-12">
            <div class="row row-grid">
              <div class="col-lg-4">
                <img src="@/assets/breadboard.jpg" class="img-fluid" alt />
                <card class="border-0" hover shadow body-classes="py-5">
                  <!-- <icon name="ni ni-check-bold" type="primary" rounded class="mb-4">
                  </icon>-->
                  <h6 class="text-primary text-uppercase">Introducción a la robótica</h6>
                  <p
                    class="description mt-3"
                  >Aprendé los concéptos básicos de la programación y la electrónica mediante al uso de la plataforma de desarrollo más popular de la actualidad: Arduino.</p>
                  <p
                    class="description mt-3"
                  >Integra tus conocimientos trabajando con proyectos de robótica simples pero desafiantes.</p>
                  <div>
                    <badge type="primary" rounded>nivel: inicial</badge>
                    <badge type="primary" rounded>arduino</badge>
                    <badge type="primary" rounded>c</badge>
                  </div>
                  <base-button
                    @click="showCourse1 = true"
                    tag="a"
                    href="/course-01"
                    type="primary"
                    class="mt-4"
                  >Ver más</base-button>
                </card>
              </div>
              <div class="col-lg-4">
                <img src="@/assets/car.jpg" class="img-fluid" alt />
                <card class="border-0" hover shadow body-classes="py-5">
                  <h6 class="text-success text-uppercase">Curso intermedio de Robótica</h6>
                  <p
                    class="description mt-3"
                  >Aprendé sobre funcionalidades avanzadas de Arduino y programación.</p>
                  <p
                    class="description mt-3"
                  >Trabajá con proyectos más complejos con un mayór foco en la parte mecánica.</p>
                  <div>
                    <badge type="success" rounded>nivel: intermedio</badge>
                    <badge type="success" rounded>arduino</badge>
                    <badge type="success" rounded>c++</badge>
                  </div>
                  <base-button disabled type="success" class="mt-4">Próximamente</base-button>
                </card>
              </div>
              <div class="col-lg-4">
                <img src="@/assets/rpi.jpg" class="img-fluid" alt />
                <card class="border-0" hover shadow body-classes="py-5">
                  <h6 class="text-warning text-uppercase">Curso avanzado de Robótica</h6>
                  <p
                    class="description mt-3"
                  >Amplia tus posibilidades aprendiendo sobre la microcomputadora Raspberry Pi.</p>
                  <p
                    class="description mt-3"
                  >Aprendé sobre domótica y Internet of Things (IoT). Integrá tus proyectos con otros sistemas en internet.</p>
                  <div>
                    <badge type="warning" rounded>nivel: avanzado</badge>
                    <badge type="warning" rounded>Raspberry Pi</badge>
                    <badge type="warning" rounded>js</badge>
                  </div>
                  <base-button disabled type="warning" class="mt-4">Próximamente</base-button>
                </card>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="section section section-shaped my-0 overflow-hidden">
      <div class="shape shape-style-1 bg-gradient-warning shape-skew">
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
      </div>
      <div class="container py-0">
        <div class="row row-grid align-items-center">
          <div class="col-md-6 order-lg-2 ml-lg-auto">
            <div class="position-relative pl-md-5">
              <img src="img/ill/ill-2.svg" class="img-center img-fluid" />
            </div>
          </div>
          <div class="col-lg-6 order-lg-1">
            <div class="d-flex px-3">
              <!-- <div>
                                <icon name="ni ni-building" size="lg" class="bg-gradient-white" color="primary" shadow
                                      rounded></icon>
              </div>-->
              <div class="pl-4">
                <h4 class="display-3 text-white">Nuestra propuesta</h4>
                <p
                  class="text-white"
                >Creemos que la mejor forma de aprender es haciendo. Por eso te ofrecemos una propuesta integral que combina el trabajo en clase con asistencia continua durante la cursada.</p>
              </div>
            </div>
            <card shadow class="shadow-lg--hover mt-5">
              <div class="d-flex px-3">
                <div>
                  <icon name="ni ni-building" gradient="success" color="white" shadow rounded></icon>
                </div>
                <div class="pl-4">
                  <h5 class="title text-success">Cursos presenciales</h5>
                  <p>Dictamos los cursos de manera presencial en nuestras aulas ubicadas en Beccar, San Isidro. Contamos con todos los materiales necesarios, solamente necesitas una notebook.</p>
                </div>
              </div>
            </card>
            <card shadow class="shadow-lg--hover mt-5">
              <div class="d-flex px-3">
                <div>
                  <icon name="ni ni-badge" gradient="warning" color="white" shadow rounded></icon>
                </div>
                <div class="pl-4">
                  <h5 class="title text-warning">Consultas online</h5>
                  <p>Los alumnos tienen acceso a un canal de comunicación privado donde los acompañamos con cualquier consulta o inquietud que tengan fuera de clase.</p>
                </div>
              </div>
            </card>
          </div>
        </div>
      </div>
    </section>
    <section class="section section-lg">
      <div class="container">
        <div class="row justify-content-center text-center mb-lg">
          <div class="col-lg-8">
            <h2 class="display-3">Nosotros</h2>
            <p
              class="lead text-muted"
            >Contamos con años de experiencia profesional en la industria del software y la electrónica. Hace cuatro años dictamos diversos cursos de programación, robótica, matemática y física para alumnos de nivel secundario.</p>
          </div>
        </div>
        <div class="row">
          <div class="col-md-6 col-lg-6 mb-5 mb-lg-0">
            <div class="px-4">
              <img
                src="img/theme/nitt.jpg"
                class="rounded-circle img-center img-fluid shadow shadow-lg--hover"
                style="width: 200px;"
              />
              <div class="pt-4 text-center">
                <h5 class="title">
                  <span class="d-block mb-1">Juan</span>
                  <small class="h6 text-muted">Ing. Informático (UBA)</small>
                </h5>
              </div>
            </div>
          </div>
          <div class="col-md-6 col-lg-6 mb-5 mb-lg-0">
            <div class="px-4">
              <img
                src="img/theme/tomi.jpeg"
                class="rounded-circle img-center img-fluid shadow shadow-lg--hover"
                style="width: 200px;"
              />
              <div class="pt-4 text-center">
                <h5 class="title">
                  <span class="d-block mb-1">Tomi</span>
                  <small class="h6 text-muted">Ing. Electrónico (ITBA)</small>
                </h5>
              </div>
            </div>
          </div>
          <!-- <div class="col-md-6 col-lg-3 mb-5 mb-lg-0">
                        <div class="px-4">
                            <img v-lazy="'img/theme/team-3-800x800.jpg'"
                                 class="rounded-circle img-center img-fluid shadow shadow-lg--hover"
                                 style="width: 200px;">
                            <div class="pt-4 text-center">
                                <h5 class="title">
                                    <span class="d-block mb-1">Alexander Smith</span>
                                    <small class="h6 text-muted">UI/UX Designer</small>
                                </h5>
                                <div class="mt-3">
                                    <base-button tag="a" href="#" type="info" icon="fa fa-twitter" rounded
                                                 icon-only></base-button>
                                    <base-button tag="a" href="#" type="info" icon="fa fa-facebook" rounded
                                                 icon-only></base-button>
                                    <base-button tag="a" href="#" type="info" icon="fa fa-dribbble" rounded
                                                 icon-only></base-button>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-6 col-lg-3 mb-5 mb-lg-0">
                        <div class="px-4">
                            <img v-lazy="'img/theme/team-4-800x800.jpg'"
                                 class="rounded-circle img-center img-fluid shadow shadow-lg--hover"
                                 style="width: 200px;">
                            <div class="pt-4 text-center">
                                <h5 class="title">
                                    <span class="d-block mb-1">John Doe</span>
                                    <small class="h6 text-muted">Founder and CEO</small>
                                </h5>
                                <div class="mt-3">
                                    <base-button tag="a" href="#" type="success" icon="fa fa-twitter" rounded
                                                 icon-only></base-button>
                                    <base-button tag="a" href="#" type="success" icon="fa fa-facebook" rounded
                                                 icon-only></base-button>
                                    <base-button tag="a" href="#" type="success" icon="fa fa-dribbble" rounded
                                                 icon-only></base-button>
                                </div>
                            </div>
                        </div>
          </div>-->
        </div>
      </div>
    </section>
    <section class="section section-shaped my-0 overflow-hidden">
      <div class="shape shape-style-3 bg-gradient-default shape-skew">
        <span></span>
        <span></span>
        <span></span>
        <span></span>
      </div>
      <div id="contactanos" class="container pt-lg pb-300">
        <div class="row text-center justify-content-center">
          <div class="col-lg-10">
            <h2 class="display-3 text-white">Contactanos</h2>
            <p class="lead text-white">
              Si estás interesado en alguno de los cursos o querés hacernos una consulta podés contactarnos vía mail a
              <a
                href="mailto:roboticalittlerobots@gmail.com"
              >roboticalittlerobots@gmail.com</a>, por nuestro
              <a href="https://www.instagram.com/roboticalittlerobots/">instagram</a> o dejanos tus datos:
            </p>
          </div>
        </div>
        <!-- <div class="row row-grid mt-5">
                    <div class="col-lg-4">
                        <icon name="ni ni-settings" size="lg" gradient="white" shadow round color="primary"></icon>
                        <h5 class="text-white mt-3">Building tools</h5>
                        <p class="text-white mt-3">Some quick example text to build on the card title and make up the
                            bulk of the card's content.</p>
                    </div>
                    <div class="col-lg-4">
                        <icon name="ni ni-ruler-pencil" size="lg" gradient="white" shadow round color="primary"></icon>
                        <h5 class="text-white mt-3">Grow your market</h5>
                        <p class="text-white mt-3">Some quick example text to build on the card title and make up the
                            bulk of the card's content.</p>
                    </div>
                    <div class="col-lg-4">
                        <icon name="ni ni-atom" size="lg" gradient="white" shadow round color="primary"></icon>
                        <h5 class="text-white mt-3">Launch time</h5>
                        <p class="text-white mt-3">Some quick example text to build on the card title and make up the
                            bulk of the card's content.</p>
                    </div>
        </div>-->
      </div>
    </section>
    <section class="section section-lg pt-lg-0 section-contact-us">
      <div class="container">
        <div class="row justify-content-center mt--300">
          <div class="col-lg-8">
            <card gradient="secondary" shadow body-classes="p-lg-5">
              <h4 class="mb-1">Tus datos</h4>
              <!-- <p class="mt-0">Dejanos tus datos</p> -->
              <base-input
                class="mt-5"
                alternative
                placeholder="Nombre"
                v-model="name"
                addon-left-icon="ni ni-user-run"
              ></base-input>
              <base-input
                alternative
                placeholder="Email"
                v-model="email"
                addon-left-icon="ni ni-email-83"
              ></base-input>
              <base-input
                alternative
                placeholder="Teléfono"
                v-model="phone"
                addon-left-icon="ni ni-bell-55"
              ></base-input>
              <base-input class="mb-4">
                <textarea
                  v-model="message"
                  class="form-control form-control-alternative"
                  name="name"
                  rows="4"
                  cols="80"
                  placeholder="Tu consulta..."
                ></textarea>
              </base-input>
              <base-button @click="sendContactForm" type="default" round block size="lg">Enviar</base-button>
            </card>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
// const { WebClient } = require('@slack/web-api')
import Modal from "@/components/Modal.vue"
import axios from 'axios'

axios.defaults.baseURL = 'https://slack.com/api'
// axios.defaults.headers.common[ 'Authorization' ] = process.env.VUE_APP_SLACK_TOKEN
axios.defaults.headers.post[ 'Content-Type' ] = 'application/x-www-form-urlencoded'

export default {
  name: "home",
  components: { Modal },
  data: () => {
    return {
      name: '',
      email: '',
      phone: '',
      message: '',
      showModal: false,
      showCourse1: false,
      modalTitle: '',
      modalBody: '',
      modalType: 'danger'
    }
  },
  methods: {
    sendContactForm: async function () {
      if (this.name.length > 0 && this.email.length > 0 && this.email.includes('@') && this.email.includes('.') && this.message.length > 0) {
        let text = `********* Nuevo contacto *********\nNombre: ${this.name}\nEmail: ${this.email}\nTeléfono: ${this.phone}\nMensaje: ${this.message}`
        // const web = new WebClient(process.env.VUE_APP_SLACK_TOKEN)
        // const res = await web.chat.postMessage({ channel: process.env.VUE_APP_SLACK_CHANNEL, text: text })
        try {
          const params = new URLSearchParams()
          params.append('token', process.env.VUE_APP_SLACK_TOKEN)
          params.append('channel', process.env.VUE_APP_SLACK_CHANNEL)
          params.append('text', text)
          let res = await axios.post('/chat.postMessage', params, { headers: { 'Content-Type': 'application/x-www-form-urlencoded' } })
          console.log(res)
          this.modalType = 'primary'
          this.modalTitle = 'Gracias por dejarnos un mensaje'
          this.modalBody = 'Te contactaremos a la brevedad.'
          this.showModal = true
          this.name = ''
          this.phone = ''
          this.message = ''
          this.email = ''
        } catch (error) {
          this.modalType = 'danger'
          this.modalTitle = 'Error'
          this.modalBody = 'No se pudo enviar el mensaje. Por favor contactanos vía email a roboticalittlerobots@gmail.com. Gracias!'
          this.showModal = true
        }

      } else {
        this.modalType = 'danger'
        this.modalTitle = 'Error'
        this.modalBody = 'Por favor completá tu nombre, email y tu consulta así podemos contactarte. Gracias!'
        this.showModal = true
      }
    }
  }
};
</script>
