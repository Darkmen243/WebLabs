<template>
  <div id="app">
    <CheckBox v-model="switch1"></CheckBox>
    <SwitchButton v-model="switch1"></SwitchButton>
   </div>
  </template>
<script>
import SwitchButton from './components/SwitchButton.vue'
import CheckBox from './components/Checkbox.vue'
export default {
  name: 'App',
  components: {
   SwitchButton,
   CheckBox
  },
  data:
    function () {
      return {
        switch1:false
      };
    }
}
</script>

<style>
#app {
  font-family: Lato, sans-serif;
}

#app .switch-button {
  margin: 10px 0;
}
</style>
