<template>
  <div class="box-container">
    <div class="header bg-primary">
        <Header />
    </div>
    <div class="main container">
        <Main />
    </div>
    <div class="footer bg-secondary">
        <Footer />
    </div>
  </div>
</template>

<style scoped>
.header {
  grid-area: header;
}
.main {
  grid-area: main;
}
.footer {
  grid-area: footer;
}
.box-container {
  display: grid;
  grid-template-areas:
    "header"
    "main"
    "footer";
  height: 100vh;
  grid-template-rows: 50px calc(100% - 100px) 50px;
}
.container {
  margin-left: auto;
  margin-right: auto;
}
</style>