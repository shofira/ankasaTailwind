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
        <nuxt-link to="/splashscreen" class="show sm:hidden">
          <Icons type="button-back" />
        </nuxt-link>

        <form class="mt-8 lg:mt-16">
          <b class="text-2xl text-gray-800">Login</b>
          <div class="mt-10 mb-4">
            <input class="w-full py-3 px-3 text-gray-700 text-sm mb-3 leading-tight border-b-2 focus:outline-none" type="text" placeholder="Username" required>
          </div>
          <div class="mb-3">
            <input class="w-full py-3 px-3 text-gray-700 text-sm mb-3 leading-tight border-b-2 focus:outline-none" type="password" placeholder="Password" required>
          </div>
          <button class="w-full bg-blue-500 text-white font-bold py-3 px-6 shadow-xl  hover:shadow-none focus:outline-none rounded-lg">
            Sign In
          </button>
          <div class="text-center mt-3 leading-6">
            <p class="text-gray-600 text-sm">Did you forgot your password?</p>
            <a class="text-right text-sm text-blue-500 hover:text-blue-700 cursor-pointer">
              Tap here for reset
            </a>

            <hr class="mt-5">
            <p class="text-sm text-gray-600 mt-3 mb-2">Or sign in with</p>
            <div class="flex items-center justify-center mb-4">
              <button class="bg-transparent border border-blue-500 py-3 px-6 mr-4 focus:outline-none shadow rounded" disabled>
                <img src="../assets/img/google.png" alt="google sign in">
              </button>
              <button class="bg-transparent border border-blue-500 py-3 px-6 focus:outline-none shadow rounded" disabled>
                <img src="../assets/img/fb.png" alt="facebook sign in">
              </button>
            </div>
            <a class="text-sm text-gray-700">
              Dont Have an account? 
              <nuxt-link to="/register" class=" text-blue-500 hover:text-blue-700 cursor-pointer">Please, create a new one</nuxt-link>
            </a>
          </div>
        </form>
      </div>
    </div>
  </div>
</template>