<template>
  <div class="">

    <div class="tw-relative tw-w-full tw-h-72">
      <img class="tw-absolute tw-top-0 tw-left-0 tw-w-full tw-h-full tw-object-cover"
        src="https://img.freepik.com/free-photo/businessmen-hands-white-table-with-documents-drafts_176420-354.jpg?w=740&t=st=1693316696~exp=1693317296~hmac=4d5dd6c602e96f8eb10e33b3219c6127a96658bfde3c8c266ad17c71b9e89201"
        alt="Banner Image">
      <div
        class="tw-relative tw-w-full tw-h-full tw-flex tw-flex-col tw-justify-center tw-items-center tw-bg-gray-900 tw-bg-opacity-60">
        <h1 class="tw-text-4xl tw-font-bold tw-text-white" data-aos="fade-up">Contact Us</h1>
      </div>
    </div>
    <div class="tw-flex tw-items-center tw-space-x-2 tw-px-8">
      <v-breadcrumbs :items="breadcrumbItems" divider="/" class="tw-text-lg tw-font-extrabold"></v-breadcrumbs>
    </div>



    <div class="lg:tw-mx-8 tw-transform tw--translate-y-58 tw-bottom-0 tw-left-0 tw-px-8 tw-py-12">
      <div class="lg:tw-flex lg:tw-flex-row sm:tw-flex sm:tw-flex-col lg:tw-justify-betwen lg:tw-gap-12">

        <div class="tw-text-lg sm:tw-text-lg lg:tw-w-3/4 tw-mb-12">
          <h1 class="tw-text-black tw-text-8xl tw-font-extrabold">
            Get in <span class="text-color">touch.</span>
          </h1>
          <p class="tw-text-black tw-text-xl tw-mt-2">
            Reach out to me anytime and I will get back to you within 24 hours.
          </p>
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


              <div class="tw-w-full tw-mb-8">
                <label class="tw-block tw-font-extrabold tw-mb-1" for="message">
                  Message
                </label>

                <textarea id="message" rows="3" name="message" v-model="contact.message"
                  class="tw-block  tw-bg-gray-300 tw-placeholder-gray-500 tw-w-full tw-text-black tw-p-4  tw-shadow-lg tw-rounded-lg  tw-outline-none tw-appearance-none  tw-mb-1 tw-py-3"
                  placeholder="Enter your message here." required></textarea>
              </div>

              <button
                class="tw-group bg-color tw-shadow-lg tw-rounded-lg tw-relative tw-h-12 tw-mt-4 tw-cursor-pointer hover:tw-transform hover:tw-translate-x-2 hover:tw-transition-transform hover:tw-duration-300 hover:tw-shadow-2xl-blue-600 hover:tw-shadow-2xl-lg tw-w-48 tw-overflow-hidden tw-rounded-lg tw-text-lg tw-shadow-2xl-2xl">
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
          <img class="tw-rounded-lg tw-shadow-2xl tw-shadow-gray-300 tw-mb-8" src="https://img.freepik.com/free-photo/businessmen-hands-white-table-with-documents-drafts_176420-354.jpg?w=740&t=st=1693316696~exp=1693317296~hmac=4d5dd6c602e96f8eb10e33b3219c6127a96658bfde3c8c266ad17c71b9e89201">

             <div class="tw-shadow-2xl tw-rounded-lg tw-shadow-gray-300 tw-p-4">
              <h1 class="tw-text-black tw-font-bold tw-text-xl tw-mt-2">Shoot me a mail:</h1>
              <p class="text-color tw-text-2xl tw-font-extrabold tw-mt-4">sergetassiga22@gmail.com</p>

              <h2 class="tw-text-black tw-font-bold tw-text-xl tw-mt-4">
                You can always reach out by calling:</h2>
              <p class="text-color tw-text-2xl tw-font-extrabold tw-mt-4">+250 785 658 174
              </p>
             </div>
            </div>



      </div> <!-- end hero -->

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
  background-color: #FD8D14;
}

.text-color {
  color: #FD8D14;
}


button {
  color: black
}
</style>
