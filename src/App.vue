<template>
  <div id="app">
    <QuoteMachine />
  </div>
</template>

<script>
import QuoteMachine from './components/QuoteMachine';

export default {
  name: 'App',
  components: {
    QuoteMachine,
  },
};
</script>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

body {
  min-height: 100vh;
  background-image: url('./assets/mountains.jpg');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}
</style>
