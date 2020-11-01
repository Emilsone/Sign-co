<template>
  <div class="pt-24">
    <main
      class="bg-white max-w-lg mx-auto p-8 md:p-12 my-10 rounded-lg shadow-2xl"
    >
      <section>
        <h3 class="font-bold text-2xl text-gray-600">Welcome to Signco</h3>
        <p class="text-gray-600 pt-2">Sign in to your account.</p>
      </section>
      <section class="mt-10">
        <form class="" netlify>
          <div class="mb-6 pt-3 rounded bg-gray-200">
            <label
              class="block text-gray-700 text-sm font-bold mb-2 ml-3"
              for="email"
              >Email</label
            >
            <input
              type="text"
              id="email"
              class="bg-gray-200 rounded w-full text-gray-700 focus:outline-none border-b-4 border-gray-300 focus:border-orange-600 transition duration-500 px-3 pb-3"
            />
          </div>
          <div class="mb-6 pt-3 rounded bg-gray-200">
            <label
              class="block text-gray-700 text-sm font-bold mb-2 ml-3"
              for="password"
              >Password</label
            >
            <input
              type="password"
              id="password"
              class="bg-gray-200 rounded w-full text-gray-700 focus:outline-none border-b-4 border-gray-300 focus:border-orange-600 transition duration-500 px-3 pb-3"
            />
          </div>
          <div class="flex justify-end">
            <a
              href="#"
              class="text-sm text-black hover:text-orange-700 hover:underline mb-6"
              >Forgot your password?</a
            >
          </div>
          <button
            class="bg-orange-600 hover:bg-purple-700 text-white font-bold py-2 px-8 rounded shadow-lg hover:shadow-xl transition duration-200"
            type="submit"
          >
            Sign In
          </button>
        </form>
      </section>
    </main>
  </div>
</template>

<script>
export default {
  name: 'HeroContent'
}
</script>
