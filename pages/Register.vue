<template>
  <div>
    <div class="flex">
      <div class="w-3/5 bg-blue-500 h-screen flex">
        <img src="../assets/img/illustrationWhite.png" class="m-auto md:max-w-sm">
      </div>
      <div class="w-full md:w-2/5 h-screen p-8 md:p-10">
        <div class="">
          <img src="../assets/img/bluesmallplane.png" class="inline w-10 mr-2" alt="logo ankasa">
          <b class="text-xl text-gray-700 tracking-wider">ankasa</b>
        </div>
        <div class="hidden flex justify-between">
          <nuxt-link to="/splashscreen" class="inline">
            <Icons type="button-back" />
          </nuxt-link>
          <a class="text-blue-400 text-sm text-right cursor-pointer">Continue as Guest</a>
        </div>

        <form class="mt-8 lg:mt-16">
          <b class="text-2xl text-gray-800">Register</b>
          <div class="mt-10 mb-3">
            <input class="w-full py-3 px-3 text-gray-700 text-sm mb-3 leading-tight border-b-2 focus:outline-none" type="text" placeholder="Fullname" required>
          </div>
          <div class="mb-3">
            <input class="w-full py-3 px-3 text-gray-700 text-sm mb-3 leading-tight border-b-2 focus:outline-none" type="email" placeholder="Email@gmail.com" required>
          </div>
          <div class="mb-3">
            <input class="w-full py-3 px-3 text-gray-700 text-sm mb-3 leading-tight border-b-2 focus:outline-none" type="password" placeholder="Password" required>
          </div>
          <button @click="register" class="w-full bg-blue-500 text-white font-bold py-3 px-6 shadow-xl hover:shadow-none focus:outline-none rounded-lg">
            Sign Up
          </button>
            <label class="block mt-3 text-gray-600">
              <input class="mr-2" type="checkbox" required>
              <span class="text-sm tracking-wider">
                Accept terms and condition!
              </span>
            </label>
          <div class="text-center mt-3 leading-6">
            <hr>
            <p class="text-sm text-gray-600 mt-2 mb-3">Already have an account?</p>
            <div class="flex items-center justify-center">
              <nuxt-link to="/login" class="w-full border border-blue-500 text-blue-700 py-3 px-6 mr-4 focus:outline-none shadow-xl hover:shadow-none cursor-pointer rounded">
                Sign In
              </nuxt-link>
            </div>
          </div>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
import Swal from 'sweetalert2'
import Icons from '../components/Icons'

export default {
  name: 'Login',
  components: {
    Icons
  },
  methods: {
    register() {
      Swal.fire(
        'Your Registration Success',
        'Please Check Your Email to activate',
        'success'
      )
      this.$router.push('/login')
    }
  }
}
</script>