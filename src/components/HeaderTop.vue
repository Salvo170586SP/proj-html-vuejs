<template>
  <div id="header-top" class="py-3">
    <div class="container">
      <nav class="navbar navbar-expand-lg  ">
        <div class="container-fluid">
          <img src="../assets/images/white-logo-2.png" alt="logo" />
          <div class="collapse navbar-collapse d-flex justify-content-end my-4" id="navbarNav">
            <ul class="d-flex justify-content-end p-0 mb-0">
              <li v-for="(item, index) in items" :key="index">
                <a :class="{ active: item.active }" href="#">{{ item.text }}</a>
              </li>
            </ul>
          </div>
          <div class=" ">
            <a class="bg-blue" href="#">Sing-in</a>
          </div>
        </div>
      </nav>
    </div>
  </div>
</template>

<script>
export default {
  nome: "HeaderTop",
  props: ["items"],
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

a {
  border-radius: 25px;
  padding: 10px 15px;

  &.active {
    color: $red-span;
  }
}

a.bg-blue {
  background: linear-gradient(270deg,
      rgba(2, 0, 36, 1) 0%,
      rgba(36, 36, 115, 1) 0%,
      rgba(0, 160, 186, 1) 100%);

  &.bg-blue:hover {
    background: linear-gradient(90deg,
        rgba(0, 29, 36, 1) 0%,
        rgba(100, 133, 145, 1) 0%,
        rgba(227, 18, 47, 1) 100%);
    color: white;
  }
}
</style>