<template>
  <div id="mytitle">
  </div>
</template>

<script>

  export default {
    name: 'Mytitle',
    methods: {
    }
  }
</script>
    
<style>
#mytitle {
    position: fixed;
    top: 0;
    right: 0;
    z-index: 1000;
    width: 100%;
    height: 32px;
    background-color: rgb(53, 52, 52);
    -webkit-app-region: drag;
}
</style>