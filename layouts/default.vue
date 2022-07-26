<template>
  <Nuxt />
</template>

<style>
@font-face {
font-family: "SF Pro";
src: url("../static/fonts/SFPRODISPLAYREGULAR.OTF");
src: url("../static/fonts/SFPRODISPLAYREGULAR.OTF") format("woff")
}

@font-face {
font-family: "SF Pro Bold";
src: url("../static/fonts/SFPRODISPLAYBOLD.OTF");
src: url("../static/fonts/SFPRODISPLAYBOLD.OTF") format("woff")
}

html, body{
  margin: 0;
  padding: 0;
  font-size: 1rem;
}
body{
  font-family: SF Pro;
  color: #ffffff;
  scroll-behavior: smooth;
}
*{
  box-sizing: border-box;
}
h1,h2,h3{
  line-height: 1.2;
  margin: 0;
}
@media screen and (max-width: 1400px) {
  html{
    font-size: .8rem;
  }
}
@media screen and (max-width: 600px) {
  html, body{
    font-size: .7rem;
  }
}
</style>