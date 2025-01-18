<template>
  <div class="home-page" :style="backgroundStyle">
    <!-- Header -->
    <Header />

    <!-- Main Content -->
    <main class="flex-grow bg-opacity-75 text-white py-16">
      <div class="container mx-auto text-center">
        <h2 class="text-4xl font-bold mb-8">Welcome to Lucidium Studios</h2>
        <p class="text-lg mb-8">
          At Lucidium Studios, we bring innovative and immersive games to life.
          Our team of creative developers and designers is dedicated to making your gaming experiences unforgettable.
        </p>
        <div class="flex justify-center space-x-6">
          <a href="/portfolio" class="px-6 py-3 bg-yellow-500 text-white rounded-lg hover:bg-yellow-400 transition duration-300">View Portfolio</a>
          <a href="/contact" class="px-6 py-3 border-2 border-yellow-500 text-yellow-500 rounded-lg hover:bg-yellow-100 transition duration-300">Get in Touch</a>
        </div>
      </div>
    </main>

    <!-- Footer -->
    <Footer />
  </div>
</template>

<script>
import Header from '~/components/Header.vue'
import Footer from '~/components/Footer.vue'

export default {
  name: 'IndexPage',
  components: {
    Header,
    Footer
  },
  data() {
    return {
      backgroundStyle: {
        backgroundImage: 'url("/images/lucidium.png")', // Ensure this path is correct
        backgroundSize: 'cover',
        backgroundPosition: 'center',
        backgroundAttachment: 'fixed', 
        minHeight: '100vh'
      }
    }
  }
}
</script>

<style scoped>
/* Additional styling for your page */
.home-page {
  height: 100vh;
  display: flex;
  flex-direction: column;
}

main {
  flex-grow: 1; /* This makes the main content grow to fill the available space */
}
</style>
