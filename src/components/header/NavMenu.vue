<template>
  <div id="NavMenuContainer">
      
    <img id="logo" width="181" height="43" src="@/assets/MibuscaLogo.png"/>

    <nav>
      <ul class="nav">
          <li class="nav-item">
            <a class="nav-link active" href="#">Inicio</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Quem somos</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Cadastre-se</a>
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
  width: 100%;
  height: 70px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

#NavMenuContainer nav {
  display: flex;
  justify-content: flex-center;
  margin-right: 110px;
}

img {
  margin-left: 110px;
}

ul li a {
  color: #002b5b;
}

ul li a:hover {
  font-weight: bolder;
  text-decoration: underline;
}
</style>
