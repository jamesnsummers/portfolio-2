<template>
  <div class="nav">
    <p>developer // writer \\ musician</p>
    <ul>
      <li>home</li>
      <li>projects</li>
      <li>resume</li>
      <li>contact</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'Nav',
}
</script>

<style scoped lang="scss">
p {
  font-size: 22px;
  margin: 50px auto 0;
  width: fit-content;
}
ul {
  display: block;
  margin: 50px auto 0;
  padding: 0;
  width: fit-content;
  li {
    cursor: pointer;
    display: inline-block;
    font-size: 22px;
    list-style: none;
    margin: 0 22px;
  }
}
</style>
