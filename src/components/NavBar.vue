<template>

  <div class="nav">

    <div class="nav_left">
      <button class="menu">
        <img src="../../src/assets/menu_black_24dp.svg" alt="" role="img" height="20" width="20"/>
      </button>

      <a href="/" >
        <img src="../../src/assets/uber_eats.svg" alt="uber eats" role="img" width="146" height="24" />
      </a>
    </div>

    <div class="delivery_adress">
      <div class="adress">
        <img src="../../src/assets/room_black_24dp.svg" alt="" role="img" />
        <input type="text" placeholder="Saisissez l'adresse de livraison">
      </div>
    </div>


      <a class="to_login" href="https://auth.uber.com/login/?breeze_local_zone=dca11&next_url=https%3A%2F%2Fwww.ubereats.com%2Flogin-redirect%2F%3Fcampaign%3Dsignin_universal_link%26marketing_vistor_id%3Dc1d39fdd-e0d9-4d1a-9817-ca05c7dd7fc5%26redirect%3D%252Ffr&state=a3QWLZbePIb3RM_9z1ST0EHZIFQFllu-FewVTzzyem8%3D" >
        <span>Se connecter</span>
      </a>


  </div>

</template>

<script>
export default {
  name: "NavBar",

  methods: {
    onScroll(){
        const navbar =document.querySelector('.nav');
        const login =document.querySelector('.to_login');
        const address=document.querySelector('.adress');

        if(window.scrollY>96){
          navbar.style.position='fixed';
          navbar.style.backgroundColor='white';
          login.style.backgroundColor='#EEEEEE';
          address.style.visibility='visible'
          address.style.transform='scaleX(1)';
          address.style.transformOrigin='left';


        }else{
          navbar.style.position='absolute';
          navbar.style.backgroundColor='transparent';
          login.style.backgroundColor='white';
          address.style.visibility='hidden';
          address.style.transform='scaleX(0)';
          address.style.transformOrigin='left';
        }

    }
  },

  mounted() {
    window.addEventListener('scroll', this.onScroll)
  }
}
</script>

<style scoped>

.nav{
  position: absolute;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 40px;
  margin: 0 auto;
  height: 96px;
  top:0;
  left: 0;
  right: 0;
  max-width: 1920px;
  min-width: 1024px;
  z-index: 1;
  box-sizing: border-box;
  transition: background 200ms ease;
}

button {
  padding:0;
  background: transparent;
  border: none;
  cursor: pointer;
}

.menu{
  margin-right: 32px;
}

.menu img {
  height: 30px;
  width: 30px;
}

.nav_left{
  display: flex;
  align-items: center;
}

a {
  text-decoration: none;
  color: black;
  font-size: 18px;
}


.delivery_adress{
  min-width: 500px;
  max-width: 540px;
  margin-right:4px;
  flex: 1;
}

.adress {
  display: flex;
  background-color: #F6F6F6;
  border: none;
  padding: 16px;
  box-shadow: inset 0px -1px 0px #e2e2e2;
  transition: transform 500ms;
  visibility: hidden;

}



.adress input{
  outline: none;
  padding: 0;
  border: 0;
  flex: 1;
}

.adress input::placeholder {
  font-size: 16px;
}


.to_login {
  display: flex;
  align-items: center;
  background: white;
  border-radius: 500px;
  padding: 12px 16px;
  min-height: 56px;
  cursor: pointer;
  font-weight: 500;
  line-height: 24px;
  font-size: 18px;
  box-sizing: border-box;

}

</style>