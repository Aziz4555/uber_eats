<template>
  <NavBar></NavBar>
  <Main></Main>
  <div class="discover">
    <div class="discover_uber_eats">
      <a href="">
        <span class="partenaire">Découvrez comment Uber Eats et classe les offres des partenaires. </span>
        <span class="savoir_plus">En savoir plus</span>
      </a>
    </div>
  </div>
  <Footer></Footer>
</template>

<script>


import NavBar from "./components/NavBar";
import Main from "./components/Main";
import Footer from "./components/Footer";
export default {
  name: 'App',
  components: {
    Footer,
    Main,
    NavBar

  }
}
</script>

<style>

*{
  font-family: "Uber Move Medium",sans-serif;
}

.discover {
  padding: 0 40px;
  margin: 0 auto;
  box-sizing: border-box;
}

.discover span{
  font-size: 16px;
  line-height: 24px;
  font-weight: normal;
  color: #000000;
}

.discover_uber_eats {
  display: flex;
  justify-content: center;
  padding-top: 24px;
}

.discover_uber_eats a {
  color: black;
  text-decoration: none;
}

.savoir_plus{
  text-decoration: underline;
}


</style>
