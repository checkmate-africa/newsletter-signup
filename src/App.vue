<template>
  <div id="app">
    <router-view />
  </div>
</template>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Darker+Grotesque:wght@300;400;500;600;700;800;900&family=Mandali&display=swap");

html,
body {
  margin: 0;
  height: 100%;
}

* {
  box-sizing: border-box;
  font-family: "Mandali", sans-serif;
}

h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: "Darker Grotesque", sans-serif;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  height: 100%;

  --col-primary: #65bbed;
  --col-white: #ffffff;
  --col-black: #0F0F0F;
  --col-secondary-grey: rgba(158, 158, 158, 1);
}
</style>
