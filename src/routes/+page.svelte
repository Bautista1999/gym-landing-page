<script>
  import Hero from '$lib/components/Hero.svelte';
  import Services from '$lib/components/Services.svelte';
  import Pricing from '$lib/components/Pricing.svelte';
  import Testimonials from '$lib/components/Testimonials.svelte';
  import Footer from '$lib/components/Footer.svelte';
</script>

<svelte:head>
  <title>FitPro Gym - Transform Your Body, Transform Your Life</title>
  <meta name="description" content="Join FitPro Gym and start your fitness transformation today. State-of-the-art equipment, expert trainers, and flexible membership plans." />
  <style>
    html {
      scroll-behavior: smooth;
    }
  </style>
</svelte:head>

<main class="min-h-screen">
  <!-- Hero Section -->
  <Hero />
  
  <!-- Services Section -->
  <Services />
  
  <!-- Pricing Section -->
  <Pricing />
  
  <!-- Testimonials Section -->
  <Testimonials />
  
  <!-- Footer -->
  <Footer />
</main>

<style>
  :global(body) {
    margin: 0;
    padding: 0;
    overflow-x: hidden;
  }
  
  :global(section) {
    scroll-margin-top: 80px;
  }
  
  main {
    display: flex;
    flex-direction: column;
  }
</style>