<template>
  <router-view/>
</template>

<style>


#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  background-color: #08454E;
  font-family: 'Rubik', sans-serif;
}
.container {
  background-color: white;
  width: 1200px;
  margin: 0 auto;
  overflow: auto;
  min-height: 1200px;
  padding: 60px;
}
.btn {
  background: #258FAF;
  color: #fff;
  border: none;
  border-bottom: 4px solid #105D74;
  padding: 10px 20px;
  cursor: pointer;
  text-decoration: none;
  font-size: 15px;
}

.btn:hover {
  transform: scale(1.05);
}


.danger{
  color: red;
}

h5{
  font-size: 18px;
  }

.contact-input-fields{
  float: left;
  height: auto;
  margin-top: 30px;
  padding-left: 30px;
}
</style>
