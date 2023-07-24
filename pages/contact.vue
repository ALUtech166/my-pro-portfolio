<template>
  <div class="">

    <div class="tw-relative tw-w-full tw-h-72">
      <img class="tw-absolute tw-top-0 tw-left-0 tw-w-full tw-h-full tw-object-cover"
        src="https://img.freepik.com/free-photo/top-view-workspace-with-notebook-succulent-plant_23-2148430820.jpg?w=740&t=st=1690220651~exp=1690221251~hmac=a7249088cdb9fbe455226feccdb5ea68d2bd60b9c7ae35f497131c6e9a06e731"
        alt="Banner Image">
      <div
        class="tw-relative tw-w-full tw-h-full tw-flex tw-flex-col tw-justify-center tw-items-center tw-bg-gray-900 tw-bg-opacity-60">
        <h1 class="tw-text-4xl tw-font-bold tw-text-white" data-aos="fade-up">Contact Us</h1>
      </div>
    </div>
    <div class="tw-flex tw-items-center tw-space-x-2 tw-px-8">
      <v-breadcrumbs :items="breadcrumbItems" divider="/" class="tw-text-lg tw-font-extrabold"></v-breadcrumbs>
    </div>



    <div class=" lg:tw-mx-8 tw-transform tw--translate-y-58 tw-bottom-0 tw-left-0 tw-px-8 tw-py-12">
      <div class="lg:tw-flex lg:tw-flex-row sm:tw-flex sm:tw-flex-col lg:tw-justify-betwen lg:tw-gap-12">

        <div class="tw-text-lg sm:tw-text-lg lg:tw-w-3/4">
          <h1 class="tw-text-black tw-text-8xl tw-font-extrabold">
            Get in <span class="text-color">touch.</span>
          </h1>
          <p class="tw-text-black tw-text-xl tw-mt-2">a passionate frontend developer focused on creating interactive,
            accessible, and responsive websites.</p>
          <div class="">
            <form
              class="tw-mt-2 tw-bg-white lg:tw-mt-0 tw-transform tw-translate-y-20 tw-shadow-2xl tw-rounded-xl tw-px-8 tw-py-16"
              v-on:submit.prevent="sendMessage">

              <div class="tw-w-full tw-md:w-1/2">
                <label class="tw-block tw-font-extrabold tw-mb-1" for="name">
                  Name
                </label>

                <input type="name" name="name" id="email" placeholder="John Doe" v-model="contact.name"
                  class="tw-block tw-bg-gray-300 tw-placeholder-gray-500 tw-w-full  tw-text-black tw-shadow-xl tw-rounded-lg tw-outline-none  tw-mb-1 tw-p-3"
                  required>
              </div>

              <div class="tw-w-full tw-md:w-1/2">
                <label class="tw-block tw-font-extrabold tw-mb-1" for="email">
                  Email Address
                </label>

                <input type="email" name="email" id="email" placeholder="email@example.com" v-model="contact.email"
                  class="tw-block  tw-bg-gray-300 tw-placeholder-gray-500 tw-w-full  tw-text-black tw-shadow-xl tw-rounded-lg tw-outline-none  tw-mb-1 tw-p-3"
                  required>
              </div>


              <div class="tw-w-full tw-md:w-1/2">
                <label class="tw-block tw-font-extrabold tw-mb-1" for="number">
                  Phone Number
                </label>

                <input type="text" name="number" id="number" placeholder="+228 91 58 50 75" v-model="contact.phone"
                  class="tw-block  tw-bg-gray-300 tw-placeholder-gray-500 tw-w-full  tw-text-black tw-shadow-xl tw-rounded-lg tw-outline-none  tw-mb-1 tw-p-3"
                  required>
              </div>


              <div class="tw-w-full tw-md:w-1/2">
                <label class="tw-block tw-font-extrabold tw-mb-1" for="text">
                  Company
                </label>

                <input type="text" name="text" id="text" placeholder="Enter your company here" v-model="contact.company"
                  class="tw-block  tw-bg-gray-300 tw-placeholder-gray-500 tw-w-full  tw-text-black tw-shadow-xl tw-rounded-lg  tw-outline-none  tw-mb-1 tw-p-3"
                  required>
              </div>

              <div class="tw-w-full tw-md:w-1/2">
                <label class="tw-block tw-font-extrabold tw-mb-1" for="text">
                  Position
                </label>

                <input type="text" name="text" id="text" placeholder="Enter your position here" v-model="contact.position"
                  class="tw-block tw-bg-gray-300 tw-placeholder-gray-500 tw-rounded-lg tw-w-full  tw-text-black tw-shadow-lg tw-outline-none  tw-mb-1 tw-p-3"
                  required>
              </div>




              <div class="tw-w-full tw-mb-8">
                <label class="tw-block tw-font-extrabold tw-mb-1" for="message">
                  Message
                </label>

                <textarea id="message" rows="3" name="message" v-model="contact.message"
                  class="tw-block  tw-bg-gray-300 tw-placeholder-gray-500 tw-w-full tw-text-black tw-p-4  tw-shadow-lg tw-rounded-lg  tw-outline-none tw-appearance-none  tw-mb-1 tw-py-3"
                  placeholder="Enter your message here." required></textarea>
              </div>

              <button
                class="tw-group bg-color tw-relative tw-h-12 tw-mt-4 tw-cursor-pointer hover:tw-transform hover:tw-translate-x-2 hover:tw-transition-transform hover:tw-duration-300 hover:tw-shadow-2xl-blue-600 hover:tw-shadow-2xl-lg tw-w-48 tw-overflow-hidden tw-rounded-lg tw-text-lg tw-shadow-2xl-2xl">
                <div
                  class="tw-absolute tw-inset-0 tw-w-full bg-color tw--transition-all tw-duration-[250ms] tw-ease-out group-hover:tw-w-full">
                </div>
                <span class="tw-relative tw-inline-flex tw-items-center tw-gap-2 tw-text-white group-hover:tw-text-white">
                  Send

                </span>
              </button>
            </form>

           
          </div>
        </div>

        <div class="lg:tw-mt-56 lg:tw-w-1/2 tw-items-center">
          <img class="tw-rounded-lg tw-shadow-2xl tw-shadow-gray-900 tw-mb-8" data-aos="fade-up" src="https://img.freepik.com/free-photo/top-view-workspace-with-notebook-succulent-plant_23-2148430820.jpg?w=740&t=st=1690220651~exp=1690221251~hmac=a7249088cdb9fbe455226feccdb5ea68d2bd60b9c7ae35f497131c6e9a06e731">

              <h1 class="tw-text-black tw-text-xl tw-mt-2">Shoot us a mail</h1>
              <p class="text-color tw-text-2xl tw-font-extrabold tw-mt-4">sergetassiga22@gmail.com</p>

              <h2 class="tw-text-black tw-text-xl tw-mt-4">
                You can always reach out by calling</h2>
              <p class="text-color tw-text-2xl tw-font-extrabold tw-mt-4">+250 785 658 174
              </p>
            </div>



      </div> <!-- end hero -->

    </div>

    <div class="tw-mt-4 tw-shadow-2xl tw-rounded-lg tw-shadow-gray-900 lg:tw-px-8 tw-pb-4 tw-aspect-w-16 tw-aspect-h-7 tw-overflow-hidden" data-aos="fade-up">

      <iframe class="tw-shadow-2xl tw-rounded-lg tw-shadow-gray-900"
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d63800.26059361784!2d30.057428788649723!3d-1.94642533671203!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x19dca5a86d814c61%3A0x7d3b83e12b1c11a9!2sNorrsken%20House%20Kigali!5e0!3m2!1sfr!2srw!4v1684802051331!5m2!1sfr!2srw"
        width="100%" height="500" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
    </div>

  </div>
</template>

<script>
import AOS from 'aos';
import 'aos/dist/aos.css';
const swal = require('sweetalert2')

export default {
  data() {
    return {
      title: 'Nous contacter Page',
      contact: {
        name: "",
        phone: "",
        email: "",
        message: "",
      },

    }
  },

  head() {
    return {
      title: 'Nous contacter Page',

    }
  },

  computed: {
    breadcrumbItems() {
      const items = [{
        text: 'Home',
        href: '/',
      },
      {
        text: 'Contact Us',

      },

      ];

      return items.map((item) => ({
        ...item,
        disabled: !item.href,
      }));
    },
  },

  mounted() {
    if (!this.initialized) {
      AOS.init({
        once: true,
        duration: 2000
      });
      this.initialized = true;
    }
  },

  methods: {


    async sendMessage(contact) {
      try {
        const response = await fetch('/api/v1/send-email', {
          method: 'POST',
          body: JSON.stringify({
            contact: {
              name: this.contact.name,
              phone: this.contact.phone,
              email: this.contact.email,
              message: this.contact.message,
            }
          }),
          headers: {
            'Content-Type': 'application/json'
          }
        });
        const data = await response.json();
        if (response.ok) {
          new swal({
            title: 'Message envoyé!',
            text: 'Votre message a été envoyé avec succès.',
            icon: 'success',
            button: 'Fermer',
          });
        }
        return data;
      } catch (error) {
        console.error('Error sending message:', error);
        new swal({
          title: 'Erreur!',
          text: 'Une erreur s\'est produite lors de l\'envoi de votre message.',
          icon: 'error',
          button: 'Fermer',
        });
      }
    }



  },
}

</script>

<style scoped>
.bg-image {
  background-image: url(https://img.freepik.com/premium-photo/african-american-practitioner-assistant-with-protective-face-mask-against-coroanvirus_482257-26733.jpg?w=740);
  background-size: cover;
  height: 100%;
  width: 100%;
}

.bg-color {
  background-color: #03989e;
}

.text-color {
  color: #03989e;
}


button {
  color: black
}
</style>
