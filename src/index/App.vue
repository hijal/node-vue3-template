<template>
  <video-background :sources="['/video/timelapse.mp4']" img="/img/bg.jpeg">
    <!-- Our Nav Bar Component and Side Menu -->
    <nav-bar />
    <!-- Main Content and Buttons -->
    <intro-section-block />
    <!-- Footer -->
    <footer-section />
  </video-background>
</template>

<script>
// Import our components from component directory
import NavBar from "./components/Nav/NavBar.vue";
import IntroSection from "./components/Intro/IntroSection.vue";
import Footer from "./components/Footer.vue";

// Use our components in our App.vue template
export default {
  components: {
    introSectionBlock: IntroSection,
    navBar: NavBar,
    footerSection: Footer,
  },
};
</script>
