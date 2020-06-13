<template>
  <div class="dm-toggle">
    <label v-on:mouseup="toggleDarkMode" class="switch">
      <input type="checkbox">
      <span class="slider round"></span>
    </label>
    <p>dark mode</p>
  </div>
</template>

<script>
export default {
  name: 'Toggle',
  methods: {
    toggleDarkMode: function() {
      document.documentElement.classList.toggle('dm');
    }
  }
}
</script>

<style scoped lang="scss">
.dm-toggle {
  position: absolute;
  right: 1em;
  top: 1em;
  width: 5em;
}
.switch {
  display: inline-block;
  height: 34px;
  position: relative;
  width: 60px;
  input {
    height: 0;
    opacity: 0;
    width: 0;
  }
}
.slider {
  background-color: #ccc;
  border-radius: 34px;
  bottom: 0;
  cursor: pointer;
  left: 0;
  position: absolute;
  right: 0;
  top: 0;
  transition: .4s;
  -webkit-transition: .4s;
  &::before {
    background-color: #fff;
    border-radius: 50%;
    bottom: 4px;
    content: "";
    height: 26px;
    left: 4px;
    position: absolute;
    transition: .4s;
    width: 26px;
    -webkit-transition: .4s;
  }
}
input:checked {
  + .slider {
    background-color: #9FD6AE;
  }
  + .slider:before {
    transform: translateX(26px);
    -ms-transform: translateX(26px);
    -webkit-transform: translateX(26px);
  }
}
input:focus + .slider {
  box-shadow: 0 0 1px #9FD6AE;
}
</style>
