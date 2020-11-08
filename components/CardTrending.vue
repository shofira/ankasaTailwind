<template>
  <div>
    <div class="w-full md:max-w-3xl bg-blue-500 text-white rounded-3xl mx-auto text-center shadow-xl">
      <div class="p-10 leading-10">
        <p>Top 10</p>
        <div class="font-bold text-xl mb-2">Top Destination</div>
        <div class="grid grid-cols-1 sm:grid-cols-3 md:grid-cols-5  justify-items-center">
          <img src="../assets/img/paris.png" alt="paris" class="img-destination">
          <img src="../assets/img/bali.png" alt="Bali" class="img-destination">
          <img src="../assets/img/singapore.png" alt="Singapore" class="img-destination">
          <img src="../assets/img/agra.png" alt="Agra" class="img-destination">
          <img src="../assets/img/sydney.png" alt="Sydney" class="img-destination">
        </div>
        <div class="inline-flex space-x-3 my-5">
          <button class="btn-next">
            <Icons type='button-back'/>
          </button>
          <button class="btn-next">
            <Icons type='button-right'/>
          </button>
        </div>
      </div>
    </div>
  </div>
</template>