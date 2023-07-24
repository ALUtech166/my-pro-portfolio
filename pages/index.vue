<template>
  <div>
    <section class="lg:tw-mx-12">
      <div class="bg-image tw-py-24 tw-rounded-lg tw-shadow-2xl tw-shadow-gray-900 tw-h-full tw-w-full">
        <div
          class="tw-w-full tw-h-full tw-flex tw-flex-col tw-bg-black tw-bg-opacity-60 tw-p-12">
          <div class="tw-text-left tw-px-8 tw-h-full">
            <p class="tw-text-white tw-text-xl tw-mb-4">Hello, I am</p>
            <h1 class="tw-text-white tw-text-7xl tw-font-extrabold lg:tw-w-1/2">
              Serge Anan
            </h1>
            <h1 class="text-color tw-mt-4 tw-text-7xl tw-font-extrabold lg:tw-w-1/2">
             TASSIGA
            </h1>

            <p class="tw-text-white tw-text-xl lg:tw-w-1/2 tw-mt-4">a passionate frontend developer focused on creating interactive, accessible, and responsive websites.</p>



          </div>
        </div>
      </div>

      <div
        class="bg-color tw-shadow-2xl tw-rounded-lg tw-shadow-gray-800 lg:tw-mx-24 tw-mx-8 tw-transform tw--translate-y-20 tw-bottom-0 tw-left-0 tw-px-8 tw-py-12">
        <h1 class="tw-font-extrabold lg:tw-text-4xl tw-text-center tw-text-white tw-text-2xl tw-p-4">
          "Think before you toss! Unleash your creativity
          and give plastic a second life"
        </h1>
      </div>
    </section>

  </div>
</template>
<script>
import AOS from 'aos';
import 'aos/dist/aos.css';

export default {
  data() {
    return {
      initialized: false,
      posts: []
    };
  },
  mounted() {
    this.initializeAOS();

  },


  destroyed() {
    AOS.refresh(); // Manually refresh AOS when the component is destroyed
  },

  methods: {
    initializeAOS() {
      if (!this.initialized) {
        AOS.init({
          once: true,
          duration: 2000
        });
        this.initialized = true;
      }
    },

  },
  head() {
    return {
      title: 'Welcome to Sheba Plastic Platform'
    };
  }
};

</script>



<style scoped>
button {
  border: 1px solid #03989e;
  background-color: white;
}


.bg-color:hover {
  background-color: #03989e;
  color: white;
}

.bg-color {
  background-color: #03989e;
  color: white;
}

.bg-color-1 {
  background-color: #03989e;
}

.bg-image {
  background-image: url('https://img.freepik.com/free-photo/top-view-workspace-with-notebook-succulent-plant_23-2148430820.jpg?w=740&t=st=1690220651~exp=1690221251~hmac=a7249088cdb9fbe455226feccdb5ea68d2bd60b9c7ae35f497131c6e9a06e731');
  background-size: cover;
  height: 100%;
}

.bg-image-1 {
  background-image: url('../assets/omapny.png');
  background-size: cover;
  height: 100%;
}


.text-color {
  color: #03989e;
}

/* Popup */
.tw-modal {
  opacity: 0;
  visibility: hidden;
  transition: all 0.3s ease-in-out;
}

.tw-modal-overlay {
  opacity: 0;
  visibility: hidden;
  transition: all 0.3s ease-in-out;
}

.tw-modal-container {
  opacity: 0;
  visibility: hidden;
  transform: translateY(-50px);
  transition: all 0.3s ease-in-out;
}

.tw-modal .tw-modal-overlay {
  opacity: 1;
  visibility: visible;
}

.tw-modal.open {
  opacity: 1;
  visibility: visible;
}


/* Popup */
.tw-modal {
  opacity: 0;
  visibility: hidden;
  transition: all 0.3s ease-in-out;
}

.tw-modal-overlay {
  opacity: 0;
  visibility: hidden;
  transition: all 0.3s ease-in-out;
}

.tw-modal-container {
  opacity: 0;
  visibility: hidden;
  transform: translateY(-50px);
  transition: all 0.3s ease-in-out;
}

.tw-modal .tw-modal-overlay {
  opacity: 1;
  visibility: visible;
}

.tw-modal.open {
  opacity: 1;
  visibility: visible;
}

.tw-modal.open .tw-modal-container {
  transform: translateY(0);
  opacity: 1;
  visibility: visible;
}

/* Close button */
.tw-modal-close {
  cursor: pointer;
}

/* Animation */
@keyframes fadeIn {
  from {
    opacity: 0;
  }

  to {
    opacity: 1;
  }
}

.animated {
  animation-duration: 0.3s;
  animation-fill-mode: both;
}

.fadeIn {
  animation-name: fadeIn;
}
</style>
