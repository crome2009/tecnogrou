# tecnogrou

<head>
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


<br><br><br><br><br><br><br>



</body>

