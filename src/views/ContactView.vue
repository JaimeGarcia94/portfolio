<script>
import emailjs from '@emailjs/browser';
export default {
  name: "ContactView",
  props: {},
  methods: {
    sendEmail() {
      emailjs.sendForm('service_cfucjfh', 'template_gtchhos', this.$refs.form, 'DwmqeVGuD9uOuSwQ2')
        .then((result) => {
            console.log('SUCCESS!', result.text);
        }, (error) => {
            console.log('FAILED...', error.text);
        });
    }
  },
};
</script>
<template>
  <div class="container mx-auto min-h-screen" style="border: 1px solid red">

  <div class="text-center py-4">
      <h1>Contact</h1>
    </div>
   
  <form ref="form" class="grid place-items-center content-center py-12">
    <input type="hidden" name="from_name" value="Jaime">
    <div class="relative z-0 w-full px-4 sm:w-full md:w-96 lg:w-96 xl:w-96 2xl:w-96 mb-6 group">
        <input type="text" name="user_name" v-model="name" id="floating_first_name" class="block py-2.5 px-0 w-full text-sm text-gray-900 bg-transparent border-0 border-b-2 border-gray-300 appearance-none dark:text-white dark:border-gray-600 dark:focus:border-blue-500 focus:outline-none focus:ring-0 focus:border-blue-600 peer" placeholder=" ">
        <label for="user_name_label" class="peer-focus:font-medium absolute text-sm text-gray-500 dark:text-gray-400 duration-300 transform -translate-y-6 scale-75 top-3 -z-10 origin-[0] peer-focus:left-0 peer-focus:text-blue-600 peer-focus:dark:text-blue-500 peer-placeholder-shown:scale-100 peer-placeholder-shown:translate-y-0 peer-focus:scale-75 peer-focus:-translate-y-6">First name</label>
    </div>

    <div class="relative z-0 w-full px-4 sm:w-full md:w-96 lg:w-96 xl:w-96 2xl:w-96 mb-6 group">
        <input type="email" name="user_email" v-model="email" class="block py-2.5 px-0 w-full text-sm text-gray-900 bg-transparent border-0 border-b-2 border-gray-300 appearance-none dark:text-white dark:border-gray-600 dark:focus:border-blue-500 focus:outline-none focus:ring-0 focus:border-blue-600 peer" placeholder=" ">
        <label for="user_email_label" class="peer-focus:font-medium absolute text-sm text-gray-500 dark:text-gray-400 duration-300 transform -translate-y-6 scale-75 top-3 -z-10 origin-[0] peer-focus:left-0 peer-focus:text-blue-600 peer-focus:dark:text-blue-500 peer-placeholder-shown:scale-100 peer-placeholder-shown:translate-y-0 peer-focus:scale-75 peer-focus:-translate-y-6">Email address</label>
    </div>

    <div class="relative z-0 w-full px-4 sm:w-full md:w-96 lg:w-96 xl:w-96 2xl:w-96 mb-6 group">
        <textarea rows="4" name="message" v-model="text" class="block py-2.5 px-0 w-full text-sm text-gray-900 bg-transparent border-0 border-b-2 border-gray-300 appearance-none dark:text-white dark:border-gray-600 dark:focus:border-blue-500 focus:outline-none focus:ring-0 focus:border-blue-600 peer" placeholder=" "></textarea>
        <label for="message_label" class="peer-focus:font-medium absolute text-sm text-gray-500 dark:text-gray-400 duration-300 transform -translate-y-6 scale-75 top-3 -z-10 origin-[0] peer-focus:left-0 peer-focus:text-blue-600 peer-focus:dark:text-blue-500 peer-placeholder-shown:scale-100 peer-placeholder-shown:translate-y-0 peer-focus:scale-75 peer-focus:-translate-y-6">Message</label>
    </div>
    
    
    <button @submit.prevent="sendEmail" class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm w-full sm:w-full md:w-96 lg:w-96 xl:w-96 2xl:w-96 px-4 py-2.5 text-center dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">Send</button>
  </form>

</div>
</template>

<!-- <template>
  <form ref="form" @submit.prevent="sendEmail">
    <input type="hidden" name="from_name" value="Jaime">
    <label>Name</label>
    <input type="text" name="user_name">
    <label>Email</label>
    <input type="email" name="user_email">
    <label>Message</label>
    <textarea name="message"></textarea>
    <button type="submit" value="Send">send</button>
  </form>
</template>

<script>
import emailjs from '@emailjs/browser';

export default {
  methods: {
    sendEmail() {
      emailjs.sendForm('service_cfucjfh', 'template_gtchhos', this.$refs.form, 'DwmqeVGuD9uOuSwQ2')
        .then((result) => {
            console.log('SUCCESS!', result.text);
        }, (error) => {
            console.log('FAILED...', error.text);
        });
    }
  }
}
</script> -->