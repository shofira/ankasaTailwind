<template>
  <div>
    <Header />
    <div class="flex justify-between py-3">
      <div class="my-12">
        <h4 class="flex text-5xl text-gray-800 justify-center">Find your
          <p class="text-blue-500">&nbsp; Flight</p>
        </h4>
        <p class="flex text-gray-500 justify-center">and explore the world with us</p>
        <img src="../assets/img/jumbotronimage1.png" alt="jumbotron left" class="my-16">
      </div>
      <div>
        <img src="../assets/img/jumbotronimage2.jpg" alt="jumbotron right">
        <img src="../assets/img/vector.png" alt="vector" class="w-2/3 ">
      </div>
    </div>
    <div class="container pb-10">
      <b class="text-tracking mb-2">Trending</b>
      <p class="font-bold text-xl mb-5">Trending Destinations</p>
      <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-5 justify-items-center mb-20">
        <img src="../assets/img/trending1.png" alt="trending" class="image-trending rounded-3xl">
        <img src="../assets/img/trending2.png" alt="trending" class="image-trending rounded-3xl">
        <img src="../assets/img/trending1.png" alt="trending" class="image-trending rounded-3xl">
        <img src="../assets/img/trending2.png" alt="trending" class="image-trending flex md:hidden lg:flex rounded-3xl">
      </div>
      <CardTrending />
    </div>
    <Footer />
  </div>
</template>
