# cholloshop
Tienda online con las mejores ofertas de el mercado 
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>CholloShop - Ofertas Brutales</title>
  <style>
    body {
      font-family: 'Segoe UI', Arial, sans-serif;
      background: linear-gradient(135deg, #f5f7fa, #e4e9f2);
      margin: 0;
      padding: 20px;
      color: #333;
    }
    .container {
      max-width: 900px;
      margin: 0 auto;
      background: white;
      border-radius: 20px;
      box-shadow: 0 10px 30px rgba(0,0,0,0.1);
      overflow: hidden;
    }
    header {
      background: #e91e63;
      color: white;
      text-align: center;
      padding: 30px 20px;
    }
    h1 {
      margin: 0;
      font-size: 2.5em;
    }
    .subtitle {
      font-size: 1.2em;
      opacity: 0.9;
    }
    .qr-section {
      text-align: center;
      padding: 30px 20px;
      background: #fff;
    }
    .qr-section img {
      width: 200px;
      height: 200px;
      border: 10px solid #fff;
      box-shadow: 0 5px 20px rgba(0,0,0,0.15);
      border-radius: 12px;
    }
    .producto {
      padding: 30px;
      border-top: 1px solid #eee;
    }
    .producto img {
      width: 100%;
      max-height: 400px;
      object-fit: contain;
      border-radius: 12px;
    }
    .precio {
      font-size: 32px;
      color: #e91e63;
      font-weight: bold;
      margin: 15px 0;
    }
    .old-price {
      text-decoration: line-through;
      color: #999;
      font-size: 18px;
    }
    button {
      background: #e91e63;
      color: white;
      border: none;
      padding: 15px 30px;
      font-size: 18px;
      border-radius: 10px;
      cursor: pointer;
      margin-top: 20px;
    }
    button:hover {
      background: #c2185b;
    }
  </style>
</head>
<body>

<div class="container">
  <header>
    <h1>🔥 CholloShop</h1>
    <p class="subtitle">Tienda online con las mejores ofertas del mercado</p>
  </header>

  <div class="qr-section">
    <p><strong>¡Escanea y descubre chollos increíbles!</strong></p>
    <img src="https://api.qrserver.com/v1/create-qr-code/?size=300x300&data=https://cholloshop.netlify.app" 
         alt="Código QR CholloShop">
    <p style="margin-top: 15px; font-size: 1.1em; color: #e91e63;">
      Mira esta tienda super barata 🔥<br>
      Seguro que ves algún chollo interesante
    </p>
  </div>

  <!-- Producto de ejemplo -->
  <div class="producto">
    <img src="https://via.placeholder.com/800x500?text=Producto+de+Ejemplo" alt="Producto">

    <h2>Anillo Elegante con Piedra Brillante - Plata 925</h2>
    
    <p class="precio">12,99 € <span class="old-price">29,99 €</span></p>
    
    <p><strong>Descripción:</strong> Anillo de alta calidad fabricado en plata 925 con piedra brillante. Diseño moderno y elegante, perfecto para cualquier ocasión.</p>
    
    <p style="color: #4caf50; font-weight: bold;">🚚 Envío gratis en 8-15 días</p>
    
    <p><strong>Tallas disponibles:</strong> 6, 7, 8, 9</p>
    
    <p><strong>Opciones de envío:</strong><br>
      • Estándar: Gratis (8-15 días)<br>
      • Express: +4,99 € (4-7 días)
    </p>

    <button onclick="alert('Producto añadido al carrito ✓')">Añadir al carrito</button>
  </div>

</div>

</body>
</html>
