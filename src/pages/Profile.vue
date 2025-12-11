<template>
  <div class="min-h-screen flex flex-col">
    <Header />
    
    <!-- Desktop Profile Section -->
    <div class="hidden md:block flex-1 bg-white">
      <div class="container mx-auto px-8 py-12 max-w-7xl">
        <!-- Title Section -->
        <div class="mb-12">
          <h1 class="text-5xl font-bold text-gray-800 mb-2">AMISHA NABILA WIGUNA</h1>
          <p class="text-gray-600 text-lg">11231008 - INFORMATIKA</p>
        </div>
        
        <!-- Main Content: Left Description + Skills, Right Photo -->
        <div class="grid grid-cols-2 gap-12 pb-12">
          <!-- Left Section: Description and 3 Skills Horizontal -->
          <div class="flex flex-col">
            <!-- Description -->
            <div class="mb-12">
              <div class="text-gray-700 text-base leading-relaxed space-y-4">
                <p>
                  I'm a passionate developer dedicated to creating beautiful and functional web experiences.
                  With expertise in modern frameworks and responsive design, I craft digital solutions
                  that make a difference.
                </p>
                <p>
                  My journey in web development started with a curiosity about how websites work,
                  and it has evolved into a career dedicated to building scalable and user-friendly applications.
                </p>
                <p>
                  I believe in continuous learning and staying updated with the latest trends in web development.
                </p>
              </div>
            </div>

            <!-- 3 Skills Horizontal - Larger -->
            <div class="grid grid-cols-3 gap-6">
              <!-- Skill 1 -->
              <div class="flex flex-col items-center p-6 bg-white rounded-lg border-2 border-gray-300 shadow-sm">
                <div class="w-40 h-40 bg-green-100 rounded-lg flex items-center justify-center shadow-md mb-4 border border-green-300 text-6xl">
                  ⚡
                </div>
                <p class="text-gray-800 font-bold text-lg text-center">Vue 3</p>
                <p class="text-gray-600 text-sm text-center mt-1">Progressive Framework</p>
              </div>

              <!-- Skill 2 -->
              <div class="flex flex-col items-center p-6 bg-white rounded-lg border-2 border-gray-300 shadow-sm">
                <div class="w-40 h-40 bg-blue-100 rounded-lg flex items-center justify-center shadow-md mb-4 border border-blue-300 text-6xl">
                  🎨
                </div>
                <p class="text-gray-800 font-bold text-lg text-center">Tailwind</p>
                <p class="text-gray-600 text-sm text-center mt-1">CSS Framework</p>
              </div>

              <!-- Skill 3 -->
              <div class="flex flex-col items-center p-6 bg-white rounded-lg border-2 border-gray-300 shadow-sm">
                <div class="w-40 h-40 bg-yellow-100 rounded-lg flex items-center justify-center shadow-md mb-4 border border-yellow-300 text-6xl">
                  💻
                </div>
                <p class="text-gray-800 font-bold text-lg text-center">JavaScript</p>
                <p class="text-gray-600 text-sm text-center mt-1">Programming Language</p>
              </div>
            </div>
          </div>

          <!-- Right Section: Photo -->
          <div class="flex flex-col items-center justify-start">
            <!-- Photo -->
            <div class="w-80 h-80 rounded-lg overflow-hidden shadow-xl border-4 border-gray-300">
              <img
                src="@/assets/amisha.jpg"
                alt="Profile"
                class="w-full h-full object-cover"
              />
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Mobile Profile Section - Name, About, Skills -->
    <div class="md:hidden flex-1 bg-white py-8">
      <div class="container mx-auto px-4">
        <!-- Title Section -->
        <div class="mb-8">
          <h1 class="text-3xl font-bold text-gray-800 mb-1">AMISHA NABILA WIGUNA</h1>
          <p class="text-gray-600 text-sm">11231008 - INFORMATIKA</p>
        </div>

        <!-- Description Section -->
        <div class="mb-8">
          <div class="text-gray-700 text-sm leading-relaxed space-y-3">
            <p>
              I'm a passionate developer dedicated to creating beautiful and functional web experiences.
              With expertise in modern frameworks and responsive design, I craft digital solutions
              that make a difference.
            </p>
            <p>
              My journey in web development started with a curiosity about how websites work,
              and it has evolved into a career dedicated to building scalable and user-friendly applications.
            </p>
            <p>
              I believe in continuous learning and staying updated with the latest trends in web development.
            </p>
          </div>
        </div>

        <!-- Skills Vertical Stack -->
        <div class="space-y-6">
          <!-- Skill 1 -->
          <div class="flex flex-col items-center p-6 bg-white rounded-lg border-2 border-gray-300 shadow-sm">
            <div class="w-28 h-28 bg-green-100 rounded-lg flex items-center justify-center shadow-md mb-3 border border-green-300 text-5xl">
              ⚡
            </div>
            <p class="text-gray-800 font-bold text-lg">Vue 3</p>
            <p class="text-gray-600 text-xs">Progressive Framework</p>
          </div>

          <!-- Skill 2 -->
          <div class="flex flex-col items-center p-6 bg-white rounded-lg border-2 border-gray-300 shadow-sm">
            <div class="w-28 h-28 bg-blue-100 rounded-lg flex items-center justify-center shadow-md mb-3 border border-blue-300 text-5xl">
              🎨
            </div>
            <p class="text-gray-800 font-bold text-lg">Tailwind CSS</p>
            <p class="text-gray-600 text-xs">CSS Framework</p>
          </div>

          <!-- Skill 3 -->
          <div class="flex flex-col items-center p-6 bg-white rounded-lg border-2 border-gray-300 shadow-sm">
            <div class="w-28 h-28 bg-yellow-100 rounded-lg flex items-center justify-center shadow-md mb-3 border border-yellow-300 text-5xl">
              💻
            </div>
            <p class="text-gray-800 font-bold text-lg">JavaScript</p>
            <p class="text-gray-600 text-xs">Programming Language</p>
          </div>
        </div>
      </div>
    </div>

    <Footer />
  </div>
</template>

<script setup>
import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'

defineOptions({ name: 'Profile' })
</script>
