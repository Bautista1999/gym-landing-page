<script>
  // No script logic needed for this basic hero component
</script>

<section class="relative min-h-screen flex items-center justify-center overflow-hidden bg-gray-900">
  <!-- Background Image Overlay -->
  <div class="absolute inset-0 bg-black/60 z-10"></div>
  
  <!-- Background Image -->
  <div class="absolute inset-0 bg-gradient-to-br from-gray-900 via-gray-800 to-black">
    <!-- Fallback gradient background since we don't have generated images yet -->
    <div class="absolute inset-0 opacity-30 bg-[url('data:image/svg+xml,%3Csvg width="60" height="60" viewBox="0 0 60 60" xmlns="http://www.w3.org/2000/svg"%3E%3Cg fill="none" fill-rule="evenodd"%3E%3Cg fill="%23ffffff" fill-opacity="0.1"%3E%3Ccircle cx="30" cy="30" r="4"/%3E%3C/g%3E%3C/g%3E%3C/svg%3E')]"></div>
  </div>

  <!-- Hero Content -->
  <div class="relative z-20 max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
    <div class="max-w-4xl mx-auto">
      <!-- Main Headline -->
      <h1 class="text-4xl sm:text-5xl md:text-6xl lg:text-7xl font-bold text-white mb-6 leading-tight">
        Transform Your <span class="text-transparent bg-clip-text bg-gradient-to-r from-orange-400 to-red-500">Body</span>,
        <br class="hidden sm:block">
        Transform Your <span class="text-transparent bg-clip-text bg-gradient-to-r from-orange-400 to-red-500">Life</span>
      </h1>

      <!-- Subheading -->
      <p class="text-lg sm:text-xl md:text-2xl text-gray-300 mb-12 max-w-3xl mx-auto leading-relaxed">
        Begin your fitness journey with expert trainers, state-of-the-art equipment, and a supportive community. 
        Achieve your goals and unlock your potential with personalized workout plans designed for lasting results.
      </p>

      <!-- CTA Buttons -->
      <div class="flex flex-col sm:flex-row gap-4 sm:gap-6 justify-center items-center">
        <!-- Primary CTA -->
        <button class="w-full sm:w-auto px-8 py-4 bg-gradient-to-r from-orange-500 to-red-500 text-white font-bold text-lg rounded-full hover:from-orange-600 hover:to-red-600 transform hover:scale-105 transition-all duration-300 shadow-lg hover:shadow-xl">
          Start Free Trial
        </button>

        <!-- Secondary CTA -->
        <button class="w-full sm:w-auto px-8 py-4 bg-transparent border-2 border-white text-white font-bold text-lg rounded-full hover:bg-white hover:text-gray-900 transition-all duration-300 shadow-lg hover:shadow-xl">
          View Membership
        </button>
      </div>

      <!-- Additional Info -->
      <p class="text-gray-400 text-sm mt-8">
        No commitment required • Cancel anytime • Join 10,000+ members
      </p>
    </div>
  </div>

  <!-- Decorative Elements -->
  <div class="absolute bottom-0 left-0 right-0 h-32 bg-gradient-to-t from-black/80 to-transparent z-15"></div>
  
  <!-- Scroll Indicator -->
  <div class="absolute bottom-8 left-1/2 transform -translate-x-1/2 z-20">
    <div class="w-6 h-10 border-2 border-white/50 rounded-full flex justify-center">
      <div class="w-1 h-3 bg-white/70 rounded-full mt-2 animate-pulse"></div>
    </div>
  </div>
</section>

<style>
  /* Custom animations and transitions */
  @keyframes fadeInUp {
    from {
      opacity: 0;
      transform: translateY(30px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }

  h1 {
    animation: fadeInUp 1s ease-out;
  }

  p {
    animation: fadeInUp 1s ease-out 0.2s both;
  }

  .flex.flex-col.sm\\:flex-row {
    animation: fadeInUp 1s ease-out 0.4s both;
  }

  /* Responsive adjustments */
  @media (max-width: 640px) {
    section {
      min-height: 100vh;
      padding: 2rem 0;
    }
  }

  /* Button hover effects */
  button {
    position: relative;
    overflow: hidden;
  }

  button::before {
    content: '';
    position: absolute;
    top: 50%;
    left: 50%;
    width: 0;
    height: 0;
    background: rgba(255, 255, 255, 0.1);
    border-radius: 50%;
    transform: translate(-50%, -50%);
    transition: width 0.6s, height 0.6s;
  }

  button:hover::before {
    width: 300px;
    height: 300px;
  }
</style>