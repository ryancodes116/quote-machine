<template>
  <div id="app">
    <QuoteMachine />
  </div>
</template>

<script>
import QuoteMachine from "./components/QuoteMachine";

export default {
  name: "App",
  components: {
    QuoteMachine
  }
};
</script>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
</style>
