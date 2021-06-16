<template>
  <!-- nav -->
  <div class="py-6 px-4 relative">
    <div class="container mx-auto flex items-center justify-between">
      <div class="text-2xl font-bold uppercase text-primary">Mentor</div>
      <button @click="showMenu = !showMenu" class="sm:hidden">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-6 w-6"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M4 6h16M4 12h16M4 18h16"
          />
        </svg>
      </button>
      <div
        class="
          bg-white
          absolute
          top-16
          left-0
          w-full
          h-auto
          sm:w-auto
          sm:bg-none
          sm:flex
          sm:static
          sm:top-auto
          sm:left-auto
          sm:items-center
          px-2
          py-4
        "
        :class="showMenu ? 'block' : 'hidden'"
      >
        <div class="sm:space-x-4">
          <a href="#" class="text-primary font-bold block sm:inline py-2 px-2">
            Home
          </a>
          <a
            v-for="i in 5"
            :key="i"
            href="#"
            class="hover:text-primary font-bold block sm:inline py-2 px-2"
          >
            Link {{ i }}
          </a>
        </div>
        <a
          href="#"
          class="
            mt-5
            sm:mt-0
            sm:ml-10
            rounded-full
            bg-primary
            text-white
            font-bold
            px-4
            py-2
            hover:bg-opacity-80
            transition
            duration-300
            block
            text-center
          "
        >
          Get Started
        </a>
      </div>
    </div>
  </div>
  <!-- ./nav -->

  <!--     
    style="
      background-image: url(https://bootstrapmade.com/demo/templates/Mentor/assets/img/hero-bg.jpg);
    "
   -->
  <!--  hero section -->
  <div
    style="
      background-image: url(https://bootstrapmade.com/demo/templates/Mentor/assets/img/hero-bg.jpg);
    "
    class="sm:h-[calc(100vh-300px)] bg-cover bg-no-repeat"
  >
    <div
      class="
        container
        mx-auto
        flex
        items-center
        justify-between
        py-10
        sm:py-20
        space-x-10
        h-full
        px-4
        sm:px-0
      "
    >
      <div class="w-full sm:w-6/12">
        <h1
          class="text-4xl sm:text-5xl font-black leading-tight text-white mb-5"
        >
          Learning Today,<br />
          Leading Tomorrow
        </h1>
        <p class="text-2xl font-light leading-tight mb-12 block text-white">
          We are team of talented designers making websites with Bootstrap
        </p>
        <a
          href="#"
          class="
            rounded-full
            border border-white
            font-bold
            text-white
            px-6
            py-3
            text-xl
            transition
            duration-300
            hover:bg-primary
            hover:text-white
            hover:border-primary
          "
        >
          Get Started
        </a>
      </div>
    </div>
  </div>
  <!-- ./hero -->

  <!-- about -->
  <div class="bg-white py-5 sm:py-10 px-4 sm:px-0">
    <div
      class="flex flex-col sm:flex-row container items-start mx-auto gap-x-6"
    >
      <div class="w-full sm:w-7/12">
        <h2 class="text-3xl text-primary font-bold mb-4">Why Us?</h2>
        <p class="mb-5 text-lg">
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. Neque sed
          delectus explicabo. Voluptatum nostrum voluptate eaque adipisci
          temporibus, voluptatibus dolorum voluptas eos sequi quo. Quos nulla
          cupiditate molestiae deserunt ipsam.
        </p>
        <ul>
          <li
            v-for="i in 5"
            :key="i"
            class="flex items-center w-full gap-x-4 mb-3 font-medium"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-6 w-6 text-primary"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M9 12l2 2 4-4M7.835 4.697a3.42 3.42 0 001.946-.806 3.42 3.42 0 014.438 0 3.42 3.42 0 001.946.806 3.42 3.42 0 013.138 3.138 3.42 3.42 0 00.806 1.946 3.42 3.42 0 010 4.438 3.42 3.42 0 00-.806 1.946 3.42 3.42 0 01-3.138 3.138 3.42 3.42 0 00-1.946.806 3.42 3.42 0 01-4.438 0 3.42 3.42 0 00-1.946-.806 3.42 3.42 0 01-3.138-3.138 3.42 3.42 0 00-.806-1.946 3.42 3.42 0 010-4.438 3.42 3.42 0 00.806-1.946 3.42 3.42 0 013.138-3.138z"
              />
            </svg>

            Lorem ipsum, dolor sit amet consectetur adipisicing elit
          </li>
        </ul>
      </div>
      <div class="w-full sm:w-5/12">
        <img
          class="rounded"
          alt=""
          src="https://bootstrapmade.com/demo/templates/Mentor/assets/img/about.jpg"
        />
      </div>
    </div>
  </div>

  <!-- ./about -->

  <!-- counter -->
  <div class="bg-primary bg-opacity-5 py-14">
    <div class="container mx-auto">
      <div class="grid grid-cols-1 sm:grid-cols-4 gap-y-5 sm:gap-y-0">
        <div v-for="i in 4" :key="i" class="text-center">
          <h3 class="text-primary text-5xl font-black mb-3">1234</h3>
          <h4 class="font-semibold text-xl">Students</h4>
        </div>
      </div>
    </div>
  </div>
  <!-- ./counter -->

  <!-- contact -->
  <!-- ./contact -->

  <!-- footer -->
  <div class="bg-gray-50 py-10 px-6 sm:px-0">
    <div
      class="
        container
        mx-auto
        gap-y-5
        sm:gap-y-0
        grid grid-cols-1
        sm:grid-cols-4
      "
    >
      <div class="font-black text-2xl text-primary">Mentor</div>
      <div>
        <div class="font-bold mb-4">Useful Links</div>
        <ul>
          <li v-for="i in 4" :key="i" class="mb-2">
            <a href="#" class="text-gray-500 hover:text-primary block">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class="h-4 w-4 inline"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M9 5l7 7-7 7"
                />
              </svg>
              Link
            </a>
          </li>
        </ul>
      </div>
      <div>
        <div class="font-bold mb-4">Our Services</div>
        <ul>
          <li v-for="i in 4" :key="i" class="mb-2">
            <a href="#" class="text-gray-500 hover:text-primary block">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class="h-4 w-4 inline"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M9 5l7 7-7 7"
                />
              </svg>
              Link
            </a>
          </li>
        </ul>
      </div>
      <div>
        <div class="font-bold mb-4">Join Our Newsletter</div>
        <div class="mb-4 text-gray-500">
          Lorem ipsum dolor sit amet consectetur adipisicing elit
        </div>
        <div class="flex">
          <input
            type="text"
            class="
              px-4
              py-2
              rounded-full
              mr-2
              border
              focus:outline-none
              focus:ring focus:ring-primary
              transition
              duration-300
            "
          />
          <button
            type="button"
            class="
              bg-primary
              rounded-full
              text-white
              font-bold
              px-4
              py-2
              focus:outline-none
              active:bg-opacity-70
            "
          >
            Subscribe
          </button>
        </div>
      </div>
    </div>
  </div>

  <!-- ./footer -->
</template>

<script setup>
import { ref } from "vue";

const showMenu = ref(false);
</script>

<style>
</style>
