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
        <div class="tw-flex tw-items-center tw-space-x-2 tw-px-8">
            <v-breadcrumbs :items="breadcrumbItems" divider="/" class="tw-text-lg tw-font-extrabold"></v-breadcrumbs>
        </div>

        <section class="tw-p-6 tw-px-24 tw-pt-24">
            <v-row class="tw-mx-12">
                <v-col class="" cols="12" md="6" lg="6">


                    <v-img class="tw-rounded-lg tw-cursor-pointer"
                        src="https://img.freepik.com/premium-photo/empty-wooden-table-hotel-interior-product-background_148157-391.jpg?size=626&ext=jpg"
                        width="450px"></v-img>
                </v-col>

                <v-col class="" cols="12" md="6" lg="6">
                    <div class="tw-p-4" data-aos="fade-up">
                        <h1 class="tw-text-black tw-text-5xl tw-font-extrabold tw-text-justify">
                            About
                            <strong class="text-color">Me</strong>
                        </h1>

                        <p class="tw-text-md tw-text-gray-800 tw-font-medium tw-text-justify tw-pt-4 tw-mb-2">
                            Experience the forefront of education through e-tuto—an innovative platform seamlessly blending
                            dynamic Experience the forefront of education through e-tuto—an innovative platform seamlessly blending
                            dynamic Experience the forefront of education through e-tuto—an innovative platform seamlessly blending
                            dynamic Experience the forefront of education through e-tuto—an innovative platform seamlessly blending
                            dynamic 
                        </p>

                       

                    </div>
                </v-col>
               

            </v-row>

        </section>

        <section class="tw-p-6 tw-px-24 tw-pt-24">
            <div class="tw-text-center tw-items-center" data-aos="fade-up">
                <h1 class="tw-text-black tw-text-5xl tw-font-extrabold">
                    Our
                    <strong class="text-color">Works</strong>
                </h1>

                <p class="tw-text-md tw-text-gray-800 tw-font-medium tw-text-center tw-pt-4 tw-mb-2">
                    Experience the forefront of education through e-tuto—an innovative platform seamlessly blending dynamic
                </p>
            </div>
            <v-row class="tw-mx-8" data-aos="fade-up">

                <v-col class="" cols="12" md="4" lg="4">


                    <v-img class="tw-rounded-lg tw-cursor-pointer tw-rounded-lg tw-shadow-xl"
                        src="https://img.freepik.com/premium-vector/realistic-modern-black-smartphone-mockup-design-mobile-applicationvector_348082-2406.jpg?w=740"
                        width="450px"></v-img>
                </v-col>

                <v-col class="" cols="12" md="4" lg="4">


                    <v-img class="tw-rounded-lg tw-cursor-pointer tw-rounded-lg tw-shadow-xl"
                        src="https://img.freepik.com/free-vector/isometric-university-landing-page-template_52683-14464.jpg?size=626&ext=jpg"
                        width="450px"></v-img>
                </v-col>

                <v-col class="" cols="12" md="4" lg="4">


                    <v-img class="tw-rounded-lg tw-cursor-pointer tw-rounded-lg tw-shadow-xl"
                        src="https://img.freepik.com/premium-vector/social-media-network-digital-communication-concept-website-landing-page-template_348082-2153.jpg?size=626&ext=jpg"
                        width="450px"></v-img>
                </v-col>

                <v-col class="" cols="12" md="4" lg="4">


                    <v-img class="tw-rounded-lg tw-cursor-pointer tw-rounded-lg tw-shadow-xl"
                        src="https://img.freepik.com/free-vector/gradient-ui-ux-landing-page-template_23-2149053801.jpg?w=740&t=st=1693314599~exp=1693315199~hmac=8eee3494221264337224e230b564f079ee303d3a667d1c5d6d304b47994aa93b"
                        width="450px"></v-img>
                </v-col>

                <v-col class="" cols="12" md="4" lg="4">


                    <v-img class="tw-rounded-lg tw-cursor-pointer"
                        src="https://img.freepik.com/premium-photo/asian-woman-checking-bills-taxes-bank-account-balance-calculating-credit-card-expenses-family-budget-finance-concept-top-view_164138-1536.jpg?w=740"
                        width="450px"></v-img>
                </v-col>

                <v-col class="" cols="12" md="4" lg="4">


                    <v-img class="tw-rounded-lg tw-cursor-pointer tw-rounded-lg tw-shadow-xl"
                        src="https://img.freepik.com/premium-photo/web-design-text-work-desk-surrounded-with-web-development-team-devices-projects-ideas-paper-concept-team-meeting_176814-958.jpg?w=740"
                        width="450px"></v-img>
                </v-col>

            </v-row>

        </section>


    </div>
</template>

<script>
import AOS from 'aos';
import 'aos/dist/aos.css';

export default {

    mounted() {
    if (!this.initialized) {
      AOS.init({
        once: true,
        duration: 2000
      });
      this.initialized = true;
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
