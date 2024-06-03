
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
        <button class="button"

