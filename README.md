



<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>TECNOGROUP</title>
  <link rel="stylesheet" href="style.css">
  <script>
    document.addEventListener("DOMContentLoaded", function() {
      const menu = document.querySelector('.header__menu');
      menu.addEventListener('click', function(event) {
        if (event.target.tagName === 'A') {
          event.preventDefault();
          const targetId = event.target.getAttribute('href').substring(1);
          const targetSection = document.getElementById(targetId);
          if (targetSection) {
            window.scrollTo({
              top: targetSection.offsetTop,
              behavior: 'smooth'
            });
          }
        }
      });
    });
  </script>
</head>
<body>
<header class="header">
  <div class="header__content">
    <a class="header__logo" href="#">
      <strong>TECNOGROUP</strong>
    </a>
    <ul class="header__menu">
      <li><a href="#lavori">Lavori</a></li>
      <li><a href="#chisiamo">Chi Siamo</a></li>
      <li><a href="#contatti">Contatti</a></li>
      <li><a href="#ordina-ora">Ordina Ora</a></li>
      <li><a href="#info">Info</a></li>
    </ul>
    <div class="header__quick">
      <a href="#contatti" class="button mb-2">Contattaci</a>
      <div class="icon-hamburger">
        <span></span>
        <span></span>
      </div>
    </div>
  </div>
</header>

<div class="cover" style="background-image:linear-gradient(to bottom, rgba(0,0,0,0.2), rgba(0,0,0,0.6)), url('https://images2.alphacoders.com/434/thumb-1920-434134.jpg');">
  <div class="cover__content">
    <h1> TECNOGROUP</h1>
    <h2> Azienda edile</h2>
  </div>
</div>

<br><br><br><br>

<div class="grid">
  <div class="col-50" id="chisiamo">
    <div style="text-align: justify;">
      <h1>CHI SIAMO?</h1>
      <p>TECNOGROUP Snc. La nostra etica professionale è basata sulla passione e sull'amore per il lavoro. Siamo un'azienda molto esperta che opera nella provincia di Milano, Varese e Monza. Ci impegniamo a fornire servizi su misura e di alta qualità, valutando attentamente soluzioni adatte a ogni situazione. Offriamo una vasta gamma di servizi, tra cui nuove costruzioni, opere murarie portanti e tamponature di varie tipologie, tramezzature portanti o divisorie in muratura piena o alveolata, assistenza impianti, rifacimento tetti, facciate, e ristrutturazioni complete o parziali di case, condomini, appartamenti, edifici commerciali, industriali e singoli locali come bagni, cucine, uffici, studi, saloni, eccetera. Ci occupiamo anche di progettazione e manutenzione ordinaria e straordinaria. Scegliendo TECNOGROUP, potrete contare su uno staff altamente affidabile e professionale e su un supporto serio e continuativo. Il nostro unico obiettivo è guadagnare la vostra fiducia e soddisfazione, mantenendo al contempo i costi contenuti e garantendo la massima qualità nei nostri servizi.</p>
    </div>
  </div>
</div>

<br><br><br><br>

<div class="container-video">
  <video src="D:\TECNOGROUP .2.mp4" autoplay muted loop playsinline controls></video>
</div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.10.2/gsap.min.js" charset="utf-8"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.10.2/ScrollTrigger.min.js"></script>

<script>
  let tl = gsap.timeline({
    scrollTrigger:{
      trigger: ".container-video",
      start: "top center",
      end: "bottom center",
      scrub: true,
    }
  });

  tl.to(".container-video", {
    opacity: 1,
    width: "80%"
  });
</script>

<script>
  let item = document.querySelector('.icon-hamburger');
  item.addEventListener("click", function() {
    document.body.classList.toggle('menu-open');
  });
</script>

<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>

<div class="grid">
  <div class="col-50" id="lavori">
    <h1>Lavori</h1>
    <p>Qui ci saranno i dettagli sui lavori eseguiti dall'azienda.</p>
  </div>
</div>

<br><br><br><br>

<div class="grid">
  <div class="col-50" id="ordina-ora">
    <div style="text-align: justify;">
      <h1>Ordina Ora</h1>
      <div class="product">
        <img src="https://i.pinimg.com/originals/3e/c8/3d/3ec83db557850a650cdd1e52cae7cfef.jpg" alt="Product Image">
        <div class="title"><h4>GRES EFFETTO LEGNO</h4></div>
        <div class="price"><h4>€ 14.00</h4></div>
        <button class="button" onclick="addToCart('PIASTRELLE GRES EFFETTO LEGNO', 14.00)">Aggiungi al carrello</button>
      </div>
      <div class="product">
        <img src="https://www.bing.com/th?id=OPEC.6WibUN5mblDNcA474C474&o=5&pid=21.1&w=160&h=160&qlt=100&dpr=1&c=8" alt="Product Image">
        <div class="title"><h4>Lavabo da Appoggio Lavandino moderno Rotondo in Ceramica Bianca 40 x 15 cm -75577</h4></div>
        <div class="price"><h4>€ 83.99</h4></div>
        <button class="button" onclick="addToCart('Lavandino moderno Rotondo ', 83.99)">Aggiungi al carrello</button>
      </div>
      <div class="product">
        <img src="https://limitless.sirv.com/magento/catalog/product/b/c/bctbw001.jpg?q=80&canvas.width=1000&canvas.height=1000&canvas.color=ffffff&w=1000&h=1000" alt="Product Image">
        <div class="title"><h4>Sanitario Bagno WC Ovale 460x360x565mm con Sedile Copri WC Soft Close - Alswear</h4></div>
        <div class="price"><h4>€ 168.00</h4></div>
        <button class="button" onclick="addToCart('Sanitario Bagno WC Ovale ', 168.00)">Aggiungi al carrello</button>
      </div>
      <div class="product">
        <img src="https://limitless.sirv.com/magento/catalog/product/b/f/bfb2012_hr_a_1000.jpg?q=80&canvas.width=1000&canvas.height=1000&canvas.color=ffffff&w=1000&h=1000" alt="Product Image">
        <div class="title"><h4>Lavabo Bagno da Appoggio in Ceramica Ovale 590x425mm - Otterton</h4></div>
        <div class="price"><h4>€ 156.00</h4></div>
        <button class="button" onclick="addToCart('Lavabo Bagno da Appoggio', 156.00)">Aggiungi al carrello</button>
      </div>
        <div class="product">
          <img src="https://www.bing.com/th?id=OPEC.LH4UuI2N1KZzyw474C474&o=5&pid=21.1&w=160&h=160&qlt=100&dpr=1&c=8" alt="Product Image">
          <div class="title"><h4>Box doccia 70x100 doppio scorrevole altezza 190 Kamalu-1000</h4></div>
          <div class="price"><h4>€ 197,45</h4></div>
          <button class="button" onclick="addToCart('Box doccia', 197.45)">Aggiungi al carrello</button>
        </div>
        <div class="cart">
          <h2>Carrello</h2>
          <ul id="cart-items"></ul>
          <p id="cart-total">Totale: €0.00 </p>
        </div>
      </div>
    </div>
  </div>

  <script>
    document.querySelectorAll('.remove-btn').forEach(button => {
        button.addEventListener('click', () => {
            button.closest('.cart-item').classList.add('fade-out');
            setTimeout(() => {
                button.closest('.cart-item').remove();
                updateTotal();
            }, 500);
        });
    });

    function updateTotal() {
        let total = 0;
        document.querySelectorAll('.cart-item .price').forEach(price => {
            total += parseFloat(price.textContent.replace('€', ''));
        });
        document.querySelector('.cart-total h3').textContent = 'Totale: €' + total.toFixed(2);
    }
</script>
<script>
  let cart = [];

  function addToCart(productName, productPrice) {
    cart.push({ name: productName, price: productPrice });
    updateCart();
  }

  function updateCart() {
    const cartItems = document.getElementById('cart-items');
    const cartTotal = document.getElementById('cart-total');
    cartItems.innerHTML = '';
    let total = 0;

    cart.forEach((item, index) => {
      const listItem = document.createElement('li');
      listItem.textContent = `${item.name} - €${item.price.toFixed(2)}`;
      cartItems.appendChild(listItem);
      total += item.price;
    });

    cartTotal.textContent = `Totale: €${total.toFixed(2)}`;
  }
</script>

<br><br><br><br>

<div class="grid">
  <div class="col-50" id="contatti">
    <div style="text-align: justify;">
      <h1>Contattaci</h1>
      <p>Per qualsiasi informazione, potete contattarci ai seguenti recapiti:</p>
      <p><strong>Telefono referente Giancarlo:</strong> +39 347 269 2695<br>
        <strong>Email:</strong> tecnogroupsnc@libero.it</p>
      <a href="mailto:tecnogroupsnc@libero.it" class="button">Invia Email</a>
    </div>
  </div>
</div>




<br><br><br><br><br><br>

<div class="grid">
  <div class="col-50" id="info">
    <div style="text-align: justify;">
      <h1>Info</h1>
    <div id="commentSection">
    <button class="button" onclick="displayReply('chi siete')">Chi siamo?</button><br><br>
    <button class="button" onclick="displayReply('cosa facciamo')">Cosa facciamo?</button><br><br>
    <button class="button" onclick="displayReply('dove operiamo')">Dove operiamo?</button><br><br>
    <button class="button" onclick="displayReply('etica professionale')">Qual è la nostra etica professionale?</button><br><br>
    <button class="button" onclick="displayReply('servizi offerti')">Quali servizi offriamo?</button><br><br>
    <button class="button" onclick="displayReply('come contattarci')">Come contattarci?</button><br><br>
    <button class="button" onclick="displayReply('nostri obiettivi')">Quali sono i nostri obiettivi?</button><br><br>
    <button class="button" onclick="displayReply('cosa ci distingue')">Cosa ci distingue?</button><br><br>
    <button class="button" onclick="displayReply('referente')">Chi è il nostro referente?</button><br><br>
    <button class="button" onclick="displayReply('recapiti')">Quali sono i nostri recapiti?</button><br><br>
    <button class="button" onclick="displayReply('specializzazione')">Qual è la nostra specializzazione?</button><br><br>
    <button class="button" onclick="displayReply('come garantiamo qualità')">Come garantiamo la qualità?</button><br><br>
    <button class="button" onclick="displayReply('team')">Chi fa parte del nostro team?</button><br><br>
  
    </div>
<script>
  function displayReply(question) {
      const replies = {
          "chi siete": "Siamo TECNOGROUP Snc, un'azienda molto esperta che opera nella provincia di Milano, Varese e Monza, fornendo servizi su misura e di alta qualità.",
          "cosa facciamo": "Offriamo una vasta gamma di servizi, tra cui nuove costruzioni, opere murarie, rifacimento tetti, facciate e ristrutturazioni complete o parziali di varie tipologie di edifici.",
          "dove operiamo": "Operiamo principalmente nella provincia di Milano, Varese e Monza.",
          "etica professionale": "La nostra etica professionale è basata sulla passione e sull'amore per il lavoro, garantendo servizi su misura e di alta qualità.",
          "servizi offerti": "Offriamo una vasta gamma di servizi, tra cui nuove costruzioni, opere murarie, rifacimento tetti, facciate e ristrutturazioni complete o parziali.",
          "come contattarci": "Potete contattarci tramite telefono al numero +39 347 269 2695 o via email all'indirizzo tecnogroupsnc@libero.it.",
          "nostri obiettivi": "Il nostro unico obiettivo è guadagnare la vostra fiducia e soddisfazione, mantenendo i costi contenuti e garantendo la massima qualità nei nostri servizi.",
          "cosa ci distingue": "Ci distinguono la nostra esperienza, passione e impegno nel fornire servizi su misura e di alta qualità.",
          "referente": "Il nostro referente è Giancarlo, contattabile al numero +39 347 269 2695.",
          "recapiti": "Potete contattarci al telefono referente Giancarlo: +39 347 269 2695 o via email tecnogroupsnc@libero.it.",
          "specializzazione": "Siamo specializzati in nuove costruzioni, opere murarie, rifacimento tetti, facciate e ristrutturazioni complete o parziali.",
          "come garantiamo qualità": "Garantiamo la qualità attraverso un team altamente professionale e affidabile e un supporto serio e continuativo.",
          "team": "Il nostro team è composto da professionisti altamente qualificati e affidabili."
      };

      const replyText = replies[question];
      const commentSection = document.getElementById('commentSection');
      
      // Creazione del div per la risposta
      const botReply = document.createElement('div');
      botReply.className = 'comment bot-reply';
      botReply.innerText = replyText;
      commentSection.appendChild(botReply);

      // Scorri in basso per mostrare il nuovo commento
      commentSection.scrollTop = commentSection.scrollHeight;
  }
</script>

/* ! Reset */
body, html{ font-family: 'Inter', Arial, Helvetica, sans-serif; font-size: 16px; box-sizing: border-box;margin: 0;padding: 0;}*,*:before,*:after{ box-sizing: border-box; }h1,h2,h3,h4,h5,h6, p, ol, ul{margin: 0 0 1rem 0;padding: 0;}ol,ul{list-style-type: none;}img{height: auto;}h1{font-size: 4rem;} h2{font-size: 3rem;} h3{font-size: 2rem;} h4{font-size: 1rem;} h5{font-size: 0.8rem;} h6{font-size: 0.6rem;}a{text-decoration:none}

.spacer{height: 100px;}

/* Menu */
:root { 
    --menu-bg: #b9aeae; 
    --menu-color: #333; 
}

/*style*/
.container-video{
  border: 1px solid;
  background: #000000; 
  width: 100%;
  height: 500px;
  margin: 0 auto;
  opacity: 0;
  position: relative;  
}
.container-video video{
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: auto;
}
.spacer{
  height: 80ovh;
}




/* ! Reset */
body, html {
  font-family: 'Inter', Arial, Helvetica, sans-serif;
  font-size: 16px;
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

*, *:before, *:after {
  box-sizing: border-box;
}

h1, h2, h3, h4, h5, h6, p, ol, ul {
  margin: 0 0 1rem 0;
  padding: 0;
}

ol, ul {
  list-style-type: none;
}

img {
  height: auto;
}

h1 {
  font-size: 4rem;
}

h2 {
  font-size: 3rem;
}

h3 {
  font-size: 2rem;
}

h4 {
  font-size: 1rem;
}

h5 {
  font-size: 0.8rem;
}

h6 {
  font-size: 0.6rem;
}

a {
  text-decoration: none;
}

.spacer {
  height: 100px;
}

/* Menu */
:root {
  --menu-bg: #afa2a2;
  --menu-color: #333;
}

/*style*/
.container-video {
  border: 1px solid;
  background: #000000;
  width: 100%;
  height: 500px;
  margin: 0 auto;
  opacity: 0;
  position: relative;
}

.container-video video {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: auto;
}

.spacer {
  height: 80vh;
}

/*head*/
.header {
  background-color: var(--menu-bg);
  position: fixed;
  top: 0;
  left: 0;
  z-index: 9999;
  width: 100%;
  padding: 10px 15px;
}

.header__content {
  max-width: 1200px;
  width: 100%;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
}

.header__logo,
.header__quick {
  display: flex;
  align-items: center;
  color: var(--menu-color);
}

.header__menu {
  padding: 0;
  margin: 0;
}

.header__menu li {
  display: inline-block;
}

.header__menu li a {
  color: var(--menu-color);
  opacity: 0.8;
  display: block;
  padding: 16px;
  font-size: 15px;
}

@media (max-width: 768px) {
  .header__menu {
    position: absolute;
    top: 60px;
    left: 0;
    background-color: var(--menu-bg);
    width: 100%;
    height: 100vh;
    height: 0vh;
    overflow: hidden;
    transition: all 1s cubic-bezier(.215, .61, .355, 1);
  }

  .header__menu li {
    width: 100%;
    border-bottom: 1px solid #000000;
  }

  .menu-open .header__menu {
    height: 100vh;
    padding: 3%;
  }

  .icon-hamburger {
    height: 50px;
    width: 40px;
    margin-left: 20px;
    padding-top: 5px;
  }

  .icon-hamburger span {
    height: 2px;
    width: 30px;
    background: var(--menu-color);
    position: relative;
    display: block;
    margin-top: 11px;
    transition: all 0.2s cubic-bezier(.215, .61, .355, 1);
  }

  .menu-open .icon-hamburger span:nth-child(1) {
    transform: rotate(45deg) translateY(9px);
  }

  .menu-open .icon-hamburger span:nth-child(2) {
    transform: rotate(-45deg) translateY(-9px);
  }

  .header__quick {
    display: flex;
    justify-content: flex-end;
    width: 50%;
  }
}

/* ! Title System */
h1, .text-1 {
  font-size: 3.5rem;
  margin-bottom: 0.5rem;
  color: #000000;
}

h2, .text-2 {
  font-size: 2.4rem;
  margin-bottom: 1rem;
  color: #000000;
}

h3, .text-3 {
  font-size: 1.8rem;
  margin-bottom: 1rem;
  color: #000000;
}

h4, p, .text-4 {
  font-size: 1rem;
  margin-bottom: 1rem;
  line-height: 1.5;
  color: #000000;
}

a {
  color: rgb(0, 0, 0);
}

/* ! button System */
.button {
  font-size: 1rem;
  text-transform: uppercase;
  background: #333;
  color: #fff;
  text-decoration: none;
  padding: 14px 25px;
  display: inline-block;
  border-radius: 4px;
  font-weight: 700;
}

.button:hover {
  background: #ff0000;
}

/* ! Cover */
.cover {
  text-align: center;
  padding: 10px;
  margin: 0px;
  min-height: 600px;
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  background-position: center center;
  background-size: cover;
}

.cover * {
  color: #fff;
}

/*carrello*/
body {
  font-family: 'Inter', sans-serif;
  margin: 0;
  padding: 0;
  background: #c0bdbd;
  color: #000000;
  font-size: 1rem;
}

.product {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 50px;
  background: #686262;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.product img {
  max-width: 30%;
  border-radius: 10px;
}

.product .title {
  font-size: 1.5em;
  margin: 20px 0;
}

.product .price {
  font-size: 1.2em;
  color: #ffffff;
  margin-bottom: 20px;
}

.product .button {
  background: #ff730048;
  color: #ffffff;
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  text-decoration: none;
  font-weight: 700;
  cursor: pointer;
}

.product .button:hover {
  background: #ff0000;
}

.cart {
  margin: 20px;
  padding: 20px;
  background: #686262;
  border-radius: 10px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.cart h2 {
  margin: 0 0 20px;
}

.cart ul {
  list-style: none;
  padding: 0;
}

.cart ul li {
  margin-bottom: 10px;
}









/* ! Grid System */
.grid {
  margin: 0 auto;
  padding: 0 15px;
  max-width: 1250px;
  display: flex;
  flex-flow: row;
  flex-wrap: wrap;
}

.grid--center {
  justify-content: center;
}

.col {
  flex: 1;
}

[class*='col-'] {
  position: relative;
  padding: 0 15px;
}

.grid .grid [class*='col-'] {
  padding: 0px;
}

.col-20 {
  width: 20%;
}

.col-25 {
  width: 25%;
}

.col-30 {
  width: 30%;
}

.col-33 {
  width: 33.33%;
}

.col-50 {
  width: 50%;
}

.col-70 {
  width: 70%;
}

.col-80 {
  width: 80%;
}

.col-100 {
  width: 100%;
}









/*head*/
.header{ background-color: var(--menu-bg); position: fixed; top:0;  left:0; z-index: 9999; width: 100%; padding: 10px 15px; }
.header__content{max-width: 1200px;width: 100%;margin: 0 auto; display: flex;justify-content: space-between;}

.header__logo,
.header__quick{display: flex; align-items: center;color:var(--menu-color)}

.header__menu{padding: 0;margin: 0;}
.header__menu li{display: inline-block;}
.header__menu li a{color:var(--menu-color); opacity: 0.8;display: block;padding: 16px;font-size: 15px;}

@media (max-width: 768px) {
  .header__menu{   
    position: absolute; top:60px; left:0; background-color: var(--menu-bg); width: 100%; height: 100vh;
    height: 0vh; overflow: hidden;transition: all 1s cubic-bezier(.215, .61, .355, 1);
  }

  .header__menu li{width: 100%;border-bottom: 1px solid #000000}
  .menu-open .header__menu{height: 100vh;padding: 3%;}

  .icon-hamburger{height: 50px;width: 40px;margin-left: 20px;padding-top: 5px;}
  .icon-hamburger span{height: 2px; width: 30px;background: var(--menu-color);position: relative;display: block;margin-top: 11px;transition: all 0.2s cubic-bezier(.215, .61, .355, 1);}

  .menu-open .icon-hamburger span:nth-child(1){transform: rotate(45deg) translateY(9px);}
  .menu-open .icon-hamburger span:nth-child(2){transform: rotate(-45deg) translateY(-9px);}

  .header__quick{display: flex; justify-content: flex-end; width: 50%;}

}




/* ! Title System */
h1, .text-1 {font-size: 3.5rem;margin-bottom:0.5rem;color: #000000;}
h2, .text-2 {font-size: 2.4rem;margin-bottom:1rem; color: #000000;}
h3, .text-3  {font-size: 1.8rem;margin-bottom:1rem; color: #000000;}
h4, .text-4 {font-size: 1rem;margin-bottom:1rem; line-height: 1.5;color: #ffffff;}
p, .text-4 {font-size: 1rem;margin-bottom:1rem; line-height: 1.5;color: #000000;}
a{color: rgb(0, 0, 0)}





/* ! button System */
.button { 
  font-size: 1rem; text-transform: uppercase; background: #333; color:#fff;
  text-decoration: none;padding: 14px 25px; display: inline-block;
  border-radius: 4px; font-weight: 700;
}
.button:hover{ background: #ff0000; }







/* ! Cover */
.cover{ 
  text-align: center; padding:10px; margin:0px; min-height:600px; width:100%; 
  display:flex; flex-direction:column; justify-content:center; 
  background-position: center center; background-size:cover;
}
.cover * {color:#fff}






/*carrello*/
    .grid {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
    }

    .product {
      flex: 1 1 calc(20% - 10px);
      box-sizing: border-box;
      border: 1px solid #646262;
      padding: 10px;
      text-align: center;
      
    }

    .product img {
      max-width: 100%;
      height: auto;
    }

    .button {
      padding: 10px 20px;
      background-color: #ff6600;
      color: white;
      border: none;
      cursor: pointer;
      transition: transform 0.2s;
    }

    .product .button:hover {
      padding: 10px 20px;
      background-color: #ff6600;
      color: white;
      border: none;
      cursor: pointer;
      transition: transform 0.2s;
    }


    

    @keyframes add-to-cart {
      0% { transform: scale(1); }
      50% { transform: scale(1.1); }
      100% { transform: scale(1); }
    }

    .added {
      animation: add-to-cart 0.5s ease-in-out;
    }














/* ! Grid System */
.grid { margin: 0 auto; padding: 0 15px; max-width: 1250px; display: flex; flex-flow: row; flex-wrap: wrap;}
.grid--center{justify-content: center;}
.col{ flex: 1;}

[class*='col-'] { position: relative;padding: 0 15px;}
.grid .grid [class*='col-'] {padding: 0px;}

.col-20{ width: 20%; }
.col-25{ width: 25%; }
.col-30{ width: 30%; }
.col-33{ width: 33.33%; }
.col-50{ width: 50%; }
.col-70{ width: 70%; }
.col-80{ width: 80%; }
.col-100{ width: 100%; }

@media (max-width: 991px) {
    .tab-20 { width: 20%; }
    .tab-25 { width: 25%; }
    .tab-33 { width: 33.33%; }
    .tab-50 { width: 50%; }
    .tab-100 { width: 100%; }
}

@media (max-width: 768px) {
    [class*='col-'] { width: 100%;}
    .sma-20 { width: 20%; }
    .sma-25 { width: 25%; }
    .sma-33 { width: 33.33%; }
    .sma-50 { width: 50%; }
    .sma-100 { width: 100%; }
}

/* ! Helpers  */
.mt-0{margin-top: 0 }
.mt-1{margin-top: 10px}
.mt-2{margin-top: 20px}
.mt-3{margin-top: 40px}
.mt-4{margin-top: 100px }

.mb-0{margin-bottom: 0}
.mb-1{margin-bottom: 10px}
.mb-2{margin-bottom: 20px}
.mb-3{margin-bottom: 40px}
.mb-4{margin-bottom: 100px}

.p-0{padding: 0}
.p-1{padding: 10px}
.p-2{padding: 20px}
.p-3{padding: 40px}
.p-4{padding: 100px}

.pt-1{padding-top: 10px;}
.pt-3{padding-top: 20px;}
.pt-3{padding-top: 40px;}
.pt-4{padding-top: 15vh;}

.pb-1{padding-bottom: 10px;}
.pb-2{padding-bottom: 20px;}
.pb-3{padding-bottom: 40px;}
.pb-4{padding-bottom: 15vh;}

.text-center { text-align: center; }
.text-right { text-align: right; }
.text-left { text-align: left; }
.img-res { width: 100%; height: auto; margin-bottom: 20px;vertical-align: middle;}
<br><br><br><br><br><br><br>



</body>
</html>

