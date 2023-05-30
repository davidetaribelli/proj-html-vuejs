<script>
import PageHeader from './components/PageHeader.vue';
import PageMain from './components/PageMain.vue';
import PageFooter from './components/PageFooter.vue';

export default {
  components: {
    PageHeader,
    PageMain,
    PageFooter
  },
  data() {
    return {
      linkList: [
        { link: "Home" },
        { link: "About Us" },
        { link: "Portfolio" },
        { link: "Our Process" },
        { link: "Pricing" },
        { link: "Blog" },
        { link: "Contact" },
      ]
    }
  }
}
</script>

<template>
  <header>
    <PageHeader :linkArray="linkList" />
  </header>
  <main>
    <PageMain />
  </main>
  <footer>
    <PageFooter />
  </footer>
</template>

<style lang="scss">
@use './style/general.scss' as *;

header {
  background-image: url(./assets/img/banner-bg.png);
  background-repeat: no-repeat;
  background-size: cover;
}

main {
  margin-top: 250px;
}
</style>
