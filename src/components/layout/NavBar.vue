<template>
  <div id="nav">

    <router-link to="/" id="logo_url"><img :src="logo" id="logo" :alt="alt"></router-link>
    <router-link to="/">Home</router-link>
    <router-link to="/about">About</router-link>
  </div>
</template>

<script>
export default {

  name: 'Navbar',
  props: ["logo", "alt"]

}
</script>

<style scoped>
#nav {
  background-color: #222;
  border-bottom: 4px solid #111;
  padding: 15px 50px;
  display: flex;
  justify-content: flex-end;
  align-content: center;
}

#nav #logo_url {
  margin: auto;
  margin-left: 0;
}

 #logo{
  width: 40px;
  height: 40px;
}

#nav a{
  color: #FCBA03;
  text-decoration:none;
  margin: 12px;
  transform: .5s;

}

#nav a:hover{
  color: #fff;

}



</style>