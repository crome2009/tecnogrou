Certo, ecco il codice HTML, CSS e JavaScript tutto insieme per il sito "TECNOGROUP". Questo codice include la struttura della pagina, lo stile e le funzionalità JavaScript per la navigazione e il carrello.

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>TECNOGROUP</title>
  <style>
    /* Reset */
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

    /* Header */
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

    .header__logo, .header__quick {
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

    /* Title System */
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

    /* Button System */
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

    /* Cover */
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

    /* Carrello */
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

    .product .title, .product .price {
      color: #fff;
      margin-top: 10px;
    }

    .cart {
      background: #fff;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    }

    .cart h2 {
      margin-bottom: 10px;
    }

    .cart ul {
      list-style: none;
      padding: 0;
    }

    .cart li {
      display: flex;
      justify-content: space-between;
      padding: 10px 0;
      border-bottom: 1px solid #ccc;
    }

    .cart-total {
      font-weight: bold;
      margin-top: 10px;
    }

    .remove-btn {
      background: #ff0000;
      color: #fff;
      border: none;
      padding: 5px 10px;
      cursor: pointer;
      border-radius: 5px;
    }

    .comment.bot-reply {
      background: #f1f1f1;
      border-radius: 5px;
      padding: 10px;
      margin: 10px 0;
    }
  </style>
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
    <h1

