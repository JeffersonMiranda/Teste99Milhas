<template>
  <div id="NavMenuContainer"> 
   
    <img id="logo" class="img-fluid" src="@/assets/MibuscaLogo.png"/>
   
    <nav>
      <ul>
          <li>
            <a href="#">Inicio</a>
          </li>
          <li>
            <a href="#">Quem somos</a>
          </li>
          <li>
            <a href="#">Cadastre-se</a>
          </li>
      </ul>   
    </nav>

  </div>
</template>


<script>
export default {
  name: "NavMenu"
};
</script>

<style scoped>
#NavMenuContainer {
  padding: 0 120px;
  min-height: 70px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

nav {
  width: 350px;
}

ul {
  margin: 0;
  padding: 0;
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  list-style: none;
}

ul li a {
  color: #002b5b;
}

ul li a:hover {
  font-weight: bolder;
  text-decoration: underline;
}

@media (max-width: 640px) {
  #NavMenuContainer {
    flex-direction: column;
    justify-content: center;
    padding: 0;
  }
  nav {
    width: 100%;
  }
  ul {
    flex-direction: column;
    align-items: center;
  }
}
</style>
