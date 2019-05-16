<template>
  <div id="app" class="min-h-screen bg-navy-darker font-sans antialiased leading-tight">
    <div class="container mx-auto px-6">
      <header class="flex justify-between items-center py-8">
        <div>
          <img class="block h-12" src="./assets/transistor-logo.svg" alt="Logo">
        </div>
        <div>
          <a class="font-medium no-underline text-white hover:underline" href="#">Sign In</a>
        </div>
      </header>
      <div class>
        <h1
          class="py-16 pb-16 text-white text-3xl font-medium text-center"
        >Start your podcast today:</h1>
        <div class="flex flex-wrap -mx-6">
          <div class="w-1/2">
            <plan-selector></plan-selector>
          </div>

          <div class="w-1/2 px-4 pt-10">
            <form action="#" method="POST">
              <input
                type="text"
                placeholder="Your Name"
                class="mb-4 block w-full bg-navy-dark px-4 py-4 rounded text-xl text-center text-white font-medium focus:bg-navy focus:outline-none"
              >
              <input
                type="email"
                placeholder="Your Email"
                class="mb-4 block w-full bg-navy-dark px-4 py-4 rounded text-xl text-center text-white font-medium focus:bg-navy focus:outline-none"
              >
              <input
                type="password"
                placeholder="Set Your Password"
                class="mb-4 block w-full bg-navy-dark px-4 py-4 rounded text-xl text-center text-white font-medium focus:bg-navy focus:outline-none"
              >
              <input
                type="number"
                placeholder="Card number"
                class="mb-4 block w-full bg-navy-dark px-4 py-4 rounded text-xl text-center text-white font-medium focus:bg-navy focus:outline-none"
              >
              <button
                class="bg-yellow mb-4 block w-full uppercase px-4 py-4 text-yellow-dark font-semibold rounded-lg border-b-2"
              >Create my account</button>
              <p
                class="text-white font-bold text-sm text-center"
              >Includes a 14 day trial before billing begins</p>
            </form>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import PlanSelector from './components/PlanSelector.vue'

export default {
  name: "app",
  components: {
    PlanSelector
  }
}
</script>

<style>
@tailwind base;
@tailwind components;
@tailwind utilities;
</style>