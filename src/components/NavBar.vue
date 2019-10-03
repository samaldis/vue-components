<template>
  <nav>
    <div class="navbar">
      <div class="nav--left">
        <h1>{{title[0].toUpperCase() + title.substr(1)}}</h1>
      </div>
      <div class="nav--button-container">
        <div class="nav--button">
          <h2>test</h2>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "NavBar",
  props: {
    title: String
  }
};
</script>

<style lang="scss">
nav {
  height: 40px;
  position: fixed;
  left: 0px;
  top: 0px;
  right: 0px;
  width: auto;
  height: auto;
  background: rgba(255, 255, 255, 0.5);
  box-shadow: 0 0 4px 5px rgba(0, 0, 0, 0.137);
  .navbar {
    width: 100vw;
    display: inline-flex;
    .nav--button-container {
      display: inline-block;
      height: 40px;
      .nav--button {
        display: block;
        background-color: #4f4f4f;
        color: white;
        transition: 0.5s;
        height: auto;
        padding-left: 2px;
        padding-right: 2px;
        position: fixed;
        min-width: 60px;
        right: 0;
        &:last-child {
          margin-right: 10px;
        }
        &:hover {
        background-color: #000000;
        }
      }
    }
    .nav--left {
      color: black;
      width: fit-content;
      display: inline-block;
      padding-left: 10px;
      text-align: left;
      align-content: center;
    }
  }
}
</style>