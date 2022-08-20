<template>
  <div class="container mx-auto mb-12">
    <div class="text-center">
      <h1
        class="
          font-general-sans-medium
          text-3xl
          sm:text-4xl
          text-primary-dark
          dark:text-primary-light
          mb-5
        "
      >
        Sobre mi
      </h1>
    </div>
    <div
      class="grid sm:grid-cols-1 md:grid-cols-2 lg:grid-cols-2 xl:grid-cols-2"
    >
      <div class="flex justify-center mb-2">
        <img
          src="@/assets/img/jaime.jpg"
          alt=""
          class="
            rounded-full
            sm:rounded-full
            md:rounded-none
            lg:rounded-none
            xl:rounded-none
          "
          style="width: 300px"
        />
      </div>
      <div
        class="flex items-center font-general-sans-medium text-gray-400 px-2"
      >
        <p>
          Soy un Programador Web Full-Stack que desarrolla aplicaciones en:
          Symfony, Laravel, VueJS, JavaScript, JQuery y en entornos de
          despliegue como: Docker. Me considero una persona curiosa, resolutiva
          y capaz de trabajar en equipo.
        </p>
      </div>
    </div>
    <div class="text-center">
      <h1
        class="
          font-general-sans-medium
          text-3xl
          sm:text-4xl
          text-primary-dark
          dark:text-primary-light
          mb-5
          mt-5
        "
      >
        Experiencias
      </h1>
    </div>
    <div
      class="
        grid
        sm:ml-2 sm:grid-cols-1
        md:grid-cols-2
        lg:grid-cols-2
        xl:grid-cols-2
        px-2
      "
    >
      <div
        class="
          sm:text-start
          md:text-end
          lg:text-end
          xl:text-end
          sm:mr-0
          md:mr-4
          lg:mr-4
          xl:mr-4
        "
      >
        <div class="font-general-sans-medium mb-5">
          <p>Educación</p>
        </div>
        <div class="font-general-sans-medium text-gray-400 mb-5">
          <ul>
            <li><font-awesome-icon icon="fa-solid fa-map-pin" /> 2018</li>
            <li>Máster Javascript: JS, JQUERY, ANGULAR 6 Y NODEJS</li>
            <li>
              Máster desarrollo web completo: HTML5, CSS3, AJAX, PHP Y MYSQL
            </li>
            <li>Plataforma Udemy</li>
          </ul>
        </div>
        <div class="font-general-sans-medium text-gray-400 mb-5">
          <ul>
            <li>
              <font-awesome-icon icon="fa-solid fa-map-pin" /> 2016 - 2017
            </li>
            <li>Técnico superior en desarrollo de aplicaciones web</li>
            <li>IES Juan de Garay</li>
          </ul>
        </div>
        <div class="font-general-sans-medium text-gray-400">
          <ul>
            <li>
              <font-awesome-icon icon="fa-solid fa-map-pin" /> 2014 - 2016
            </li>
            <li>
              Técnico superior en desarrollo de aplicaciones multiplataforma
            </li>
            <li>Centro de formación profesional ASES</li>
          </ul>
        </div>
      </div>
      <div class="text-start sm:ml-0 md:ml-4 lg:ml-4 xl:ml-4">
        <div class="font-general-sans-medium mb-5">
          <p>Profesional</p>
        </div>
        <div class="font-general-sans-medium text-gray-400 mb-5">
          <ul>
            <li>
              <font-awesome-icon icon="fa-solid fa-map-pin" /> Julio 2022 -
              Presente
            </li>
            <li>Programador Web Full-Stack en Grupo Tenea</li>
            <li>Participo en diferentes desarrollos para CaixaBank</li>
          </ul>
        </div>
        <div class="font-general-sans-medium text-gray-400 mb-5">
          <ul>
            <li>
              <font-awesome-icon icon="fa-solid fa-map-pin" /> Diciembre 2020 -
              Junio 2022
            </li>
            <li>Programador Web Full-Stack en Premium Numbers</li>
            <li>
              Participación en el desarrollo de centralitas virtuales y
              aplicaciones de gestión
            </li>
          </ul>
        </div>
        <div class="font-general-sans-medium text-gray-400 mb-5">
          <ul>
            <li>
              <font-awesome-icon icon="fa-solid fa-map-pin" /> Diciembre 2018 -
              Octubre 2020
            </li>
            <li>Programador Web Full-Stack en Witrac</li>
            <li>
              Participación en proyectos de geolocalización en tiempo real para
              clientes como: Mercadona, Ford, Logifruit, entre otros
            </li>
          </ul>
        </div>
        <div class="font-general-sans-medium text-gray-400 mb-5">
          <ul>
            <li>
              <font-awesome-icon icon="fa-solid fa-map-pin" /> Noviembre 2017 -
              Agosto 2018
            </li>
            <li>Consultor Junior de oracle en Capgemini</li>
            <li>
              Soporte técnico a los hospitales de la Comunidad Valenciana dentro
              del proyecto Orion Logis
            </li>
          </ul>
        </div>
        <div class="font-general-sans-medium text-gray-400 mb-5">
          <ul>
            <li><font-awesome-icon icon="fa-solid fa-map-pin" /> 2017</li>
            <li>Prácticas formativas en Dusnic</li>
            <li>
              Participación en el desarrollo de una web interna para la empresa
            </li>
          </ul>
        </div>
        <div class="font-general-sans-medium text-gray-400">
          <ul>
            <li><font-awesome-icon icon="fa-solid fa-map-pin" /> 2016</li>
            <li>Prácticas formativas en Carcrash</li>
            <li>Desarrollo de dos apps para la empresa con Ionic</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>
