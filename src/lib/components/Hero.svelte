<script lang="ts">
  // Images are in static/images, accessed via absolute paths
</script>

<section class="relative min-h-screen flex items-center justify-center overflow-hidden pt-20">
  <!-- Background Elements -->
  <div class="absolute top-0 left-1/2 -translate-x-1/2 w-[800px] h-[500px] bg-primary/20 blur-[120px] rounded-full pointer-events-none"></div>
  
  <div class="container mx-auto px-6 relative z-10 flex flex-col md:flex-row items-center gap-12">
    <!-- Text Content -->
    <div class="flex-1 text-center md:text-left space-y-8">
      <h1 class="text-5xl md:text-7xl font-bold leading-tight">
        TRAIN SMARTER <br/>
        <span class="text-primary">NOT HARDER</span>
      </h1>
      <p class="text-xl text-gray-400 max-w-lg mx-auto md:mx-0">
        AI-powered workout plans and nutrition schedules tailored exactly to your body and goals. The future of personal coaching is here.
      </p>
      
      <div class="flex flex-col sm:flex-row gap-4 justify-center md:justify-start">
        <button class="px-8 py-4 bg-primary text-black font-bold text-lg rounded-full hover:bg-opacity-90 transition-all transform hover:scale-105">
          Get Started Free
        </button>
        <button class="px-8 py-4 border border-white/20 hover:border-primary hover:text-primary font-bold text-lg rounded-full transition-all">
          View Demo
        </button>
      </div>
      
      <div class="flex items-center justify-center md:justify-start gap-8 pt-8 text-sm text-gray-500">
        <div class="flex items-center gap-2">
          <div class="w-2 h-2 rounded-full bg-primary"></div>
          <span>AI-Driven Analysis</span>
        </div>
        <div class="flex items-center gap-2">
          <div class="w-2 h-2 rounded-full bg-primary"></div>
          <span>Real-time Adaptations</span>
        </div>
      </div>
    </div>
    
    <!-- Hero Image -->
    <div class="flex-1 relative">
      <div class="relative z-10 transform md:rotate-[-5deg] hover:rotate-0 transition-all duration-500">
        <div class="absolute inset-0 bg-primary/20 blur-2xl -z-10 rounded-[3rem]"></div>
        <img 
          src="/images/screenshot-dashboard.png" 
          alt="AisyFit Dashboard" 
          class="w-[300px] mx-auto rounded-[2.5rem] border-8 border-neutral-900 shadow-2xl"
        />
      </div>
      
      <!-- Floating Elements (Optional decoration) -->
      <div class="absolute -top-10 -right-10 w-24 h-24 bg-neutral-800/80 backdrop-blur-md rounded-2xl p-4 border border-white/10 animate-bounce hidden md:block">
        <div class="text-primary text-2xl font-bold">540</div>
        <div class="text-xs text-gray-400">Calories Burned</div>
      </div>
    </div>
  </div>
</section>
