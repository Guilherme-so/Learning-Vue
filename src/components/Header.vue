<template>
  <header class="header">
    <div>
      <h1 class="heading">{{ logo }}</h1>
    </div>

    <nav>
      <ul class="navlinks">
        <li class="link"><a href="#">Home</a></li>
        <li class="link"><a href="#">About</a></li>
        <li class="link"><a href="#">Contact</a></li>
        <li class="link" v-show="logado">
          <a href="#">{{ perfil }}</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  props: {
    logo: String,
    logado: Boolean,
    perfil: String,
  },
};
</script>

<style scoped>
.header {
  display: flex;
  justify-content: space-around;
  align-items: center;
  background-color: #999;
}

.heading {
  color: turquoise;
}

.navlinks {
  display: flex;
}

.link {
  margin-right: 20px;
  list-style: none;
  cursor: pointer;
  transition: 1s ease-in-out;
}

.link:hover::after {
  content: "";
  display: inline-block;
  width: 100%;
  height: 1px;
  transform: translateY(-4px);
  background-color: turquoise;
}

.link a:hover {
  transform: translateY(-5px);
  color: turquoise;
}

.link:hover {
  transform: translateY(-5px);
  color: turquoise;
}
</style>
