<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link>
      <router-link to="/about">About</router-link>
    </div>
    <router-view/>
  </div>
</template>

<style>
:root{
  --link-height: 48px;
}

body, html{
  padding: 0;
  margin: 0;
  background-color: #ecf0f1;
}

#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color:#34495e;
}
#nav {
  height: var(--link-height);
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #16a085;
}

#nav a {
  font-weight: bold;
  color: #34495e;
  padding: 0px 15px;
  height: var(--link-height);
  line-height: var(--link-height);
  text-decoration: none;
}

#nav a:hover {
  background-color: #1abc9c;
}

#nav a.router-link-exact-active {
  background-color: #1abc9c;
}
</style>
