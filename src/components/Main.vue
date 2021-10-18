<script setup>
import { ref } from "vue";

defineProps({
  msg: String,
});

const count = ref(0);
</script>

<template>
  <div class="navbar mb-2 shadow-lg bg-base text-neutral">
    <div class="container mx-auto">
      <div class="flex-none px-2 mx-2">
        <img
          src="https://www.openteknik.com/themes/default/images/logo.png?v1=&ossn_cache=684a5094"
        />
      </div>
      <div class="flex-1 px-2 mx-2">
        <div class="items-stretch hidden lg:flex">
          <a class="btn btn-ghost btn-sm rounded-btn"> Home </a>
          <a class="btn btn-ghost btn-sm rounded-btn"> Portfolio </a>
          <a class="btn btn-ghost btn-sm rounded-btn"> About </a>
          <a class="btn btn-ghost btn-sm rounded-btn"> Contact </a>
        </div>
      </div>
      <div class="flex-none">
        <button class="btn btn-square btn-ghost">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            class="inline-block w-6 h-6 stroke-current"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z"
            ></path>
          </svg>
        </button>
      </div>
      <div class="flex-none">
        <button class="btn btn-square btn-ghost">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            class="inline-block w-6 h-6 stroke-current"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"
            ></path>
          </svg>
        </button>
      </div>
    </div>
  </div>
  <div class="py-6 mt-20 text-neutral">
    <div class="container flex mx-auto">
      <div class="grid grid-cols-2 gap-10">
        <div>
          <img
            class="bg-neutral py-3 mb-5 rounded"
            src="https://www.opensource-socialnetwork.org/themes/default/images/logo.png?ossn_cache=d845fcae"
          />
          <h1
            class="
              text-2xl
              sm:text-5xl
              leading-none
              font-extrabold
              tracking-tight
              mb-3
              sm:mb-10
            "
          >
            Join over
            <span class="text-info">{{ msg }}</span> others in saying "NO" to
            big data.
          </h1>
          <p class="text-lg font-medium space-y-6 mb-6">
            Open Source Social Network gives you the power of social networking
            without the compromise of data collection and sales. We give users
            the power to host their own solutions and tailor the experience to
            fit their needs.
          </p>
        </div>
        <div>
          <div class="mockup-window bg-base-300 shadow-xl">
            <div class="flex justify-center px-4 py-16 bg-base-200">
              <img src="../assets/camera.svg" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
</style>
