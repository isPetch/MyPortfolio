<script setup>
import DeviconHtml5 from './components/icon/DeviconHtml5.vue'
import DeviconCss3 from './components/icon/DeviconCss3.vue'
import LogosJavascript from './components/icon/LogosJavascript.vue'
import DeviconTailwindcss from './components/icon/DeviconTailwindcss.vue'
import DeviconVuejs from './components/icon/DeviconVuejs.vue'
import DeviconLinux from './components/icon/DeviconLinux.vue'
import DeviconMysql from './components/icon/DeviconMysql.vue'
import DeviconJava from './components/icon/DeviconJava.vue'
import { ref } from 'vue';

const scrollToSection = (sectionId) => {
  const section = document.querySelector(`.${sectionId}`);
  if (section) {
    section.scrollIntoView({ behavior: 'smooth' });
  }
};


</script>
 
<script setup>
</script>
<template>
  <div class="w-screen h-screen hidden md:block">


    <div class="flex flex-col w-full h-full bg-white">

      <!-- เมนู -->
      <div class="flex flex-row w-full h-20 justify-end items-center space-x-6 drop-shadow-xl pr-6 bg-white">
        <button @click="scrollToSection('pp-home')" class=" hover:border-b-2 border-orange-400 text-black">Home</button>
        <button @click="scrollToSection('pp-about')" class=" hover:border-b-2 border-orange-400 text-black">About</button>
        <button @click="scrollToSection('pp-skills')"
          class=" hover:border-b-2 border-orange-400 text-black">Skills</button>
        <button @click="scrollToSection('pp-projects')"
          class=" hover:border-b-2 border-orange-400 text-black">Portfolio</button>
        <button @click="scrollToSection('pp-contact')"
          class=" hover:border-b-2 border-orange-400 text-black">Contact</button>
      </div>

      <!-- แนะนำ 1 -->
      <div class="pp-home flex w-full h-full justify-center items-center bg-white">
        <div class="flex flex-col w-1/2 space-y-6">
          <div class="space-y-1">
            <div class="text-black">Hi, my name is</div>
            <div class="text-5xl font-bold text-black">Phatcharaphon Saisung</div>
          </div>

          <div class="text-black">I'm a student majoring in Information Technology<br /> at King Mongkut's University of
            Technology Thonburi.</div>
        </div>
      </div>


    </div>

    <!-- About -->
    <div class="pp-about flex flex-col w-full h-full bg-white">
      <div class=" flex w-full h-full justify-center items-start pt-20">
        <div class="flex flex-row w-1/2 ">
          <div class="flex flex-col w-1/2 space-y-4">
            <div class="text-2xl font-bold text-black">About Me</div>
            <div class="text-black">I'm Phatcharaphon Saisung, a third-year student majoring in Information
              Technology at King
              Mongkut's University of Technology Thonburi. I have a strong passion for creativity, especially in web
              development.
            </div>
            <div class="text-black">My goal is to find an internship opportunity to enhance my skills and contribute to
              real-world projects.</div>
            <div class="text-black"> When I'm not in front of my computer, I enjoy reading manga and watching anime. These
              hobbies help me
              unwind and provide a different perspective on storytelling and creativity.
            </div>
          </div>

          <div class="flex w-1/2 items-center justify-center">
            <div>
              <img class="mask mask-squircle" src="./components/icon/me.png" />
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Skills -->
    <div class="pp-skills flex flex-col w-full h-2/3  bg-white pt-10">
      <div class=" flex w-full h-full justify-center items-start">
        <div class="flex flex-row w-1/2  items-center">
          <div class="text-2xl w-1/3 font-bold text-black">Skills</div>

          <div class="flex flex-col space-y-10">

            <div class="flex flex-row w-full space-x-6">
              <div class="lg:tooltip" data-tip="HTML5">
                <button class="btn h-16 bg-gray-200">
                  <DeviconHtml5 />
                </button>
              </div>
              <div class="lg:tooltip" data-tip="CSS3">
                <button class="btn h-16 bg-gray-200">
                  <DeviconCss3 />
                </button>
              </div>
              <div class="lg:tooltip" data-tip="JavaScript">
                <button class="btn h-16 bg-gray-200">
                  <LogosJavascript />
                </button>
              </div>
              <div class="lg:tooltip" data-tip="Tailwind CSS">
                <button class="btn h-16 bg-gray-200">
                  <DeviconTailwindcss />
                </button>
              </div>
            </div>

            <div class="flex flex-row w-full space-x-6">
              <div class="lg:tooltip" data-tip="Vue">
                <button class="btn h-16 bg-gray-200">
                  <DeviconVuejs />
                </button>
              </div>
              <div class="lg:tooltip" data-tip="Linux">
                <button class="btn h-16 bg-gray-200">
                  <DeviconLinux />
                </button>
              </div>
              <div class="lg:tooltip" data-tip="MySQL">
                <button class="btn h-16 bg-gray-200">
                  <DeviconMysql />
                </button>
              </div>
              <div class="lg:tooltip" data-tip="Java">
                <button class="btn h-16 bg-gray-200">
                  <DeviconJava />
                </button>
              </div>
            </div>

          </div>
        </div>
      </div>
    </div>

    <!-- Projects -->
    <div class="pp-projects flex flex-col w-full h-full bg-white ">
      <div class="flex w-full h-full justify-center items-start ">
        <div class="flex flex-col w-2/2  space-y-10 ">
          <div class="flex text-2xl font-bold text-black justify-center">My Projects</div>

          <div class="flex flex-col space-y-3 m-auto ">
            <div class="flex flex-row space-x-4">

              <div class="image-container w-80">
                <button>
                  <a href="https://intproj22.sit.kmutt.ac.th/sj3/admin/announcement" target="_blank">
                    <img src="./components/icon/sas.png" alt="SAS" class="image-fade rounded-xl" />
                  </a>
                </button>
                <div
                  class="flex image-text justify-center items-center  text-white bg-black bg-opacity-70 absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 w-full">
                  <div class="text-lg font-semibold">SIT Announcement System (SAS)</div>
                  <div class="text-sm">Current</div>
                </div>
              </div>

              <div class="image-container w-80 ">
                <button>
                  <a href="https://store-f08c7.web.app/" target="_blank">
                    <img src="./components/icon/203st.png" alt="Catch The Wrong Color Game"
                      class="image-fade rounded-xl" />
                  </a>
                </button>
                <div
                  class="flex image-text justify-center items-center  text-white bg-black bg-opacity-70 absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 w-full">
                  <div class="text-lg font-semibold">203 Store</div>
                  <div class="text-sm">April 2023</div>
                </div>
              </div>

            </div>

            <div class="image-container w-80 ">
              <button>
                <a href="https://catch-the-wrong-color.web.app/" target="_blank">
                  <img src="./components/icon/colorgame.png" alt="Catch The Wrong Color Game"
                    class="image-fade rounded-xl" />
                </a>
              </button>
              <div
                class="flex image-text justify-center items-center  text-white bg-black bg-opacity-70 absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 w-full">
                <div class="text-lg font-semibold">Catch The Wrong Color Game</div>
                <div class="text-sm">February 2023</div>
              </div>
            </div>

          </div>


        </div>
      </div>
    </div>


    <!-- Contact -->
    <div class="flex w-full h-2/3 items-end bg-white">
      <div class="pp-contact flex flex-col items-center w-full h-2/3 bg-gray-200 pt-5 space-y-16">
        <div class="text-2xl font-bold text-black ">Contact Me</div>
        <div class="flex flex-row w-2/3 ">

          <div class="flex flex-col w-1/3  items-center ">
            <div class=" w-16">
              <img src="./components/icon/github.png" />
            </div>
            <div class="mt-3 font-bold text-black">GitHub</div>
            <div class="text-black"> <a href="https://github.com/isPetch" target="_blank">github/isPetch</a></div>
          </div>

          <div class="flex flex-col w-1/3  items-center ">
            <div class=" w-16">
              <img src="./components/icon/mail.png" />
            </div>
            <div class="mt-3 font-bold text-black">Email</div>
            <div class="text-black">phatcharaphon.sais@gmail.com</div>
          </div>

          <div class="flex flex-col w-1/3  items-center ">
            <div class=" w-16">
              <img src="./components/icon/smartphone.png" />
            </div>
            <div class="mt-3 font-bold text-black">Phone</div>
            <div class="text-black">(+66) 83-783-4113</div>
          </div>

        </div>
      </div>
    </div>
  </div>


  <div class=" w-screen h-screen md:hidden">
    <div class="flex flex-col w-full h-full bg-white">

      <!-- เมนู -->
      <div class="flex flex-row w-full h-20 justify-center items-center space-x-6 drop-shadow-xl pr-6 bg-white">
        <button @click="scrollToSection('pp-homes')" class=" hover:border-b-2 border-orange-400 text-black">Home</button>
        <button @click="scrollToSection('pp-abouts')"
          class=" hover:border-b-2 border-orange-400 text-black">About</button>
        <button @click="scrollToSection('pp-skillss')"
          class=" hover:border-b-2 border-orange-400 text-black">Skills</button>
        <button @click="scrollToSection('pp-projectss')"
          class=" hover:border-b-2 border-orange-400 text-black">Portfolio</button>
        <button @click="scrollToSection('pp-contacts')"
          class=" hover:border-b-2 border-orange-400 text-black">Contact</button>
      </div>

      <!-- แนะนำ 1 -->
      <div class="pp-homes flex w-full h-full justify-center items-center bg-white">
        <div class="flex flex-col w-5/6 space-y-6">
          <div class="space-y-1">
            <div class="text-black">Hi, my name is</div>
            <div class="text-5xl font-bold text-black">Phatcharaphon Saisung</div>
          </div>

          <div class="text-black">I'm a student majoring in Information Technology at King Mongkut's University of
            Technology Thonburi.</div>
        </div>
      </div>


    </div>

    <!-- About -->
    <div class="pp-abouts flex flex-col w-full h-full bg-white">
      <div class=" flex w-full h-full justify-center items-start pt-20">
        <div class="flex flex-col w-5/6 items-center space-y-2 0">
          <div class="text-2xl font-bold text-black">About Me</div>
          <div class="flex flex-col w-full space-y-6">
            <div class="flex w-full items-center justify-center">
              <div>
                <img class="mask mask-squircle" src="./components/icon/me.png" />
              </div>
            </div>
            <div class="text-black">I'm Phatcharaphon Saisung, a third-year student majoring in Information
              Technology at King
              Mongkut's University of Technology Thonburi. I have a strong passion for creativity, especially in web
              development.
            </div>
            <div class="text-black">My goal is to find an internship opportunity to enhance my skills and contribute to
              real-world projects.</div>
            <div class="text-black"> When I'm not in front of my computer, I enjoy reading manga and watching anime. These
              hobbies help me
              unwind and provide a different perspective on storytelling and creativity.
            </div>
          </div>


        </div>
      </div>
    </div>

    <!-- Skills -->
    <div class="pp-skillss flex flex-col w-full h-full bg-white pt-10">
      <div class=" flex w-full h-full justify-center items-center">
        <div class="flex flex-col w-4/6  items-center space-y-4">
          <div class="text-2xl font-bold text-black">Skills</div>

          <div class="flex flex-col space-y-10">

            <div class="flex flex-row w-full space-x-6">
              <div class="lg:tooltip" data-tip="HTML5">
                <button class="btn h-16 bg-gray-200">
                  <DeviconHtml5 />
                </button>
              </div>
              <div class="lg:tooltip" data-tip="CSS3">
                <button class="btn h-16 bg-gray-200">
                  <DeviconCss3 />
                </button>
              </div>
              <div class="lg:tooltip" data-tip="JavaScript">
                <button class="btn h-16 bg-gray-200">
                  <LogosJavascript />
                </button>
              </div>
              <div class="lg:tooltip" data-tip="Tailwind CSS">
                <button class="btn h-16 bg-gray-200">
                  <DeviconTailwindcss />
                </button>
              </div>
            </div>

            <div class="flex flex-row w-full space-x-6">
              <div class="lg:tooltip" data-tip="Vue">
                <button class="btn h-16 bg-gray-200">
                  <DeviconVuejs />
                </button>
              </div>
              <div class="lg:tooltip" data-tip="Linux">
                <button class="btn h-16 bg-gray-200">
                  <DeviconLinux />
                </button>
              </div>
              <div class="lg:tooltip" data-tip="MySQL">
                <button class="btn h-16 bg-gray-200">
                  <DeviconMysql />
                </button>
              </div>
              <div class="lg:tooltip" data-tip="Java">
                <button class="btn h-16 bg-gray-200">
                  <DeviconJava />
                </button>
              </div>
            </div>

          </div>
        </div>
      </div>
    </div>

    <!-- Projects -->
    <div class="pp-projectss flex flex-col w-full h-full bg-white ">
      <div class="flex w-full h-full justify-center items-start ">
        <div class="flex flex-col w-2/2  space-y-4 ">
          <div class="flex text-2xl font-bold text-black justify-center">My Projects</div>

          <div class="flex flex-col space-y-3 m-auto ">


            <div class="image-container w-80">
              <button>
                <a href="https://intproj22.sit.kmutt.ac.th/sj3/admin/announcement" target="_blank">
                  <img src="./components/icon/sas.png" alt="SAS" class="image-fade rounded-xl" />
                </a>
              </button>
              <div
                class="flex image-text justify-center items-center  text-white bg-black bg-opacity-70 absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 w-full">
                <div class="text-lg font-semibold">SIT Announcement System (SAS)</div>
                <div class="text-sm">Current</div>
              </div>
            </div>

            <div class="image-container w-80 ">
              <button>
                <a href="https://store-f08c7.web.app/" target="_blank">
                  <img src="./components/icon/203st.png" alt="Catch The Wrong Color Game"
                    class="image-fade rounded-xl" />
                </a>
              </button>
              <div
                class="flex image-text justify-center items-center  text-white bg-black bg-opacity-70 absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 w-full">
                <div class="text-lg font-semibold">203 Store</div>
                <div class="text-sm">April 2023</div>
              </div>
            </div>



            <div class="image-container w-80 ">
              <button>
                <a href="https://catch-the-wrong-color.web.app/" target="_blank">
                  <img src="./components/icon/colorgame.png" alt="Catch The Wrong Color Game"
                    class="image-fade rounded-xl" />
                </a>
              </button>
              <div
                class="flex image-text justify-center items-center  text-white bg-black bg-opacity-70 absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 w-full">
                <div class="text-lg font-semibold">Catch The Wrong Color Game</div>
                <div class="text-sm">February 2023</div>
              </div>
            </div>

          </div>


        </div>
      </div>
    </div>

    <!-- Contact -->
    <div class="flex w-full h-full items-end bg-white">
      <div class="pp-contacts flex flex-col items-center w-full h-3/6 bg-gray-200 pt-5 space-y-6">
        <div class="text-2xl font-bold text-black ">Contact Me</div>
        <div class="flex flex-col w-5/6 space-y-6">

          <div class="flex flex-row items-center ">
            <div class="flex flex-col w-1/3  items-center ">
              <div class=" w-8">
                <img src="./components/icon/github.png" />
              </div>
              <div class="mt-1 font-bold text-black">GitHub</div>
            </div>
            <div class="text-black"> <a href="https://github.com/isPetch" target="_blank">github/isPetch</a></div>
          </div>


          <div class="flex flex-row items-center ">
            <div class="flex flex-col w-1/3  items-center ">
              <div class="w-8">
                <img src="./components/icon/mail.png" />
              </div>
              <div class="mt-1 font-bold text-black">Email</div>
            </div>
            <div class="text-black">phatcharaphon.sais@gmail.com</div>
          </div>

          <div class="flex flex-row items-center ">
            <div class="flex flex-col w-1/3  items-center ">
              <div class=" w-8">
                <img src="./components/icon/smartphone.png" />
              </div>
              <div class="mt-1 font-bold text-black">Phone</div>
            </div>
            <div class="text-black">(+66) 83-783-4113</div>
          </div>

        </div>
      </div>
    </div>



  </div>
</template>
<style scoped>
/* สไตล์สำหรับรูปที่ต้องการให้เปลี่ยนสีจาง */
.image-fade:hover {
  filter: grayscale(70%);
  transition: filter 0.3s ease-in-out;
}

/* สไตล์สำหรับข้อความที่จะแสดงเมื่อนำเมาส์ไปชี้ที่รูป */
.image-text {
  top: 80%;
  left: 50%;
  padding: 10px;
  display: none;
}

/* สไตล์สำหรับคอนเทนเนอร์ของรูป */
.image-container {
  position: relative;
  display: inline-block;
}

/* สไตล์สำหรับเมื่อเมาส์ชี้ที่คอนเทนเนอร์ของรูป */
.image-container:hover .image-text {
  display: block;
}
</style>