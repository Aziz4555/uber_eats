<template>

  <div class="footer">

    <div class="content">

      <div class="content_flex">

        <div class="content_left">
          <div class="logo_uber_eats">
            <img src="../../src/assets/uber_eats_white.svg" role="img"/>
          </div>

          <div class="logo_application">

            <div class="logo_apple">
              <a href="https://apps.apple.com/us/app/uber-eats-food-delivery/id1058959277">
                <img src="../../src/assets/download_app_store.svg" role="img">
              </a>
            </div>

            <div class="space_16"></div>

            <div class="logo_google_play">
              <a href="https://play.google.com/store/apps/details?id=com.ubercab.eats">
                <img src="../../src/assets/download_google_play.png" role="img">
              </a>
            </div>

          </div>

        </div>


        <div class="content_middle">
          <ul>
            <li> <a href="https://help.uber.com/ubereats">Obtenir de l'aide</a> </li>

            <li> <a href="https://www.ubereats.com/restaurant/fr-FR/signup">Ajoutez votre restaurant</a> </li>

            <li> <a href="https://www.uber.com/fr/fr/deliver/">Devenez coursier-partenaire</a> </li>

            <li> <a href="https://www.uber.com/fr/fr/business/solutions/eats/overview/">Créez un compte professionnel</a> </li>

            <li> <a href="https://www.ubereats.com/fr/promo">Économisez sur votre première commande</a> </li>

          </ul>
        </div>

        <div class="content_right">
          <ul>
            <li> <a href="https://www.ubereats.com/fr/near-me">Restaurants à proximité</a> </li>

            <li> <a href="https://www.ubereats.com/fr/location">Affichez toutes les villes</a> </li>

            <li> <a href="https://www.ubereats.com/fr/location#all-countries">Tous les pays</a> </li>

            <li> <a href="https://www.uber.com/fr/blog/eat/">Consultez notre blog</a> </li>

            <li> <a href="https://about.ubereats.com/fr/fr/">À propos d'Uber Eats</a> </li>

            <li> <a href="https://www.ubereats.com/fr?mod=selectLanguage&ps=1">Français</a> </li>

          </ul>
        </div>

      </div>

      <div class="separate"></div>



    </div>

  </div>

</template>

<script>
export default {
  name: "Footer"
}
</script>

<style scoped>

*{
  background: #000000;
  box-sizing: border-box;
}


.footer{
  margin-top: 80px;
  padding: 72px 0 88px 0;

}


.content {
  padding: 0 40px;
  margin: 0 auto;
}

.content_flex{
  display: flex;
}

.content_left{
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
  flex-direction: column;
  flex: 2;
}

.logo_uber_eats{
  width: 100%;
}

.logo_uber_eats img {
  height: 24px;
  margin-bottom: 64px;
}


.logo_application{
  display: flex;
  }

.logo_application img{
  height: 40px;
}

.space_16 {
  width: 16px;
}


.content_middle {
  display: flex;
  flex:1;
  flex-direction: column;
}

.content_right {
  display: flex;
  flex:1;
  flex-direction: column;
}


.content_middle a {
  display: block;
  color: white;
  text-decoration: none;
  font-size: 16px;
  line-height: 16px;
  margin-bottom: 16px;
}

.content_right a{
  display: block;
  color: white;
  text-decoration: none;
  font-size: 16px;
  line-height: 16px;
  margin-bottom: 16px;
}

.content_middle ul {
  padding: 0;
  margin: 0;
  list-style: none;
}

.content_right ul {
  padding: 0;
  margin: 0;
  list-style: none;
}

.separate {
  margin: 40px 0;
  border-bottom: 1px solid #F6F6F6;
  bottom: 1.6rem;
}
</style>