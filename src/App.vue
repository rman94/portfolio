<template>

  <v-app>
    <Header></Header>
    <test></test>

    <Portfolio></Portfolio>

  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld';
import Header from './components/Header'
import Portfolio from './components/Portfolio'
import Navigation2 from'./components/Navigation2'
import test from'./components/test'

export default {
  name: 'App',
  components: {
    HelloWorld,
    Header,
    Portfolio,
    Navigation2,
    test
  },
  data: () => ({
    //
  }),
};
</script>
