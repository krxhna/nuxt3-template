<template>

    <!-- <button class="bg-yellow-500" @click="isnewuser('fds')"> meow </button> -->
    <div v-if="!isloggedin" class="bg-white h-screen">
      <div class="min-h-full flex  font-monda  ">
        <div class="flex-1 flex flex-col justify-center py-12 px-4 sm:px-6 lg:flex-none lg:px-20 xl:px-24">
          <div class="mx-auto w-full max-w-sm lg:w-96">
            <div>
              <!-- <img class="h-12 w-auto" src="https://tailwindui.com/img/logos/workflow-mark-indigo-600.svg" alt="Workflow" /> -->
              <h2 class="mt-6 text-3xl font-extrabold text-gray-900">Create a new account</h2>
              <p class="mt-2 text-sm text-gray-600">
                Or
                {{ ' ' }}
                <a href="/signin" class="font-medium text-indigo-600 hover:text-indigo-500"> login to your existing</a>
              </p>
            </div>
  
            <div class="mt-8">
              <div>
                <div>
                  <!-- <p class="text-sm font-medium text-gray-700">Sign in with</p> -->
  
                  <div class="mt-1  gap-3">
                    <div>
                      <button @click="googlesignin()"
                        class="w-full inline-flex justify-center  px-4 border items-center border-gray-300 rounded-md shadow-sm bg-white text-sm font-medium text-gray-500 hover:bg-gray-50">
                        <span class="sr-only">Sign in with google</span>
                        <svg width="46px" height="46px" viewBox="0 0 46 46" version="1.1"
                          xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"
                          xmlns:sketch="http://www.bohemiancoding.com/sketch/ns">
                          <g id="Google-Button" stroke="none" stroke-width="1" fill="none" fill-rule="evenodd"
                            sketch:type="MSPage">
                            <g id="9-PATCH" sketch:type="MSArtboardGroup" transform="translate(-608.000000, -160.000000)">
                            </g>
                            <g id="btn_google_light_normal" sketch:type="MSArtboardGroup"
                              transform="translate(-1.000000, -1.000000)">
                              <g id="button" sketch:type="MSLayerGroup" transform="translate(4.000000, 4.000000)"
                                filter="url(#filter-1)">
                                <g id="button-bg">
                                  <use fill="#FFFFFF" fill-rule="evenodd" sketch:type="MSShapeGroup" xlink:href="#path-2">
                                  </use>
                                  <use fill="none" xlink:href="#path-2"></use>
                                  <use fill="none" xlink:href="#path-2"></use>
                                  <use fill="none" xlink:href="#path-2"></use>
                                </g>
                              </g>
                              <g id="logo_googleg_48dp" sketch:type="MSLayerGroup"
                                transform="translate(15.000000, 15.000000)">
                                <path
                                  d="M17.64,9.20454545 C17.64,8.56636364 17.5827273,7.95272727 17.4763636,7.36363636 L9,7.36363636 L9,10.845 L13.8436364,10.845 C13.635,11.97 13.0009091,12.9231818 12.0477273,13.5613636 L12.0477273,15.8195455 L14.9563636,15.8195455 C16.6581818,14.2527273 17.64,11.9454545 17.64,9.20454545 L17.64,9.20454545 Z"
                                  id="Shape" fill="#4285F4" sketch:type="MSShapeGroup"></path>
                                <path
                                  d="M9,18 C11.43,18 13.4672727,17.1940909 14.9563636,15.8195455 L12.0477273,13.5613636 C11.2418182,14.1013636 10.2109091,14.4204545 9,14.4204545 C6.65590909,14.4204545 4.67181818,12.8372727 3.96409091,10.71 L0.957272727,10.71 L0.957272727,13.0418182 C2.43818182,15.9831818 5.48181818,18 9,18 L9,18 Z"
                                  id="Shape" fill="#34A853" sketch:type="MSShapeGroup"></path>
                                <path
                                  d="M3.96409091,10.71 C3.78409091,10.17 3.68181818,9.59318182 3.68181818,9 C3.68181818,8.40681818 3.78409091,7.83 3.96409091,7.29 L3.96409091,4.95818182 L0.957272727,4.95818182 C0.347727273,6.17318182 0,7.54772727 0,9 C0,10.4522727 0.347727273,11.8268182 0.957272727,13.0418182 L3.96409091,10.71 L3.96409091,10.71 Z"
                                  id="Shape" fill="#FBBC05" sketch:type="MSShapeGroup"></path>
                                <path
                                  d="M9,3.57954545 C10.3213636,3.57954545 11.5077273,4.03363636 12.4404545,4.92545455 L15.0218182,2.34409091 C13.4631818,0.891818182 11.4259091,0 9,0 C5.48181818,0 2.43818182,2.01681818 0.957272727,4.95818182 L3.96409091,7.29 C4.67181818,5.16272727 6.65590909,3.57954545 9,3.57954545 L9,3.57954545 Z"
                                  id="Shape" fill="#EA4335" sketch:type="MSShapeGroup"></path>
                                <path d="M0,0 L18,0 L18,18 L0,18 L0,0 Z" id="Shape" sketch:type="MSShapeGroup"></path>
                              </g>
                              <g id="handles_square" sketch:type="MSLayerGroup"></g>
                            </g>
                          </g>
                        </svg>
                        <p>Sign up with google</p>
                      </button>
                    </div>
  
  
                  </div>
                </div>
  
                <div class="mt-6 relative">
                  <div class="absolute inset-0 flex items-center" aria-hidden="true">
                    <div class="w-full border-t border-gray-300" />
                  </div>
                  <div class="relative flex justify-center text-sm">
                    <span class="px-2 bg-white text-gray-500"> Or continue with </span>
                  </div>
                </div>
              </div>
  
              <div class="mt-6">
                <div class="space-y-6">
  
                  <div>
                    <label for="name" class="block text-sm font-medium text-gray-700">Name </label>
                    <div class="mt-1">
                      <input id="name" name="name" type="name" autocomplete="name" v-model="name"
                        class="appearance-none block w-full px-3 py-2 border border-gray-300 rounded-md shadow-sm placeholder-gray-400 focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 sm:text-sm" />
                    </div>
                  </div>
                  <div class="space-y-1">
                    <label for="email" class="block text-sm font-medium text-gray-700"> Email address </label>
                    <div class="mt-1">
                      <input id="email" name="email" type="email" autocomplete="email" v-model="email"
                        class="appearance-none block w-full px-3 py-2 border border-gray-300 rounded-md shadow-sm placeholder-gray-400 focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 sm:text-sm" />
                    </div>
                  </div>
  
                  <div class="space-y-1">
                    <label for="password" class="block text-sm font-medium text-gray-700"> Password </label>
                    <div class="mt-1">
                      <input id="password" v-model="password" name="password" type="password"
                        autocomplete="current-password"
                        class="appearance-none block w-full px-3 py-2 border border-gray-300 rounded-md shadow-sm placeholder-gray-400 focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 sm:text-sm" />
                    </div>
                  </div>
  
                  <div class="flex items-center justify-between">
                    <div class="flex items-center">
                      <input id="remember-me" name="remember-me" type="checkbox"
                        class="h-4 w-4 text-indigo-600 focus:ring-indigo-500 border-gray-300 rounded" />
                      <label for="remember-me" class="ml-2 block text-sm text-gray-900"> Remember me </label>
                    </div>
  
                    <!-- <div class="text-sm">
                    <a href="#" class="font-medium text-indigo-600 hover:text-indigo-500"> Forgot your password? </a>
                  </div> -->
                  </div>
  
                  <div>
                    <button type="submit" @click="emailsignup(name)"
                      class="w-full flex justify-center py-3 px-4 border border-transparent rounded-md shadow-sm text-sm font-medium text-white bg-indigo-600 hover:bg-indigo-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500">Sign
                      up</button>
                  </div>
                  <!-- <div class="text-sm">
                    <a href="#" class="font-medium "> Forgot your password? </a>
                  </div> -->
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="hidden lg:block relative w-0 flex-1">
          <img class="absolute inset-0 h-full w-full object-cover"
            src="https://cdn.jsdelivr.net/gh/krxhna/gorilla-images/auth/authcover.jpg" alt="" />
        </div>
      </div>
    </div>
  
    <div v-else class="bg-red-400">
      <div class="flex items-center justify-center w-screen h-screen bg-gradient-to-r from-indigo-600 to-blue-400">
        <img class="absolute   bottom-0 right-0 w-screen" src="@/assets/beams.png" alt="" />
  
        <div class="relative px-40 py-20 bg-black/40 rounded-md shadow-xl">
          <div class="flex flex-col items-center">
            <h1 class="font-bold text-white text-5xl m-5">
              You’re already logged in
            </h1>
  
            <!-- <h6 class="mb-2 text-2xl font-bold text-center text-gray-800 md:text-3xl">
          <span class="text-red-500">Oops!</span> Page not found
        </h6> -->
  
            <p class="mb-8 text-center text-gray-500 md:text-lg">
              Navigate back to home page 🏠
            </p>
  
            <a href="/home"
              class="px-6 py-2 text-lg font-semibold text-black bg-white rounded-md p-4 hover:scale-105 shadow-sm transition-all duration-200">Go
              home</a>
          </div>
        </div>
      </div>
    </div>
  
    <!-- Footer Mentions -->
  </template>
  
  <script setup lang="ts">
  import { onMounted } from "vue";

  
  const router = useRouter();
  const route = useRoute();
  
  
  
  const email = ref("");
  const password = ref("");
  const name = ref("");

  const isloggedin = ref(false);


  function emailsignup(email: any){

  }

  function googlesignin() {
    console.log("google signin");
  }

  </script>
  
  <style>
  
  </style>