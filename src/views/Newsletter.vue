<template>
  <div id="newsletter">
    <Header />
    <Form />
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import Header from "@/components/Header.vue";
import Footer from "@/components/Footer.vue";
import Form from "@/components/Form.vue";

export default {
  name: "Home",
  components: {
    Header,
    Footer,
    Form,
  },
};
</script>

<style lang="scss" scoped>
  #newsletter {
    height: 100%;
    display: flex;
    flex-flow: column;
    justify-content: space-between;
    padding: 2rem 7%;
  }
</style>
