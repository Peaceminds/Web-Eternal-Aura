<template>
  <div>
    <Header />
    <Banner />
    <Features />
    <Video />
    <!-- <CallToAction /> -->
    <!-- <CallToActionTwo /> -->
    <Pricing />
    <Testimonial />
    <Brands />
    <Counter />
    <!-- <Screenshots /> -->
    <!-- <Faq /> -->
    <!-- <BlogHome /> -->
    <Subscribe />
    <Footer />
  </div>
</template>
<script>
  import Header from "~/components/Header.vue";
  import Banner from "~/components/Banner.vue";
  import Features from "~/components/Features.vue";
  import Video from "~/components/Video.vue";
  import CallToAction from "~/components/CallToAction.vue";
  import CallToActionTwo from "~/components/CallToActionTwo.vue";
  import Pricing from "~/components/Pricing.vue";
  import Testimonial from "~/components/Testimonial.vue";
  import Brands from "~/components/Brands.vue";
  import Counter from "~/components/Counter.vue";
  import Screenshots from "~/components/Screenshots.vue";
  import Faq from "~/components/Faq.vue";
  import BlogHome from "~/components/BlogHome.vue";
  import Subscribe from "~/components/Subscribe.vue";
  import Footer from "~/components/Footer.vue";
  export default {
    components: {
      Header,
      Banner,
      Features,
      Video,
      CallToAction,
      CallToActionTwo,
      Pricing,
      Testimonial,
      Brands,
      Counter,
      Screenshots,
      Faq,
      BlogHome,
      Subscribe,
      Footer,

    }
  }
</script>
