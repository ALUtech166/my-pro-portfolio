<template>
  <div>
    <div class="tw-relative tw-w-full tw-h-72">
      <img class="tw-absolute tw-top-0 tw-left-0 tw-w-full tw-h-full tw-object-cover"
        src="https://img.freepik.com/free-photo/businessmen-hands-white-table-with-documents-drafts_176420-354.jpg?w=740&t=st=1693316696~exp=1693317296~hmac=4d5dd6c602e96f8eb10e33b3219c6127a96658bfde3c8c266ad17c71b9e89201"
        alt="Banner Image">
      <div
        class="tw-relative tw-w-full tw-h-full tw-flex tw-flex-col tw-justify-center tw-items-center tw-bg-gray-900 tw-bg-opacity-60">
        <h1 class="tw-text-4xl tw-font-bold tw-text-white" data-aos="fade-up">About Me</h1>
      </div>
    </div>

    <v-card-actions class="tw-mx-6">
      <nuxt-link to="/"
        class="tw-group tw-relative tw-font-extrabold xl:tw-px-6 tw-px-4 tw-py-2 xl:tw-py-3 tw-rounded-lg tw-shadow-2xl tw-h-12 tw-mt-4 tw-cursor-pointer hover:tw-transform hover:tw-translate-x-2 hover:tw-transition-transform hover:tw-duration-300 hover:tw-shadow-yellow-600 tw-border hover:tw-shadow-lg tw-overflow-hidden tw-rounded-lg tw-bg-white tw-text-lg tw-shadow-2xl">
        <div
          class="tw-absolute tw-items-center tw-inset-0 tw-w-5 tw-bg-yellow-600 tw--transition-all tw-duration-[250ms] tw-ease-out group-hover:tw-w-full">
        </div>

        <span class="tw-relative tw-inline-flex tw-items-center tw-gap-2 tw-text-black group-hover:tw-text-white">
          <svg class="tw-w-5 tw-h-5 tw--transition-all tw-duration-[250ms] tw-ease-out" xmlns="http://www.w3.org/2000/svg"
            width="24" height="24" viewBox="0 0 24 24">
            <path
              d="M20 11H7.414l5.293-5.293a1 1 0 1 0-1.414-1.414l-7 7a.997.997 0 0 0-.001 1.414l7 7a1 1 0 0 0 1.414-1.414L7.414 13H20a1 1 0 0 0 0-2z" />
          </svg>
          Back Home
        </span>


      </nuxt-link>
    </v-card-actions>

    <section class="tw-p-6 tw-px-24 tw-pt-24">
      <v-row class="tw-mx-12">
        <v-col class="" cols="12" md="6" lg="6">


          <img class="tw-rounded-lg tw-cursor-pointer" width="650px" src="../assets/Serge.png" alt="">

        </v-col>

        <v-col class="" cols="12" md="6" lg="6">
          <div class="tw-p-4" data-aos="fade-up">
            <h1 class="tw-text-black tw-text-5xl tw-font-extrabold tw-text-justify">
              About
              <strong class="text-color">Me</strong>
            </h1>

            <p class="tw-text-md tw-text-gray-800 tw-font-medium tw-text-justify tw-pt-4 tw-mb-2">
              Hello, I'm Serge Tassiga, a proficient Frontend Developer originally hailing from Togo and currently based
              in the vibrant city of Kigali, Rwanda. With a wealth of experience in crafting visually captivating and
              user-centric web applications, my skill set encompasses mastery of HTML, CSS, JavaScript, NuxtJs,
              TailwindCSS, and Vuetify. This proficiency empowers me to engineer websites that effortlessly adapt to
              diverse screen dimensions.
              <br> <br>
              My passion is rooted in the art of composing elegant and high-performing code, continuously keeping pace
              with the ever-evolving landscape of web development. In my present role, I orchestrate a diverse portfolio
              of projects, ranging from streamlined landing pages to intricate e-commerce platforms.
              <br> <br>
              I place a premium on collaboration and teamwork, actively engaging with fellow developers and designers to
              transform concepts into reality. My unwavering commitment to excellence drives me to deliver cutting-edge
              digital solutions that resonate with both users and stakeholders alike.
            </p>





          </div>
        </v-col>


      </v-row>

    </section>
    <section class="tw-p-6 tw-px-24 tw-pt-24">
    <v-row class="tw-mx-12">
      <v-col class="" cols="12" md="6" lg="6">
          <div class="tw-p-4 tw-pt-16" data-aos="fade-up">
            <h1 class="tw-text-black tw-text-5xl tw-font-extrabold tw-text-justify">
              My <br>
              <strong class="text-color">Skills</strong>
            </h1>

            <p class="tw-text-md tw-text-gray-800 tw-font-medium tw-text-justify tw-pt-4 tw-mb-2 lg:tw-w-3/4">
              Dive into the versatile realm of coding languages, from front-end web development with HTML, CSS, and
            </p>

            <button @click="$router.push('/contact')"
              class="tw-group bg-hover tw-shadow-lg tw-rounded-lg tw-relative tw-h-12 tw-mt-2 tw-cursor-pointer hover:tw-transform hover:tw-translate-x-2 hover:tw-transition-transform hover:tw-duration-300 tw-shadow-yellow-600 hover:tw-shadow-2xl tw-w-48 tw-overflow-hidden tw-rounded-lg tw-text-lg tw-shadow-2xl">
              <div
                class="tw-absolute tw-inset-0 tw-w-full bg-color tw--transition-all tw-duration-[250ms] tw-ease-out group-hover:tw-w-full">
              </div>
              <span class="tw-relative tw-inline-flex tw-items-center tw-gap-2 tw-text-white group-hover:tw-text-white">
                Hire Me

              </span>
            </button>

          </div>
        </v-col>
      <v-col class="" cols="12" md="6" lg="6">

        <Skills></Skills>
      </v-col>
    </v-row>

    </section>



    <!-- 
    <section class="tw-p-6 tw-px-24 tw-pt-24 tw-text-center tw-items-center">
      <div class="tw-text-center tw-items-center" data-aos="fade-up">
        <h1 class="tw-text-black tw-text-5xl tw-font-extrabold">
          My
          <strong class="text-color">Works</strong>
        </h1>

        <p class="tw-text-black tw-text-md lg:tw-mx-32 tw-mb-8">
          Explore a selection of our latest endeavors and discover the innovative solutions we've crafted for our clients.
          These projects showcase our expertise in frontend development, data science, and our commitment to delivering
          excellence.
        </p>
      </div>
      <portfolio></portfolio>
    </section>
 -->
  </div>
</template>

<script>
import AOS from 'aos';
import 'aos/dist/aos.css';
import Skills from '../components/Skills.vue';

export default {
  data() {
    return {
      initialized: false,
      showHoverText: false,
      showHoverText2: false,
      showHoverText3: false,
      showHoverText4: false,
      showHoverText5: false,
      showHoverText6: false,
      posts: []
    };
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
  components: { Skills }
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
