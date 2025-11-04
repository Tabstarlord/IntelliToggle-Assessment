<template>
  <section class="bg-radial-[at_50%_50%] from-[#f2f1fe] to-[#3c29eb67] to-100% py-5 px-2 relative">
    <div class="flex justify-between items-center px-4 py-2">
      <img src="/Logo1.png" alt="IntelliToggle Logo" class="w-25 lg:w-40" />

      <!-- Desktop Button -->
      <button class="bg-[#42389E] px-3 py-1 rounded-sm font-medium text-white text-sm shadow-md lg:text-lg">
        Get Started
      </button>

      <!-- Hamburger Menu (Mobile only) -->
      <button @click="toggleSidebar" class="md:hidden text-[#42389E] focus:outline-none">
        <!-- Simple Hamburger Icon -->
        <svg
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          stroke-width="2"
          stroke="currentColor"
          class="w-7 h-7"
        >
          <path stroke-linecap="round" stroke-linejoin="round" d="M4 6h16M4 12h16M4 18h16" />
        </svg>
      </button>
    </div>

    <!-- Sidebar (Mobile Drawer - Right Side) -->
    <transition name="slide-right">
      <div
        v-if="isSidebarOpen"
        class="fixed inset-0 bg-black/40 z-40 md:hidden"
        @click.self="toggleSidebar"
      >
        <div
          class="absolute right-0 top-0 w-2/3 max-w-xs bg-white h-full shadow-lg p-4 z-50"
        >
          <button
            @click="toggleSidebar"
            class="absolute top-3 right-3 text-gray-600 hover:text-gray-800"
          >
            ✕
          </button>
          <div class="mt-10">
            <!-- Empty Sidebar Content -->
            <p class="text-sm text-gray-700">Sidebar content here...</p>
          </div>
        </div>
      </div>
    </transition>

    <h4 class="text-[#42389E] text-center my-5 font-bold text-2xl md:text-3xl lg:text-5xl">
      The First Dart-Native <br /> Feature Flag & DartCodeAI
    </h4>
    <p class="text-[#42389E] text-sm lg:text-xl text-center justify-center my-5">
      Ship faster, control rollouts, and get ready for AI-powered delivery, starting at just $1/month for a limited time
    </p>
    <div class="flex w-fit mx-auto gap-4">
      <button
        class="bg-[#42389E] px-3 py-1 rounded-sm font-medium text-white text-sm shadow-md lg:text-lg">
        Start for $1/mo
      </button>
      <button
        class="border border-[#42389E] px-3 py-1 rounded-sm font-medium text-[#42389E] text-sm shadow-md lg:text-lg">
        Join AI Early Access
      </button>
    </div>
     <div class="flex mt-5 items-center justify-center px-6">
      <div class="relative w-[800px] md:w-[1000px]"> <!-- fixed reference -->
    <img src="/Frame2.png" alt="Dashboard Preview" class="w-full" />
    <img src="/Frame-1.png" alt="Floating left card"
         class="absolute w-[120px] md:w-[180px] top-[35%] left-0" />
    <img src="/Frame3.png" alt="Floating right card"
         class="absolute w-20 md:w-[150px] top-[23%] right-0" />
  </div>
</div>

  </section>

  <section class="bg-[#42389E] flex px-1 md:px-2 gap-2 py-5 md:justify-between md:items-center">
    <p class="text-xs font-medium text-white lg:text-lg">$1/month for your first year Normally $10/month. Sign up before September 15, 2025.</p>
    <div class="flex gap-2">
      <p class="grid bg-[#F9A71E] p-1.5 rounded-lg text-xs lg:text-lg text-white text-center font-semibold">36<span class="font-normal">DAYS</span></p>
      <p class="grid bg-[#F9A71E] p-1.5 rounded-lg text-xs text-white text-center font-semibold lg:text-lg">04<span class="font-normal">HRS</span></p>
      <p class="grid bg-[#F9A71E] p-1.5 rounded-lg text-xs text-white text-center font-semibold lg:text-lg">45<span class="font-normal">MIN</span></p>
      <p class="grid bg-[#F9A71E] p-1.5 rounded-lg text-xs text-white text-center font-semibold lg:text-lg">22<span class="font-normal">SEC</span></p>
    </div>
  </section>

  <section class="px-2 py-7">
    <h2 class="text-center font-semibold text-lg lg:text-3xl">Built For Every Team</h2>
    <p class="text-sm text-center lg:text-lg">Whether you're shipping code, managing products, or driving growth</p>
    <div class="md:flex gap-3">
      <div class="border border-gray-200 rounded-lg shadow-md p-2 my-3">
        <img src="/Frame4.png" alt="cards Image" class="w-10 lg:w-20 mx-auto" />
        <h2 class="text-sm font-semibold text-center lg:text-xl">Developers</h2>
        <p class="text-xs text-center lg:text-lg">Safely deploy and control feature rollouts with zero-downtime toggles.</p>
      </div>
      <div class="border border-gray-200 rounded-lg shadow-md p-2 my-3">
        <img src="/Frame4.png" alt="cards Image" class="w-10 lg:w-20 mx-auto" />
        <h2 class="text-sm font-semibold text-center lg:text-xl">Product Managers</h2>
        <p class="text-xs text-center lg:text-lg">Run experiments, manage rollouts, and launch features on your terms.</p>
      </div>
      <div class="border border-gray-200 rounded-lg shadow-md p-2 my-3">
        <img src="/Frame4.png" alt="cards Image" class="w-10 lg:w-20 mx-auto" />
        <h2 class="text-sm font-semibold text-center lg:text-xl">Enterprises</h2>
        <p class="text-xs text-center lg:text-lg">Secure, compliant, and scalable toggle management built with Dart reliability.</p>
      </div>
    </div>
  </section>

  <section class="px-2 py-7">
    <h2 class="text-center font-semibold text-lg lg:text-3xl">Powerful Features, Simplified</h2>
    <p class="text-center text-sm lg:text-lg">AI-driven intelligence meets developer-friendly simplicity</p>
    <div class="grid grid-cols-2 gap-3">
      <div class="bg-[#ECEBF5] rounded-lg shadow-md py-2 px-1 mt-3">
        <img src="/Frame5.png" alt="card image" class="w-8 lg:w-18 mb-3" />
        <h2 class="font-semibold text-sm my-1 lg:text-xl">AI-powered Flag Creation</h2>
        <p class="text-xs lg:text-lg">Our AI analyzes your user base, traffic patterns, and historical data to suggest optimal rollout strategies automatically</p>
        <a href="#" class="text-[#42389E] text-xs lg:text-base">Get Started</a>
      </div>
       <div class="bg-[#ECEBF5] rounded-lg shadow-md py-2 px-1 mt-3">
        <img src="/Frame5.png" alt="card image" class="w-8 lg:w-18 mb-3" />
        <h2 class="font-semibold text-sm my-1 lg:text-xl">Smart Targeting</h2>
        <p class="text-xs lg:text-lg">Advanced user segmentation with real-time behavioral analysis ensures your features reach the most engaged audience.</p>
        <a href="#" class="text-[#42389E] text-xs lg:text-base">Get Started</a>
      </div>
      <div class="bg-[#ECEBF5] rounded-lg shadow-md py-2 px-1 my-3">
        <img src="/Frame5.png" alt="card image" class="w-8 lg:w-18 mb-3" />
        <h2 class="font-semibold text-sm my-1 lg:text-xl">Flag Cleanup</h2>
        <p class="text-xs lg:text-lg">Keep your codebase clean with intelligent flag lifecycle management that removes technical debt automatically.</p>
        <a href="#" class="text-[#42389E] text-xs lg:text-base">Get Started</a>
      </div>
      <div class="bg-[#ECEBF5] rounded-lg shadow-md py-2 px-1 my-3">
        <img src="/Frame5.png" alt="card image" class="w-8 lg:w-18 mb-3" />
        <h2 class="font-semibold text-sm my-1 lg:text-xl">Environment & A/B Testing</h2>
        <p class="text-xs lg:text-lg">Multi-environment support with sophisticated A/B testing framework gives you confidence in every release.</p>
        <a href="#" class="text-[#42389E] text-xs lg:text-base">Get Started</a>
      </div>
    </div>
  </section>
  <section class="px-2 py-7">
    <div class="md:flex items-center">
      <div class="my-2">
        <button class="text-xs text-[#F9A71E] bg-[#FFEBC9] py-1 px-1.5 rounded-xl lg:text-base">Coming Soon</button>
        <h2 class="font-semibold lg:text-2xl">Be First to Power Your Features withDartCode AI</h2>
        <p class="text-sm lg:text-lg">DartCode AI is the only AI built specifically for Dart feature flagging. It learns from your app’s live usage, optimizes rollouts in real time, and safeguards every release</p>
        <div class="flex items-center gap-2 my-3">
          <img src="/Icon.png" alt="icon" class="w-6 h-6 lg:w-16 lg:h-16" />
          <h2 class="text-[#3F3F3F] text-sm font-semibold lg:text-lg">Predict Rollout Success<p class="font-normal text-xs lg:text-base">Forecast which users will adopt features fastest</p></h2>
        </div>
        <div class="flex items-center gap-2 my-3">
          <img src="/Icon.png" alt="icon" class="w-6 h-6 lg:w-16 lg:h-16" />
          <h2 class="text-[#3F3F3F] text-sm font-semibold lg:text-lg">Adapt Without Guesswork<p class="font-normal text-xs lg:text-base">Automatic rollout adjustments based on live results.</p></h2>
        </div>
        <div class="flex items-center gap-2 my-3">
          <img src="/Icon.png" alt="icon" class="w-6 h-6 lg:w-16 lg:h-16" />
          <h2 class="text-[#3F3F3F] text-sm font-semibold lg:text-lg">Prevent Costly Mistakes<p class="font-normal text-xs lg:text-base">Early anomaly detection and instant rollback cues.</p></h2>
        </div>
        <button class="bg-[#42389E] text-sm py-1 px-2 mt-5 mb-3 rounded-md text-white lg:text-xl">
          Start for $1/mo
        </button>
      </div>
      <img src="/Frame6.png" alt="section image" class="md:w-sm lg:w-md" />
    </div>
  </section>

  <section class="px-2 py-7">
    <h2 class="text-center text-sm text-[#42389E] mb-3 lg:text-xl">Trusted by various engineering teams</h2>
    <div class="grid grid-cols-3 gap-1.5 w-fit mx-auto md:flex md:gap-7 lg:gap-5">
      <img src="/Google.png" alt="google" class="lg:w-45" />
      <img src="/amazon.png" alt="amazone" class="lg:w-45"/>
      <img src="/Azure.png" alt="microsoft azure" class="lg:w-45" />
      <img src="/DigitalOcean.png" alt="digital ocean" class="lg:w-45" />
      <img src="/ibm.png" alt="IBM" class="lg:w-45" />
    </div>
  </section>

  <section class="bg-[#ECEBF5] px-2 py-7">
    <h2 class="font-semibold text-[#42389E] text-center text-lg lg:text-3xl">What Customers Say About Us</h2>
    <p class="text-sm text-center lg:text-lg">Stay updated with our groundbreaking research discoveries and scientific publications</p>
    <div class="md:flex gap-3">
      <div class="bg-[#FEFEFF] p-2  shadow-md my-3">
        <i class="lg:text-lg">“Intellitoggle cut our launch risk dramatically. We ship confidently every day.”</i>
        <div class="flex items-center my-2 gap-2">
          <img src="/Img1.png" alt="dp" />
          <p class="text-[#121316] font-bold grid text-sm lg:text-lg">Eng. Chima Umeh<span class="text-[#1A1A1A] font-normal text-xs lg:text-base">CTO, Nova</span></p>
        </div>
      </div>
      <div class="bg-[#FEFEFF] p-2  shadow-md my-3">
        <i class="lg:text-lg">“Our PMs now control rollouts without waiting on dev cycles. Huge win.”</i>
        <div class="flex items-center my-2 gap-2">
          <img src="/Img2.png" alt="dp" />
          <p class="text-[#121316] font-bold grid text-sm lg:text-lg">John Kennedy<span class="text-[#1A1A1A] font-normal text-xs lg:text-base">Head of Product, EdgeFlow</span></p>
        </div>
      </div>
      <div class="bg-[#FEFEFF] p-2  shadow-md my-3">
        <i class="lg:text-lg">“Experiments are painless and data-driven. Engagement up 12% in two weeks.”</i>
        <div class="flex items-center my-2 gap-2">
          <img src="/Img3.png" alt="dp" />
          <p class="text-[#121316] font-bold grid text-sm lg:text-lg">Dan Henry<span class="text-[#1A1A1A] font-normal text-xs lg:text-base">Software Engineer, Nova</span></p>
        </div>
      </div>
    </div>
  </section>

  <section class="my-5 py-7">
    <div class="bg-linear-to-r from-[#42489E] to-[#42489E] w-fit mx-auto md:w-2xl px-4 py-3 rounded-lg md:py-10">
      <h2 class="font-medium text-sm text-white text-center md:text-xl lg:text-2xl">
        Launch Features Confidently With AI Driven Flags
      </h2>
      <p class="text-xs text-center text-white md:text-base lg:text-lg">Get access now at $1/month, scale as your team grows</p>
      <div class="flex gap-2 w-fit mx-auto my-3">
        <button class="bg-[#F9A71E] px-4 text-[#42389E] font-bold text-sm rounded-sm md:text-lg lg:text-xl">Start for $1/mo</button>
        <button class="border border-[#FF99AA71] px-4 text-[#F9A71E] font-bold text-sm rounded-sm md:text-lg lg:text-xl">Join AI Early Access</button>
      </div>
    </div>
  </section>
  <section class="bg-[#E6E7F3] px-2 py-7">
    <div class="grid grid-cols-2 gap-5 md:flex md:justify-between">
      <div class="space-y-1">
        <img src="/Logo1.png" alt="Logo" class="w-25 md:w-35 lg:w-45" />
        <p class="text-xs font-light md:text-sm lg:text-lg">Intelli Toggle is built by AORTEM, a company focused on powering scalable, multi-platform developer tools.
        </p>
        <img src="/Github.png" alt="Github" />
      </div>
      <div class="space-y-1">
        <p class="text-[#263238] font-semibold text-sm lg:text-lg">Company</p>
        <p class="text-[#263238] font-light text-xs md:text-sm lg:text-lg">Pricing</p>
        <p class="text-[#263238] font-light text-xs md:text-sm lg:text-lg">Doc</p>
        <p class="text-[#263238] font-light text-xs md:text-sm lg:text-lg">About Us</p>
      </div>
      <div class="space-y-1">
        <p class="text-[#263238] font-semibold text-sm lg:text-lg">Resources</p>
        <p class="text-[#263238] font-light text-xs md:text-sm lg:text-lg">Why IntelliToggle is different</p>
        <p class="text-[#263238] font-light text-xs md:text-sm lg:text-lg">Customer Support</p>
        <p class="text-[#263238] font-light text-xs md:text-sm lg:text-lg">Terms & Conditions</p>
        <p class="text-[#263238] font-light text-xs md:text-sm lg:text-lg">Privacy Policy</p>
      </div>
      <div>
        <p class="text-sm text-[#263238] font-semibold lg:text-lg">Subscribe to Newsletter</p>
        <form class="flex">
          <input placeholder="Enter email address" class="bg-white w-30 text-xs md:text-sm md:w-40" />
          <button class="bg-[#42389E] text-white font-semibold rounded-br-md rounded-tr-md px-2">Join</button>
        </form>
      </div>
      
    </div>
  </section>
    
</template>


<script setup>
import { ref } from "vue";

const isSidebarOpen = ref(false);

function toggleSidebar() {
  isSidebarOpen.value = !isSidebarOpen.value;
}
</script>

<style scoped>
/* Slide animation for right sidebar */
.slide-right-enter-active,
.slide-right-leave-active {
  transition: transform 0.3s ease;
}
.slide-right-enter-from {
  transform: translateX(100%);
}
.slide-right-leave-to {
  transform: translateX(100%);
}
</style>
