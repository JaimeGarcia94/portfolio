<script>
import emailjs from "@emailjs/browser";
export default {
  name: "ContactView",
  props: {},
  methods: {
    sendEmail() {
      emailjs
        .sendForm(
          "service_cfucjfh",
          "template_gtchhos",
          this.$refs.form,
          "DwmqeVGuD9uOuSwQ2"
        )
        .then(
          () => {
            alert("El mensaje se ha enviado correctamente");
            this.$refs.form.reset();
          },
          (error) => {
            alert("El mensaje no se ha podido enviar", error);
            this.$refs.form.reset();
          }
        );
    },
  },
};
</script>
<template>
  <div class="container mx-auto">
    <div
      class="
        grid
        sm:grid-cols-1
        md:grid-cols-2
        lg:grid-cols-2
        xl:grid-cols-2
        2xl:grid-cols-2
        mb-12
      "
    >
      <!-- formulario contacto -->
      <div class="leading-loose">
        <form
          ref="form"
          @submit.prevent="sendEmail"
          class="
            max-w-xl
            m-4
            p-6
            sm:p-10
            bg-secondary-light
            dark:bg-secondary-dark
            rounded-lg
            shadow-xl
            text-left
          "
        >
          <input type="hidden" name="from_name" value="Jaime" />
          <p
            class="
              text-primary-dark
              dark:text-primary-light
              text-2xl
              font-semibold
              mb-8
            "
          >
            Formulario de contacto
          </p>
          <div class="">
            <label
              class="
                block
                text-lg text-primary-dark
                dark:text-primary-light
                mb-2
                font-general-sans-medium
                text-gray-400
              "
              for="user_name_label"
              >Nombre</label
            >
            <input
              class="
                w-full
                px-5
                py-2
                border-0
                text-primary-dark
                dark:text-secondary-light
                bg-ternary-light
                dark:bg-primary-dark
                rounded-md
                shadow-sm
                text-md
                dark:font-medium
              "
              id="name"
              name="user_name"
              type="text"
              required=""
              placeholder="Escriba su nombre"
              aria-label="Name"
            />
          </div>
          <div class="mt-6">
            <label
              class="
                block
                text-lg text-primary-dark
                dark:text-primary-light
                mb-2
                font-general-sans-medium
                text-gray-400
              "
              for="user_email_label"
              >Email</label
            >
            <input
              class="
                w-full
                px-5
                py-2
                border-0
                text-primary-dark
                dark:text-secondary-light
                bg-ternary-light
                dark:bg-primary-dark
                rounded-md
                shadow-sm
                text-md
                dark:font-medium
              "
              id="email"
              name="user_email"
              type="email"
              required=""
              placeholder="Escriba su email"
              aria-label="Email"
            />
          </div>

          <div class="mt-6">
            <label
              class="
                block
                text-lg text-primary-dark
                dark:text-primary-light
                mb-2
                font-general-sans-medium
                text-gray-400
              "
              for="message_label"
              >Mensaje</label
            >
            <textarea
              class="
                w-full
                px-5
                py-2
                border-0
                text-primary-dark
                dark:text-secondary-light
                bg-ternary-light
                dark:bg-primary-dark
                rounded-md
                shadow-sm
                text-md
                dark:font-medium
              "
              id="message"
              name="message"
              cols="14"
              rows="6"
              aria-label="Message"
            ></textarea>
          </div>

          <div class="mt-6">
            <button
              type="submit"
              class="
                flex
                justify-center
                items-center
                w-36
                sm:w-48
                mt-12
                mb-6
                sm:mb-0
                text-lg
                border border-indigo-200
                dark:border-ternary-dark
                py-2.5
                sm:py-3
                shadow-lg
                rounded-lg
                bg-indigo-50
                focus:ring-1 focus:ring-indigo-900
                hover:bg-indigo-500
                text-gray-500
                hover:text-white
                duration-500
              "
            >
              <font-awesome-icon icon="fa-solid fa-paper-plane" />
              <span class="ml-2 font-general-sans-medium"> Enviar</span>
            </button>
          </div>
        </form>
      </div>

      <!-- detalles contacto -->
      <div class="px-4">
        <h2
          class="
            text-2xl text-primary-dark
            dark:text-primary-light
            font-semibold
            mt-12
            mb-8
          "
        >
          Detalles del contacto
        </h2>
        <ul
          class="
            max-w-xl
            bg-secondary-light
            dark:bg-secondary-dark
            font-general-sans-medium
            text-gray-400
          "
        >
          <li class="text-lg mb-4 text-primary-dark dark:text-ternary-light">
            <font-awesome-icon icon="fa-solid fa-map-location-dot" />
            Valencia, España
          </li>
          <li class="text-lg mb-4 text-primary-dark dark:text-ternary-light">
            <font-awesome-icon icon="fa-solid fa-envelope" />
            jaimegarciagar94@gmail.com
          </li>
          <li class="text-lg mb-4 text-primary-dark dark:text-ternary-light">
            <font-awesome-icon icon="fa-solid fa-phone" /> +34 648861674
          </li>
          <li>
            <div style="width: 100%">
              <iframe
                width="100%"
                height="400"
                frameborder="0"
                scrolling="no"
                marginheight="0"
                marginwidth="0"
                src="https://maps.google.com/maps?width=100%25&amp;height=600&amp;hl=es&amp;q=Valencia,%20Espa%C3%B1a+(Mi%20nombre%20de%20egocios)&amp;t=&amp;z=14&amp;ie=UTF8&amp;iwloc=B&amp;output=embed"
                ><a href="https://www.gps.ie/car-satnav-gps/"
                  >GPS devices</a
                ></iframe
              >
            </div>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style>
.bg-ternary-light {
  --tw-bg-opacity: 1;
  background-color: rgba(246, 247, 248, var(--tw-bg-opacity)) !important;
}
</style>