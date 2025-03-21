<script setup>
import { ref } from "vue";

const selectedImage = ref(null);

const openModal = (image) => {
  selectedImage.value = image;
};
</script>

<script>
// import { ref } from "vue";

// const selectedImage = ref(null);

// const openModal = (image) => {
//   selectedImage.value = image;
// };

export default {
  data() {
    return {
      activeTab: 1,
      tech: [
        // {
        //   id: 1,
        //   name: 'HTML',
        //   imageUrl: 'https://cdn-icons-png.flaticon.com/512/1051/1051277.png',
        //   status: 'Advanced'
        // },
        {
          id: 1,
          name: 'MS Office',
          imageUrl: 'https://cdn-icons-png.flaticon.com/128/179/179331.png',
          status: 'Advanced'
        },
        {
          id: 2,
          name: 'Canva',
          imageUrl: 'https://img.icons8.com/?size=100&id=EZQdGLNeo7JI&format=png&color=000000',
          status: 'Advanced'
        },
        {
          id: 3,
          name: 'Figma',
          imageUrl: 'https://cdn-icons-png.flaticon.com/128/5968/5968705.png',
          status: 'Advance'
        },
        {
          id: 4,
          name: 'Adobe Premiere',
          imageUrl: 'https://cdn-icons-png.flaticon.com/128/5968/5968525.png',
          status: 'Advance'
        },
        {
          id: 5,
          name: 'iNews',
          imageUrl: 'https://logodix.com/logo/1946988.png',
          status: 'Advance'
        },
        // {
        //   id: 6,
        //   name: 'Looker Studio',
        //   imageUrl: 'https://img.icons8.com/?size=48&id=SruJhzn0nnLl&format=png',
        //   status: 'Advance'
        // },
        // {
        //   id: 7,
        //   name: 'SQL',
        //   imageUrl: 'https://cdn-icons-png.flaticon.com/128/2772/2772128.png',
        //   status: 'Intermediate'
        // },
        // {
        //   id: 8,
        //   name: 'HTML',
        //   imageUrl: 'https://cdn-icons-png.flaticon.com/128/1051/1051277.png',
        //   status: 'Beginner'
        // },
        // {
        //   id: 9,
        //   name: 'C/C++',
        //   imageUrl: 'https://cdn-icons-png.flaticon.com/128/6132/6132222.png',
        //   status: 'Beginner'
        // },
        // {
        //   id: 10,
        //   name: 'Java',
        //   imageUrl: 'https://cdn-icons-png.flaticon.com/128/5968/5968282.png',
        //   status: 'Beginner'
        // },
        // {
        //   id: 11,
        //   name: 'CSS',
        //   imageUrl: 'https://cdn-icons-png.flaticon.com/128/732/732190.png',
        //   status: 'Beginner'
        // },
        // {
        //   id: 12,
        //   name: 'Power BI',
        //   imageUrl: 'https://img.icons8.com/?size=64&id=70667&format=png',
        //   status: 'Intermediate'
        // }
      ],
      tools: [
        {
          id: 1,
          name: 'Content Writing',
          imageUrl: 'https://cdn-icons-png.flaticon.com/128/9079/9079294.png',
          status: 'Machine Learning'
        },
        {
          id: 2,
          name: 'SMM',
          imageUrl: 'https://cdn-icons-png.flaticon.com/128/4187/4187336.png',
          status: 'Data Manipulation'
        },
        {
          id: 3,
          name: 'News Production',
          imageUrl: 'https://cdn-icons-png.flaticon.com/128/2965/2965879.png',
          status: 'Data Manipulation'
        },
        {
          id: 4,
          name: 'TV Broadcasting',
          imageUrl: 'https://cdn-icons-png.flaticon.com/128/550/550486.png',
          status: 'Data Visualization'
        },
        {
          id: 5,
          name: 'A/V Production',
          imageUrl: 'https://cdn-icons-png.flaticon.com/128/1644/1644133.png',
          status: 'Data Visualization'
        },
        // {
        //   id: 6,
        //   name: 'tidyverse',
        //   imageUrl: 'https://tidyverse.tidyverse.org/logo.png',
        //   status: 'Data Manipulation'
        // },
        // {
        //   id: 7,
        //   name: 'ggplot2',
        //   imageUrl: 'https://ggplot2.tidyverse.org/logo.png',
        //   status: 'Data Visualization'
        // },
        // {
        //   id: 8,
        //   name: 'plotly',
        //   imageUrl: 'https://avatars.githubusercontent.com/u/5997976?s=280&v=4',
        //   status: 'Data Visualization'
        // },
        // {
        //   id: 9,
        //   name: 'lubridate',
        //   imageUrl: 'https://rstudio.github.io/cheatsheets/html/images/logo-lubridate.png',
        //   status: 'Data Manipulation'
        // },
        // {
        //   id: 10,
        //   name: 'mlr3',
        //   imageUrl: 'https://mlr3.mlr-org.com/logo.svg',
        //   status: 'Machine Learning'
        // },
        // {
        //   id: 11,
        //   name: 'tensorflow',
        //   imageUrl: 'https://img.icons8.com/?size=48&id=n3QRpDA7KZ7P&format=png',
        //   status: 'Machine Learning'
        // },
        // {
        //   id: 12,
        //   name: 'keras',
        //   imageUrl: 'https://icon.icepanel.io/Technology/svg/Keras.svg',
        //   status: 'Machine Learning'
        // },
        // {
        //   id: 13,
        //   name: 'Streamlit',
        //   imageUrl: 'https://img.icons8.com/?size=48&id=Rffi8qeb2fK5&format=png',
        //   status: 'App Framework'
        // },
        // {
        //   id: 14,
        //   name: 'Shiny',
        //   imageUrl: 'https://upload.wikimedia.org/wikipedia/commons/thumb/b/bf/Shiny_hex_logo.svg/1200px-Shiny_hex_logo.svg.png',
        //   status: 'Web Visualization'
        // },
        // {
        //   id: 15,
        //   name: 'PyTorch',
        //   imageUrl: 'https://icon.icepanel.io/Technology/svg/PyTorch.svg',
        //   status: 'Machine Learning'
        // },
        // {
        //   id: 16,
        //   name: 'SciPy',
        //   imageUrl: 'https://scipy.org/images/logo.svg',
        //   status: 'Scientific Computing'
        // },
      ],
      certificates: [
        {
          id: 1,
          title: 'Data Science',
          desc : 'at Alogritma Data Science School',
          date: '2022-12-12',
          image: 'https://ik.imagekit.io/fcuinpkmj/Screenshot%202025-02-22%20014139.png?updatedAt=1740163346916',
          slug: 'certificate-1',
          demo: 'https://ik.imagekit.io/fcuinpkmj/TeamalgoData.pdf?updatedAt=1740214069993',
        },
        {
          id: 2,
          title: 'Business Intelligence',
          desc : 'at Alogritma Data Science School',
          date: '2023-06-27',
          image: 'https://ik.imagekit.io/fcuinpkmj/TeamAlgoBI_page-0001.jpg?updatedAt=1740216257504',
          slug: 'certificate-2',
          demo: 'https://ik.imagekit.io/fcuinpkmj/TeamAlgoBI.pdf?updatedAt=1740214101230',
        },
        {
          id: 3,
          title: 'Authors',
          desc : 'at ICICoS 2024',
          date: '2024-07-18',
          image: 'https://ik.imagekit.io/fcuinpkmj/icicos2024-certificate_page-0001.jpg?updatedAt=1740216485827',
          slug: 'certificate-3',
          demo: 'https://ik.imagekit.io/fcuinpkmj/icicos2024-certificate_page-0001.jpg?updatedAt=1740216485827',
        },
        {
          id: 4,
          title: 'Authors',
          desc : 'at ICCSCI 2023',
          date: '2023-08-03',
          image: 'https://ik.imagekit.io/fcuinpkmj/Authors%2051-76-4_page-0001.jpg?updatedAt=1740216535806',
          slug: 'certificate-4',
          demo: 'https://ik.imagekit.io/fcuinpkmj/ICCSCI.pdf?updatedAt=1740216573277',
        },
      ]
    };
  }
}
</script>

<template>
  <div
    class="bg-[#06402B] px-5 py-5 md:px-12 md:py-10 text-left border border-[#383838] rounded-3xl text-amber-50 mx-3 mb-5">
    <article data-page="about">

      <header>
        <div class="text-2xl font-bold text-white mb-5 fadein-bot title-section flex items-center">
          About Winona &nbsp;
          <div class="h-[1px] w-32 bg-[#96D9C0] md:w-96 aos-init aos-animate" data-aos="zoom-in-left"
            data-aos-duration="600"></div>
        </div>
      </header>

      <section
        class="text-sm md:text-lg text-justify flex flex-col gap-4 md:flex-row md:gap-8 md:justify-left md:items-center">
        <div class="flex justify-center">
          <img class="w-60 h-60 md:w-[300px] md:h-[320px] rounded-full mb-3 fadein-up" src="/img/profile.jpg" alt="Foto">
        </div>
        <div class="md:w-7/12">
          <p class="mb-3 md:mb-7 fadein-left fadeins-1">
            &nbsp; &nbsp; &nbsp; As a 23-year-old Journalism graduate, I tell stories—whether through news scripts, social media content, or feature articles. From producing regional news at Liputan 6 SCTV to managing digital content, I’ve learned that great storytelling isn’t just about words; it’s about creating connection. In the newsroom, I thrived in fast-paced production, ensuring news was delivered clearly and impactfully to the audience.

          </p>
          <p class="mb-3 fadein-left fadeins-2">
            &nbsp; &nbsp; &nbsp; On the digital side, I craft engagement strategies that turn casual scrollers into loyal followers. With a blend of journalistic precision and creative marketing, I shape content that informs, inspires, and sparks conversations—because every story deserves to be remembered.</p>
        </div>
      </section>
    </article>
  </div>

  <div class="px-5 py-5 md:px-12 md:py-10 text-left text-black mx-3">
    <article data-page="about">
      <header>
        <div class="text-2xl font-bold text-black mb-5 fadein-bot title-section flex items-center">
          <div class="h-[1px] w-10 bg-black md:w-20 aos-init aos-animate" data-aos="zoom-in-left"
            data-aos-duration="600"></div>
          &nbsp; Skills
        </div>
      </header>
      <section>
        <div>
          <ul class="flex flex-wrap text-sm font-medium text-center text-gray-500 dark:text-white-400 mb-5">
            <li class="mr-2">
              <button class="inline-block px-4 py-3 rounded-lg hover:text-[#E3FFF5]"
                :class="{ 'text-[#06402B] bg-[#06402B] bg-opacity-10': activeTab === 1 }" @click="activeTab = 1">Tech Stack</button>
            </li>
            <li class="mr-2">
              <button class="inline-block px-4 py-3 rounded-lg hover:text-[#E3FFF5]"
                :class="{ 'text-[#06402B] bg-[#06402B] bg-opacity-10': activeTab === 2 }" @click="activeTab = 2">Soft Skill</button>
            </li>
            <li class="mr-2">
              <button class="inline-block px-4 py-3 rounded-lg hover:text-[#E3FFF5]"
                :class="{ 'text-[#06402B] bg-[#06402B] bg-opacity-10': activeTab === 3 }" @click="activeTab = 3">Publication</button>
            </li>
          </ul>
        </div>

        <!-- Tech Stack Tab -->
        <div v-show="activeTab === 1">
          <div class="grid grid-cols-2 gap-4 pb-32 md:grid-cols-3 md:gap-8 xl:grid-cols-4 xl:gap-10 2xl:gap-12">
            <div v-for="item in tech" :key="item.id">
              <div class="item-tech flex cursor-pointer items-center gap-2 rounded border border-[#06402B] px-2 py-2 hover:bg-[#06402B] hover:bg-opacity-10 md:gap-3 lg:px-3">
                <div class="flex h-12 w-12 items-center justify-center p-0 lg:h-16 lg:w-16 lg:p-2 zoom-in">
                  <img alt="HTML" loading="lazy" width="32" height="32" decoding="async" data-nimg="1"
                    class="img-tech drop-shadow-xl transition-all duration-300 h-[65%] w-[65%] lg:h-[85%] lg:w-[85%]" :src="item.imageUrl" style="color: transparent;">
                </div>
                <div class="flex items-center text-sm md:text-base lg:text-lg">
                  <div class="tech font-medium text-secondary transition-all duration-300 translate-y-0">{{ item.name }}</div>
                  <div class="status-tech opacity-0 absolute mt-5 text-[10px] text-[#06402B] transition-all duration-300 md:text-xs lg:text-sm">
                    {{ item.status }}
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>

        <!-- Library Tab -->
        <div v-show="activeTab === 2">
          <div class="grid grid-cols-2 gap-4 pb-32 md:grid-cols-3 md:gap-8 xl:grid-cols-4 xl:gap-10 2xl:gap-12">
            <div v-for="item in tools" :key="item.id">
              <div class="item-tech flex cursor-pointer items-center gap-2 rounded border border-[#06402B] px-2 py-2 hover:bg-[#06402B] hover:bg-opacity-10 md:gap-3 lg:px-3">
                <div class="flex h-12 w-12 items-center justify-center p-0 lg:h-16 lg:w-16 lg:p-2 zoom-in">
                  <img alt="HTML" loading="lazy" width="32" height="32" decoding="async" data-nimg="1"
                    class="img-tech drop-shadow-xl transition-all duration-300 h-[65%] w-[65%] lg:h-[85%] lg:w-[85%]" :src="item.imageUrl" style="color: transparent;">
                </div>
                <div class="flex items-center text-sm md:text-base lg:text-lg">
                  <div class="tech font-medium text-secondary transition-all duration-300 translate-y-0">{{ item.name }}</div>
                  <div class="status-tech opacity-0 absolute mt-5 text-[10px] text-[#06402B] transition-all duration-300 md:text-xs lg:text-sm">
                    {{ item.status }}
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>

        <!-- Certificates Tab -->
        <!-- <div v-show="activeTab === 3">
          <div class="container mx-auto p-3 md:p-8">
            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-4">
              <router-link v-for="cert in certificates" :key="cert.id" :to="`/certificate/${cert.slug}/${cert.id}`" class="block">
                <article class="bg-[#1e1e1f] border-[#383838] rounded-xl p-5 md:py-7 md:px-8 text-white hover:bg-[#282828] cursor-pointer relative group">
                  <div class="flex justify-center items-center">
                    <div class="w-64 h-48 flex items-center justify-center">
                      <img :src="cert.image" class="rounded-lg md:rounded-xl w-full h-full object-cover" alt="Certificate Image">
                    </div>
                  </div>
                  <div class="mt-4 text-center">
                    <h1 class="text-sm md:text-md text-amber-200 font-bold mb-2">{{ cert.title }}</h1>
                    <div class="text-xs text-slate-400 italic">{{ cert.date }}</div>
                  </div>
                  <div class="absolute bottom-4 left-1/2 transform -translate-x-1/2 opacity-0 group-hover:opacity-100 transition-opacity duration-300">
                    <a href="javascript:void(0)" class="px-4 py-2 text-sm bg-amber-200 text-white rounded-lg hover:bg-amber-300">
                      View Certificate
                    </a>
                  </div> -->
                  <!-- Tautan Demo -->
                  <!-- <div class="absolute bottom-4 right-4 opacity-0 group-hover:opacity-100 transition-opacity duration-300">
                    <a v-if="cert.demo" :href="cert.demo" target="_blank" rel="noreferrer" title="View certificate" class="transition-all hover:text-accent">
                      <svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" height="18" width="18" xmlns="http://www.w3.org/2000/svg">
                        <path d="M18 13v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h6"></path>
                        <polyline points="15 3 21 3 21 9"></polyline>
                        <line x1="10" y1="14" x2="21" y2="3"></line>
                      </svg>
                    </a>
                  </div>
                </article>
              </router-link>
            </div>
          </div>
        </div> -->

        <div v-if="activeTab === 3" class="certificate-section">
          <h2 class="text-2xl font-bold text-white mb-6">Certificates</h2>
          <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
            <div 
              v-for="cert in certificates" 
              :key="cert.id" 
              class="relative flex flex-col items-center gap-1 rounded-xl bg-[#1e1e1f] hover:bg-[#282828] border border-[#383838] p-5 md:py-7 md:px-8 transition duration-300 cursor-pointer"
              @click="openModal(cert.image)"
            >
              <img :src="cert.image" :alt="cert.title" class="w-full h-48 object-cover rounded-md" />
              <h3 class="text-lg font-semibold text-white mt-2">{{ cert.title }}</h3>
              <p class="text-[#b2b2b2] text-sm">{{ cert.desc }}</p>
              <p class="text-[#e1c265] text-sm">{{ cert.date }}</p>
              
              <!-- Icon View Certificate -->
              <a 
                :href="cert.demo" 
                target="_blank" 
                class="absolute bottom-4 right-4 text-gray-300 hover:text-[#FFD700] transition duration-300"
                @click.stop
              >
                <svg stroke="currentColor"
                  fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round"
                  height="18" width="18" xmlns="http://www.w3.org/2000/svg">
                  <path d="M18 13v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h6"></path>
                  <polyline points="15 3 21 3 21 9"></polyline>
                  <line x1="10" y1="14" x2="21" y2="3"></line>
                </svg>
              </a>
            </div>
          </div>

          <!-- Modal -->
          <div v-if="selectedImage" class="fixed inset-0 bg-black bg-opacity-80 flex items-center justify-center z-50" @click="selectedImage = null">
            <div class="relative bg-[#1e1e1f] p-6 md:p-8 rounded-xl w-[90vw] max-w-5xl max-h-[90vh] overflow-hidden flex flex-col items-center" @click.stop>
              <!-- <button class="absolute top-2 right-2 text-[#FFD700] text-2xl" @click="selectedImage = null">&times;</button> -->
              <button 
                @click="selectedImage = null" 
                class="absolute top-4 right-4 bg-black bg-opacity-60 text-white rounded-full p-2 transition duration-300 hover:bg-opacity-80 hover:scale-110"
              >
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" class="w-6 h-6">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
                </svg>
              </button>
              <img :src="selectedImage" class="w-full rounded-lg" />
            </div>
          </div>
        </div>


        
      </section>
    </article>
  </div>
</template>

<style>
.fadein-left {
  opacity: 0;
  animation: fadeInLeft 0.5s ease-out forwards;
}

@keyframes fadeInLeft {
  0% {
    opacity: 0;
    transform: translateX(100%);
  }

  100% {
    opacity: 1;
    transform: translateX(0);
  }
}

.fadeins-1 {
  animation-delay: 500ms;
}

.fadeins-2 {
  animation-delay: 800ms;
}

.img-tech,
.tech {
  transition: transform 0.3s ease;
}

.item-tech:hover .img-tech {
  transform: scale(1.3);
}

.item-tech:hover .tech {
  transform: translateY(-12px);
}

.item-tech:hover .status-tech {
  opacity: 1;
}
</style>
