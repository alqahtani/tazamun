<template>
  <div id="app" dir="rtl" class="">
    <Header />
    <Main />
    <Archive />
    <Newsletter />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/header"
import Main from "./components/main"
import Archive from "./components/archive"
import Newsletter from "./components/newsletter"
import Footer from "./components/footer"

export default {
  name: "app",
  components: {
    Header,
    Main,
    Archive,
    Newsletter,
    Footer,
  },
}
</script>

<style></style>
