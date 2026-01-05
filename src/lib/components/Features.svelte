<script lang="ts">
  const features = [
    {
      title: "Smart Workout Schedule",
      description: "Daily personalized workouts based on your progression and recovery.",
      image: "/images/screenshot-workout.png",
      align: "left"
    },
    {
      title: "Precision Nutrition",
      description: "Macro-perfect meal plans that adjust to your daily activity.",
      image: "/images/screenshot-diet.png",
      align: "right"
    },
    {
      title: "Track Your Journey",
      description: "Visualize your progress with detailed analytics and insights.",
      image: "/images/screenshot-progress.png",
      align: "left"
    }
  ];
</script>

<section class="py-24 relative">
  <div class="container mx-auto px-6">
    <div class="text-center mb-20">
      <h2 class="text-3xl md:text-5xl font-bold mb-4">COMPLETE <span class="text-primary">ECOSYSTEM</span></h2>
      <p class="text-gray-400 max-w-2xl mx-auto">Everything you need to reach your peak performance, all in one seamless application.</p>
    </div>

    <div class="space-y-32">
      {#each features as feature, i}
        <div class="flex flex-col md:flex-row items-center gap-12 md:gap-24 {feature.align === 'right' ? 'md:flex-row-reverse' : ''}">
          <!-- Image Side -->
          <div class="flex-1 relative group">
            <div class="absolute inset-0 bg-gradient-to-tr from-primary/20 to-transparent blur-3xl opacity-0 group-hover:opacity-100 transition-opacity duration-500"></div>
            <img 
              src={feature.image} 
              alt={feature.title}
              class="relative z-10 w-[280px] mx-auto rounded-[2.5rem] border-8 border-neutral-800 shadow-2xl transform transition-transform duration-500 group-hover:scale-105 group-hover:-rotate-2"
            />
          </div>
          
          <!-- Content Side -->
          <div class="flex-1 text-center md:text-left">
            <div class="inline-block px-4 py-1 rounded-full bg-neutral-800 border border-white/10 text-primary text-sm font-medium mb-6">
              0{i + 1}
            </div>
            <h3 class="text-3xl md:text-4xl font-bold mb-6">{feature.title}</h3>
            <p class="text-lg text-gray-400 leading-relaxed mb-8">
              {feature.description}
            </p>
            <button class="text-white hover:text-primary font-medium flex items-center gap-2 mx-auto md:mx-0 transition-colors">
              Learn more 
              <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-5 h-5">
                <path stroke-linecap="round" stroke-linejoin="round" d="M13.5 4.5 21 12m0 0-7.5 7.5M21 12H3" />
              </svg>
            </button>
          </div>
        </div>
      {/each}
    </div>
  </div>
</section>
