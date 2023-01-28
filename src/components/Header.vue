<template>
  <header class="header">
    <div>
      <h1 class="heading">Learning Vue</h1>
    </div>

    <nav>
      <ul class="navlinks">
        <li class="link">Home</li>
        <li class="link">About</li>
        <li class="link">Contact</li>
      </ul>
    </nav>
  </header>
</template>

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
.link:hover {
  transform: translateY(-5px);
  color: turquoise;
}
</style>
