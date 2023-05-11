<template>
  <div class="hello">
    <ul>
      <template v-for="(empleo, indice) in empleos" :key="indice">
        <li>
          <div data-v-03976c49="" data-v-66ca8794="">
            <div data-v-03976c49="" itemprop="https://schema.org/JobPosting" itemscope="itemscope" class="card job-card mb-3 border">
              <!---->
              <!---->
              <div data-v-03976c49="" class="card-body p-2 p-md-3">
                <!---->
                <!---->
                <div data-v-03976c49="" class="row align-items-center text-start">
                  <div data-v-03976c49="" class="justify-content-center align-items-center col-md-1 col-3">
                    <img data-v-03976c49="" src="https://png.pngtree.com/png-vector/20191004/ourmid/pngtree-building-icon-isolated-on-abstract-background-png-image_1780483.jpg" alt="Logo empresa" class="rounded" width="70" height="70">
                  </div>
                  <div data-v-03976c49="" class="col-md-11 col-9">
                    <div data-v-03976c49="" class="row align-items-center">
                      <div data-v-03976c49="" class="mb-2 col">
                        <a data-v-03976c49="" href="#" class="text-dark stretched-link d-inline d-md-inline-flex" itemprop="url" target="_self" style="text-decoration: none;">
                          <h2 data-v-03976c49="" itemprop="title" class="job-title bold pl-md-2 pr-md-2 mb-0 pb-0" style="font-size: 24px; font-weight: bold; margin-right: 5vh;"> {{ empleo.name }} </h2>
                          <section data-v-03976c49="" itemprop="skills" class="pl-md-2 d-inline d-md-inline-flex align-items-center text-truncate" v-for="(q, index) in empleo.qualifications" :key="index">
                            <div data-v-03976c49="" role="button" class="skill-tag text-truncate border border-dark text-dark text-capitalize rounded" style="font-size: 0.8em; margin-bottom: 0px !important; margin-inline: 1vh; padding: 0.8vh; border-radius: 20vh;">
                              <span data-v-03976c49=""></span> {{ q }}
                            </div>
                            <!-- <div data-v-03976c49="" role="button" class="skill-tag text-truncate border border-dark text-dark text-capitalize rounded" style="font-size: 0.8em; margin-bottom: 0px !important; margin-inline: 1vh; padding: 0.5vh; border-radius: 20vh;">
                              <span data-v-03976c49=""></span> assertive communication
                            </div>
                            <div data-v-03976c49="" role="button" class="skill-tag text-truncate border border-dark text-dark text-capitalize rounded" style="font-size: 0.8em; margin-bottom: 0px !important; margin-inline: 1vh; padding: 0.5vh; border-radius: 20vh;">
                              <span data-v-03976c49=""></span> attitude to service
                            </div> -->
                          </section>
                          <!---->
                          <!---->
                        </a>
                      </div>
                    </div>
                    <div data-v-03976c49="" class="row pl-md-2 mt-1 flex-column flex-md-row" style="font-size: 0.9em;">
                      <div data-v-03976c49="" itemprop="hiringOrganization" itemscope="itemscope" itemtype="http://schema.org/Organization" class="text-truncate text-capitalize col">
                        <svg data-v-03976c49="" viewBox="0 0 16 16" width="1em" height="1em" focusable="false" role="img" aria-label="building" xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="bi-building b-icon bi">
                          <g data-v-03976c49="">
                            <path fill-rule="evenodd" d="M14.763.075A.5.5 0 0 1 15 .5v15a.5.5 0 0 1-.5.5h-3a.5.5 0 0 1-.5-.5V14h-1v1.5a.5.5 0 0 1-.5.5h-9a.5.5 0 0 1-.5-.5V10a.5.5 0 0 1 .342-.474L6 7.64V4.5a.5.5 0 0 1 .276-.447l8-4a.5.5 0 0 1 .487.022zM6 8.694 1 10.36V15h5V8.694zM7 15h2v-1.5a.5.5 0 0 1 .5-.5h2a.5.5 0 0 1 .5.5V15h2V1.309l-7 3.5V15z"></path>
                            <path d="M2 11h1v1H2v-1zm2 0h1v1H4v-1zm-2 2h1v1H2v-1zm2 0h1v1H4v-1zm4-4h1v1H8V9zm2 0h1v1h-1V9zm-2 2h1v1H8v-1zm2 0h1v1h-1v-1zm2-2h1v1h-1V9zm0 2h1v1h-1v-1zM8 7h1v1H8V7zm2 0h1v1h-1V7zm2 0h1v1h-1V7zM8 5h1v1H8V5zm2 0h1v1h-1V5zm2 0h1v1h-1V5zm0-2h1v1h-1V3z"></path>
                          </g>
                        </svg>
                        <span data-v-03976c49="" itemprop="name" style="margin-inline: 1vh;"> {{ empleo.company }} </span>
                      </div>
                      <div data-v-03976c49="" itemprop="jobLocation" itemscope="itemscope" itemtype="http://schema.org/Place" class="text-truncate col">
                        <svg data-v-03976c49="" viewBox="0 0 16 16" width="1em" height="1em" focusable="false" role="img" aria-label="geo alt" xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="bi-geo-alt b-icon bi">
                          <g data-v-03976c49="">
                            <path d="M12.166 8.94c-.524 1.062-1.234 2.12-1.96 3.07A31.493 31.493 0 0 1 8 14.58a31.481 31.481 0 0 1-2.206-2.57c-.726-.95-1.436-2.008-1.96-3.07C3.304 7.867 3 6.862 3 6a5 5 0 0 1 10 0c0 .862-.305 1.867-.834 2.94zM8 16s6-5.686 6-10A6 6 0 0 0 2 6c0 4.314 6 10 6 10z"></path>
                            <path d="M8 8a2 2 0 1 1 0-4 2 2 0 0 1 0 4zm0 1a3 3 0 1 0 0-6 3 3 0 0 0 0 6z"></path>
                          </g>
                        </svg>
                        <span data-v-03976c49="" itemprop="name address" style="margin-inline: 1vh;"> {{ empleo.location }} </span>
                      </div>
                      <div data-v-03976c49="" itemprop="estimatedSalary baseSalary" class="text-truncate col">
                        <svg data-v-03976c49="" viewBox="0 0 16 16" width="1em" height="1em" focusable="false" role="img" aria-label="cash" xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="bi-cash b-icon bi">
                          <g data-v-03976c49="">
                            <path d="M8 10a2 2 0 1 0 0-4 2 2 0 0 0 0 4z"></path>
                            <path d="M0 4a1 1 0 0 1 1-1h14a1 1 0 0 1 1 1v8a1 1 0 0 1-1 1H1a1 1 0 0 1-1-1V4zm3 0a2 2 0 0 1-2 2v4a2 2 0 0 1 2 2h10a2 2 0 0 1 2-2V6a2 2 0 0 1-2-2H3z"></path>
                          </g>
                        </svg>
                        <span data-v-03976c49="" style="margin-inline: 1vh;"> {{ empleo.salary }} </span>
                      </div>
                      <div data-v-03976c49="" class="d-none d-md-inline-block col">
                        <svg data-v-03976c49="" viewBox="0 0 16 16" width="1em" height="1em" focusable="false" role="img" aria-label="people" xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="bi-people b-icon bi">
                          <g data-v-03976c49="">
                            <path d="M15 14s1 0 1-1-1-4-5-4-5 3-5 4 1 1 1 1h8zm-7.978-1A.261.261 0 0 1 7 12.996c.001-.264.167-1.03.76-1.72C8.312 10.629 9.282 10 11 10c1.717 0 2.687.63 3.24 1.276.593.69.758 1.457.76 1.72l-.008.002a.274.274 0 0 1-.014.002H7.022zM11 7a2 2 0 1 0 0-4 2 2 0 0 0 0 4zm3-2a3 3 0 1 1-6 0 3 3 0 0 1 6 0zM6.936 9.28a5.88 5.88 0 0 0-1.23-.247A7.35 7.35 0 0 0 5 9c-4 0-5 3-5 4 0 .667.333 1 1 1h4.216A2.238 2.238 0 0 1 5 13c0-1.01.377-2.042 1.09-2.904.243-.294.526-.569.846-.816zM4.92 10A5.493 5.493 0 0 0 4 13H1c0-.26.164-1.03.76-1.724.545-.636 1.492-1.256 3.16-1.275zM1.5 5.5a3 3 0 1 1 6 0 3 3 0 0 1-6 0zm3-2a2 2 0 1 0 0 4 2 2 0 0 0 0-4z"></path>
                          </g>
                        </svg> {{ empleo.vacancies }} Vacante(s)
                      </div>
                      <div data-v-03976c49="" class="text-truncate col">
                        <svg data-v-03976c49="" viewBox="0 0 16 16" width="1em" height="1em" focusable="false" role="img" aria-label="calendar3" xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="bi-calendar3 b-icon bi">
                          <g data-v-03976c49="">
                            <path d="M14 0H2a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V2a2 2 0 0 0-2-2zM1 3.857C1 3.384 1.448 3 2 3h12c.552 0 1 .384 1 .857v10.286c0 .473-.448.857-1 .857H2c-.552 0-1-.384-1-.857V3.857z"></path>
                            <path d="M6.5 7a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm3 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm3 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm-9 3a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm3 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm3 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm3 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm-9 3a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm3 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2zm3 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2z"></path>
                          </g>
                        </svg>
                        <!---->
                        <span data-v-03976c49="" itemprop="datePosted validThrough" class="sr-only" style="margin-inline: 1vh;"> {{ empleo.posting_date }} </span>
                        <!-- <time data-v-03976c49="" datetime="2023-05-10T15:16:59.686Z">about 23 hours ago</time> -->
                      </div>
                      <div data-v-03976c49="" class="text-truncate col d-flex align-items-center text-center">
                        <!---->
                        <div data-v-03976c49="" role="button" title="Certificaciones" class="skill-tag custom-skill-tag text-truncate border border-dark text-dark rounded" style="width: 2em; margin-inline: 1vh;">
                          <svg data-v-03976c49="" viewBox="0 0 16 16" width="1em" height="1em" focusable="false" role="img" aria-label="file earmark check" xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="bi-file-earmark-check b-icon bi">
                            <g data-v-03976c49="">
                              <path d="M10.854 7.854a.5.5 0 0 0-.708-.708L7.5 9.793 6.354 8.646a.5.5 0 1 0-.708.708l1.5 1.5a.5.5 0 0 0 .708 0l3-3z"></path>
                              <path d="M14 14V4.5L9.5 0H4a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h8a2 2 0 0 0 2-2zM9.5 3A1.5 1.5 0 0 0 11 4.5h2V14a1 1 0 0 1-1 1H4a1 1 0 0 1-1-1V2a1 1 0 0 1 1-1h5.5v2z"></path>
                            </g>
                          </svg>
                        </div>
                        <div data-v-03976c49="" role="button" title="Fiesta de fin de año" class="skill-tag custom-skill-tag text-truncate border border-dark text-dark rounded" style="width: 2em; margin-inline: 1vh;">
                          <svg data-v-03976c49="" viewBox="0 0 16 16" width="1em" height="1em" focusable="false" role="img" aria-label="emoji sunglasses" xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="bi-emoji-sunglasses b-icon bi">
                            <g data-v-03976c49="">
                              <path d="M4.968 9.75a.5.5 0 1 0-.866.5A4.498 4.498 0 0 0 8 12.5a4.5 4.5 0 0 0 3.898-2.25.5.5 0 1 0-.866-.5A3.498 3.498 0 0 1 8 11.5a3.498 3.498 0 0 1-3.032-1.75zM7 5.116V5a1 1 0 0 0-1-1H3.28a1 1 0 0 0-.97 1.243l.311 1.242A2 2 0 0 0 4.561 8H5a2 2 0 0 0 1.994-1.839A2.99 2.99 0 0 1 8 6c.393 0 .74.064 1.006.161A2 2 0 0 0 11 8h.438a2 2 0 0 0 1.94-1.515l.311-1.242A1 1 0 0 0 12.72 4H10a1 1 0 0 0-1 1v.116A4.22 4.22 0 0 0 8 5c-.35 0-.69.04-1 .116z"></path>
                              <path d="M16 8A8 8 0 1 1 0 8a8 8 0 0 1 16 0zm-1 0A7 7 0 1 0 1 8a7 7 0 0 0 14 0z"></path>
                            </g>
                          </svg>
                        </div>
                        <div data-v-03976c49="" role="button" title="Capacitaciones" class="skill-tag custom-skill-tag text-truncate border border-dark text-dark rounded" style="width: 2em; margin-inline: 1vh;">
                          <svg data-v-03976c49="" viewBox="0 0 16 16" width="1em" height="1em" focusable="false" role="img" aria-label="clipboard check" xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="bi-clipboard-check b-icon bi">
                            <g data-v-03976c49="">
                              <path fill-rule="evenodd" d="M10.854 7.146a.5.5 0 0 1 0 .708l-3 3a.5.5 0 0 1-.708 0l-1.5-1.5a.5.5 0 1 1 .708-.708L7.5 9.793l2.646-2.647a.5.5 0 0 1 .708 0z"></path>
                              <path d="M4 1.5H3a2 2 0 0 0-2 2V14a2 2 0 0 0 2 2h10a2 2 0 0 0 2-2V3.5a2 2 0 0 0-2-2h-1v1h1a1 1 0 0 1 1 1V14a1 1 0 0 1-1 1H3a1 1 0 0 1-1-1V3.5a1 1 0 0 1 1-1h1v-1z"></path>
                              <path d="M9.5 1a.5.5 0 0 1 .5.5v1a.5.5 0 0 1-.5.5h-3a.5.5 0 0 1-.5-.5v-1a.5.5 0 0 1 .5-.5h3zm-3-1A1.5 1.5 0 0 0 5 1.5v1A1.5 1.5 0 0 0 6.5 4h3A1.5 1.5 0 0 0 11 2.5v-1A1.5 1.5 0 0 0 9.5 0h-3z"></path>
                            </g>
                          </svg>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
              <!---->
              <!---->
            </div>
          </div>
        </li>

        <!-- <li :style="fruta.amount<=5 ? 'color: red' : ''" v-if="fruta.amount > 0">
          {{ fruta.name }} ({{ fruta.amount }}) -> ${{ fruta.price }} 
          <button @click="venderUno(fruta)">
            Vender uno
          </button>
          &nbsp;
          <button @click="fruta.amount++">
            Comprar uno
          </button> 
        </li>
        <span v-else>No tiene más de 0</span> -->
      </template>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
    number: Number,
  },
  data() {
    return {
      // nombre: "Santiago",
      empleos: [
        {
          name: "Desarrollador Java",
          company: "Assemblers S.A.",
          location: "Remoto",
          vacancies: 2,
          qualifications: {
            a:"Java",
            b: "Spring MVC",
            c: "PostgreSQL"
          },
          salary: "$ 3.5M - 5M COP",
          posting_date: "11/05/2023"
        },
        {
          name: "Desarrollador PHP",
          company: "Developers United",
          location: "Bogotá",
          vacancies: 1,
          qualifications: {
            a: "PHP",
            b: "Laravel",
          },
          salary: "$ 4M COP",
          posting_date: "02/05/2023"
        },
        {
          name: "Desarrollador Senior",
          company: "Developers United",
          location: "Medellín",
          vacancies: 1,
          qualifications: {
            a: "JavaScript",
            b: "React",
            c: "MySQL/MariaDB"
          },
          salary: "$ 4M COP",
          posting_date: "22/04/2023"
        },
        {
          name: "Diseñador Gráfico",
          company: "Neuro",
          location: "Remoto",
          vacancies: 2,
          qualifications: {
            a: "Diseño vectorial",
            b: "Illustrator",
          },
          salary: "$ 2M COP",
          posting_date: "22/04/2023"
        },
        {
          name: "Enfermera Profesional",
          company: "TuMedical",
          location: "Barranquilla",
          vacancies: 1,
          qualifications: {
            a: "Seguridad laboral",
            b: "Lenguaje de señas",
            c: "Min. 1 año de experiencia"
          },
          salary: "$ 3M - 4M COP",
          posting_date: "10/05/2023"
        },
        {
          name: "Asesor comercial",
          company: "Activos S.A.",
          location: "Cali",
          vacancies: 10,
          qualifications: {
            a: "Inglés",
            b: "Atención al usuario",
            c: "Comunicación asertiva",
            d: "Herramientas ofimáticas"
          },
          salary: "$ 2.2M COP + prestaciones y comisiones",
          posting_date: "11/05/2023"
        },
        {
          name: "Operario de aseo",
          company: "Tu Casa Limpia",
          location: "Medellín",
          vacancies: 5,
          qualifications: {
            a: "No se requiere educación superior",
            b: "Experiencia en alturas",
          },
          salary: "$ 1.2M COP + prestaciones y bonos",
          posting_date: "22/04/2023"
        },
        {
          name: "Auxiliar de cocina",
          company: "La Rioja",
          location: "Cartagena",
          vacancies: 1,
          qualifications: {
            a: "Curso de manipulación de alimentos",
            b: "Buena presentación",
            c: "Profesional en culinaria"
          },
          salary: "$ 2M COP",
          posting_date: "30/04/2023"
        },
        {
          name: "DevOps",
          company: "Array World",
          location: "Remoto",
          vacancies: 1,
          qualifications: {
            a: "Azure Cloud",
            b: "Python",
            c: "Node JS"
          },
          salary: "$ 7M COP",
          posting_date: "19/04/2023"
        },
        {
          name: "Call Center (Medio tiempo)",
          company: "BCall",
          location: "Bogotá",
          vacancies: 15,
          qualifications: {
            a: "Servicio al cliente",
            b: "Inglés C1",
            c: "Herramientas ofimáticas"
          },
          salary: "$ 2M COP + prestaciones y bonos",
          posting_date: "28/04/2023"
        },
      ],
      // ventas: 0
    }
  },
  // methods: {
  //   venderUno(fruta) {
  //     fruta.amount--;
  //     fruta.name = this.cambiartitulo(fruta);
  //     this.ventas++;
  //   },
  //   cambiartitulo(fruta) {
  //     return fruta.name.toUpperCase();
  //   }
  // },
  beforeCreate(){
    console.log("Existe el deseo de graficar la página")
  },
  created() {
    console.log("Ya sabemos que se puede crear y hay información disponible para crearla")
  },
  beforeMount() {
    console.log("Tenemos la información y vamos a empezar a graficar")    
  },
  mounted() {
    console.log("Se graficó la página")    
  },
  beforeUnmount() {
    console.log("Hay un deseo de abandonar la página")
  },
  unmounted() {
    console.log("Salimos de la página")
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  /* display: inline-block; */
  margin: 0 10vh 0 10vh; 
}
a {
  color: #42b983;
}
</style>
