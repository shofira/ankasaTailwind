<template>
  <div class="shadow-xl">
    <nav class="container py-5 grid grid-cols-4 gap-10">
      <nuxt-link to="/">
        <img src="../assets/img/bluesmallplane.png" class="inline w-8 mr-2" alt="logo ankasa">
        <b class="text-xl text-gray-800 tracking-wider">Ankasa</b>
      </nuxt-link>
      <button class="bg-gray-200 hover:bg-gray-300 text-gray-800 rounded-md inline-flex items-center">
        <svg class="w-4 h-4 text-gray-500 ml-2" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z" />
        </svg>
        <input type="text" class="w-full bg-transparent text-gray-600 text-sm px-6 py-3 focus:outline-none rounded-md" placeholder="Where you want to go?">
      </button>

      <div class="flex items-center space-x-5">
        <nuxt-link to="">Find Ticket</nuxt-link>
        <nuxt-link to="/mybooking">My Booking</nuxt-link>
      </div>
      
      <!-- Condition -->
      <div v-if="type==='home'" class="flex space-x-8 items-center">
        <!-- <img src="../assets/img/message.png" alt="message" class="h-4 w-4">
        <img src="../assets/img/bell.png" alt="notification" class="h-5 w-4"> -->
        <nuxt-link to="/profile">
          <img src="../assets/img/profile.png" alt="profile" class="w-4/5 img-profile">
        </nuxt-link>
      </div>
      <div v-else>
        <nuxt-link to="/splashscreen" class="bg-blue-500 text-white text-center p-2 w-1/2 shadow-xl rounded-lg">
          Sign Up
        </nuxt-link>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  props: ['type']
}
</script>