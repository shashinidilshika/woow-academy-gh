<template>
  <header>
    <nav class="border-gray-200 px-4 lg:px-6 py-2.5 z-10">
      <div class="flex flex-wrap justify-between items-center mx-auto">
        <a class="flex items-center" href="/">
          <span class="self-center pb-5 text-xl font-semibold whitespace-nowrap dark:text-white"
            >Woow <br />
            Space</span
          >
        </a>
        <div class="flex items-center justify-between lg:order-2 pb-5">
          <div class="flex justify-center items-center w-fit pl-8 pr-8">
            <img alt="Flowbite Logo" class="mr-3 h-6 sm:h-9" src="../../../assets/images/points-icon.png" />
            <h5 class="text-white">56473</h5>
          </div>
          <NuxtLink to="/profile">
            <img
              alt="profile image"
              class="mr-3 h-6 sm:h-9 rounded-full"
              src="https://avatars.githubusercontent.com/u/50085447?s=96&v=4"
            />
          </NuxtLink>
          <button
            aria-controls="mobile-menu-2"
            aria-expanded="false"
            class="inline-flex items-center p-2 ml-1 text-sm text-gray-500 rounded-lg lg:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-100 dark:hover:bg-gray-700 dark:focus:ring-gray-600"
            data-collapse-toggle="mobile-menu-2"
            type="button"
          >
            <span class="sr-only">Open main menu</span>
            <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
              <path
                clip-rule="evenodd"
                d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z"
                fill-rule="evenodd"
              ></path>
            </svg>
            <svg class="hidden w-6 h-6" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
              <path
                clip-rule="evenodd"
                d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z"
                fill-rule="evenodd"
              ></path>
            </svg>
          </button>
        </div>
        <div id="mobile-menu-2" class="pb-5 hidden justify-between items-center w-full lg:flex lg:w-auto lg:order-1">
          <ul class="flex flex-col mt-4 font-medium lg:flex-row lg:space-x-8 lg:mt-0 text-white">
            <li>
              <NuxtLink
                aria-current="page"
                class="block py-2 pr-4 pl-3 text-white rounded lg:bg-transparent lg:p-0 dark:text-white"
                to="/"
                >Home
              </NuxtLink>
            </li>
            <li>
              <NuxtLink
                class="block py-2 pr-4 pl-3 text-gray-700 border-b border-gray-100 hover:bg-gray-50 lg:hover:bg-transparent lg:border-0 lg:hover:text-blue-700 lg:p-0 dark:text-gray-100 lg:dark:hover:text-white dark:hover:bg-gray-700 dark:hover:text-white lg:dark:hover:bg-transparent dark:border-gray-700"
                to="/course"
                >Course
              </NuxtLink>
            </li>
            <li>
              <a
                class="block py-2 pr-4 pl-3 text-gray-700 border-b border-gray-100 hover:bg-gray-50 lg:hover:bg-transparent lg:border-0 lg:hover:text-blue-700 lg:p-0 dark:text-gray-100 lg:dark:hover:text-white dark:hover:bg-gray-700 dark:hover:text-white lg:dark:hover:bg-transparent dark:border-gray-700"
                href="#"
                >Code Playground</a
              >
            </li>
            <li>
              <a
                class="block py-2 pr-4 pl-3 text-gray-700 border-b border-gray-100 hover:bg-gray-50 lg:hover:bg-transparent lg:border-0 lg:hover:text-blue-700 lg:p-0 dark:text-gray-100 lg:dark:hover:text-white dark:hover:bg-gray-700 dark:hover:text-white lg:dark:hover:bg-transparent dark:border-gray-700"
                href="#"
                >Top Learners</a
              >
            </li>
            <li>
              <a
                class="block py-2 pr-4 pl-3 text-gray-700 border-b border-gray-100 hover:bg-gray-50 lg:hover:bg-transparent lg:border-0 lg:hover:text-blue-700 lg:p-0 dark:text-gray-100 lg:dark:hover:text-white dark:hover:bg-gray-700 dark:hover:text-white lg:dark:hover:bg-transparent dark:border-gray-700"
                href="#"
                >Blog</a
              >
            </li>
            <li>
              <a
                class="block py-2 pr-4 pl-3 text-gray-700 border-b border-gray-100 hover:bg-gray-50 lg:hover:bg-transparent lg:border-0 lg:hover:text-blue-700 lg:p-0 dark:text-gray-100 lg:dark:hover:text-white dark:hover:bg-gray-700 dark:hover:text-white lg:dark:hover:bg-transparent dark:border-gray-700"
                href="#"
                >FAQ</a
              >
            </li>
            <li>
              <a
                class="block py-2 pr-4 pl-3 text-gray-700 border-b border-gray-100 hover:bg-gray-50 lg:hover:bg-transparent lg:border-0 lg:hover:text-blue-700 lg:p-0 dark:text-gray-100 lg:dark:hover:text-white dark:hover:bg-gray-700 dark:hover:text-white lg:dark:hover:bg-transparent dark:border-gray-700"
                href="#"
                >Contact</a
              >
            </li>
            <li>
              <a
                class="block py-2 pr-4 pl-3 text-gray-700 border-b border-gray-100 hover:bg-gray-50 lg:hover:bg-transparent lg:border-0 lg:hover:text-blue-700 lg:p-0 dark:text-gray-100 lg:dark:hover:text-white dark:hover:bg-gray-700 dark:hover:text-white lg:dark:hover:bg-transparent dark:border-gray-700"
                href="#"
                >Terms of Use</a
              >
            </li>
            <li>
              <a
                class="block py-2 pr-4 pl-3 text-gray-700 border-b border-gray-100 hover:bg-gray-50 lg:hover:bg-transparent lg:border-0 lg:hover:text-blue-700 lg:p-0 dark:text-gray-100 lg:dark:hover:text-white dark:hover:bg-gray-700 dark:hover:text-white lg:dark:hover:bg-transparent dark:border-gray-700"
                href="#"
                >Privacy Policy</a
              >
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </header>
</template>

<script lang="ts" setup></script>

<style scoped>
header {
  background-image: url(../../../assets/images/HeaderBackgroung.svg);
  background-repeat: no-repeat;
  background-position: 80% 90%;
  background-size: cover;
}
</style>
