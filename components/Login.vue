<template>
 
  <main id="app">
        <div class="h-screen pb-14 bg-right bg-cover" style="background-image:url('Assets/meals/pizza.jpg');">
            <nav :class="headerClassList" class="fixed w-full z-30 top-0 header___bar">
                <div class="w-full container mx-auto flex flex-wrap items-center justify-between mt-0 py-2">
                    <div class="pl-4 flex items-center">
                         
                           <logo :isStickable="true" :isSticky="isSticky" />
    
                    </div>
                    <div class="block lg:hidden pr-4">
                        <button class="flex items-center p-1 text-orange-800 hover:text-gray-900" @click.prevent.stop="onToggleClick">
                            <svg class="fill-current h-6 w-6" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
                                <title>Menu</title>
                                <path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z" />
                            </svg>
                        </button>
                    </div>

                    <div :class="navContentClassList" class="w-full flex-grow lg:flex lg:items-center lg:w-auto lg:block mt-2 lg:mt-0 bg-white lg:bg-transparent text-black p-4 lg:p-0 z-20">
                        <ul class="list-reset lg:flex justify-center flex-1 items-center">
                            <li class="mr-3">
                                <a class="inline-block py-2 px-4 text-black font-bold no-underline" href="#">
                                    <nuxt-link to="/">HOME</nuxt-link>
                                </a>
                            </li>
                            <li class="mr-3">
                                <a class="inline-block text-black no-underline hover:text-gray-800 hover:text-underline py-2 px-4" href="#">
                                    <nuxt-link to="/products">FEATURES</nuxt-link>
                                </a>
                            </li>
                            <li class="mr-3">
                                <a class="inline-block text-black no-underline hover:text-gray-800 hover:text-underline py-2 px-4" href="#">
                                    <nuxt-link to="/products">PRODUCTS</nuxt-link>
                                </a>
                            </li>
                            <li class="mr-3">
                                <a class="inline-block text-black no-underline hover:text-gray-800 hover:text-underline py-2 px-4" href="#">
                                    <nuxt-link to="/services">SERVICES</nuxt-link>
                                </a>
                            </li>
                            <li class="mr-3">
                                <a class="inline-block text-black no-underline hover:text-gray-800 hover:text-underline py-2 px-4" href="#">BLOG</a>
                            </li>
                            <li class="mr-3">
                                <a class="inline-block text-black no-underline hover:text-gray-800 hover:text-underline py-2 px-4" href="#">
                                    <nuxt-link to="/contactus">CONTACT US</nuxt-link>
                                </a>
                            </li>
                        </ul>

                        <ul class="list-reset lg:flex justify-end  items-center">
                            <a class="inline-block py-2 px-4 text-black font-bold text-4xl no-underline" href="#">
                                <i class="fa fa-shopping-cart" aria-hidden="true"></i>
                            </a>
                        </ul>
                    </div>
                </div>
                <hr class="border-b border-gray-100 opacity-25 my-0 py-0" />
            </nav>

            <!--Main-->
            <div class="container pt-12  px-6 mx-auto flex flex-wrap justify-end  md:flex-row items-center">
                <div class="p-4 lg:w-1/2 ">
                    <div class="h-full bg-gray-200 px-8 pt-16 pb-24 rounded-lg overflow-hidden text-left relative leading-8 ">
                        <h1 class="title-font sm:text-2xl text-xl font-medium text-gray-900 mb-3">Chelpi For Chefs</h1>
                        <h2 class="leading-relaxed mb-3">A world of food lovers now
                            <br> within your reach</h2>
                        <p>Join thousands of chef, build a community of food lovers, share and sell recipes, sell meals, share
                            skill and get inspired.</p>
                        <div class="text-center mt-2 leading-none flex justify-left  py-4">
                            <a href="#" class="p-8 bg-black text-white "> Create Virtual Restaurant</a>
                        </div>
                    </div>
                </div>
            </div>



        </div>

        <section class="text-gray-700 body-font">
            <div class="container px-5 py-24 mx-auto">
                <div class="text-center mb-20">
                    <h1 class="sm:text-3xl text-2xl font-medium title-font text-gray-900 mb-4">Why Chelpi</h1>
                </div>
                <div class="flex flex-wrap sm:-m-4 -mx-4 -mb-10 -mt-4">
                    <div class="p-4 md:w-1/2 md:mb-0 mb-6 flex flex-col items-center">
                        <div class="w-20 h-20 inline-flex items-center   mb-5 flex-shrink-0">

                        </div>
                        <div class="flex-grow">
                            <h2 class="text-gray-900 text-lg title-font font-medium mb-3">Do Less, Have More</h2>
                            <p class="leading-relaxed text-base">Focus on what you love that is preparing meals, while we do the hard work by delivering your
                                meals, satisfy customers with the food they want—when and where they want it.</p>

                        </div>
                    </div>
                    <div class="p-4 md:w-1/2 md:mb-0 mb-6 flex flex-col items-center">
                        <div class="w-20 h-20 inline-flex   mb-5 flex-shrink-0">

                        </div>
                        <div class="flex-grow">
                            <h2 class="text-gray-900 text-lg title-font font-medium mb-3">Access Food Lovers</h2>
                            <p class="leading-relaxed text-base">Reach thousands of users searching for food within your location. Sell to a variety of food lovers,
                                connect, share and learn.</p>

                        </div>
                    </div>
                </div>
                <div class="flex flex-wrap sm:-m-4 -mx-4 -mb-10 -mt-4">
                    <div class="p-4 md:w-1/2 md:mb-0 mb-6 flex flex-col items-center">
                        <div class="w-20 h-20 inline-flex items-center   mb-5 flex-shrink-0">

                        </div>
                        <div class="flex-grow">
                            <h2 class="text-gray-900 text-lg title-font font-medium mb-3">Do Less, Have More</h2>
                            <p class="leading-relaxed text-base">Focus on what you love that is preparing meals, while we do the hard work by delivering your
                                meals, satisfy customers with the food they want—when and where they want it.</p>

                        </div>
                    </div>
                    <div class="p-4 md:w-1/2 md:mb-0 mb-6 flex flex-col items-center">
                        <div class="w-20 h-20 inline-flex   mb-5 flex-shrink-0">

                        </div>
                        <div class="flex-grow">
                            <h2 class="text-gray-900 text-lg title-font font-medium mb-3">Access Food Lovers</h2>
                            <p class="leading-relaxed text-base">Reach thousands of users searching for food within your location. Sell to a variety of food lovers,
                                connect, share and learn.</p>

                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section class="text-gray-700 body-font">
            <div class="container px-5 py-24 mx-auto">
                <div class="flex flex-col text-center w-full mb-20">
                    <h1 class="sm:text-3xl text-2xl font-medium title-font mb-4 text-gray-900">How Chelpi Works</h1>
                </div>
                <div class="flex flex-wrap sm:-m-4 -mx-4 -mb-10 -mt-4">
                    <div class="p-4 md:w-1/3 sm:mb-0 mb-6">
                        <div class="g h-64 overflow-hidden">
                            <img alt="content" class="object-cover object-center h-full w-full" src="Assets/meals/meat.jpg">
                        </div>

                    </div>
                    <div class="p-4 md:w-1/3 sm:mb-0 mb-6">
                        <div class=" h-64 overflow-hidden">
                            <img alt="content" class="object-cover object-center h-full w-full" src="Assets/meals/sandwich.jpg">
                        </div>

                    </div>
                    <div class="p-4 md:w-1/3 sm:mb-0 mb-6">
                        <div class=" h-64 overflow-hidden">
                            <img alt="content" class="object-cover object-center h-full w-full" src="Assets/meals/pizza.jpg">
                        </div>

                    </div>
                </div>
            </div>
        </section>

    </main>

   
</template>

<script>
import Logo from '@/components/Logo'
export default {
  name: 'Login'
   components: {
    logo: Logo
  },
}
</script>
