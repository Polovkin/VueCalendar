<template lang="pug">

  #app.container
    Header-app
    main.users.section
      AsideNav.users__aside
      section.users__content
        h1 2

</template>

<script>
import AsideNav from "./components/app/Aside-nav.vue";
import HeaderApp from "./components/app/Header-app.vue";
export default {
  name: 'App',
  components: {HeaderApp, AsideNav},
  data() {
    return {

    }
  },
};

</script>

<style lang="scss">

</style>
