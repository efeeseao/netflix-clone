<template>
  <div id="app">
    <Header />
    <Controls />
    <Tabs />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header';
import Controls from './components/Section/Controls.component';
import Tabs from './components/Main/Tabs';
import Footer from './components/Footer/Footer.component';

export default {
  name: 'app',
  components: {
    Header,
    Controls,
    Tabs,
    Footer
  }
}
</script>

<style>
  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }

  body {
    font-family: 'Arial', sans-serif;
    -webkit-font-smoothing: antialiased;
    background: #000;
    color: #999;
  }

  ul {
    list-style: none;
  }

  h1,
  h2,
  h3,
  h4 {
    color: #fff;
  }

  a {
    color: #fff;
    text-decoration: none;
  }

  p {
    margin: 0.5rem 0;
  }

  img {
    width: 100%;
  }
</style>
