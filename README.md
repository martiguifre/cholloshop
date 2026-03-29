# cholloshop
Tienda online con las mejores ofertas de el mercado 
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>CholloShop - Ofertas y Chollos</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f8f9fa;
      margin: 0;
      padding: 20px;
      color: #333;
    }
    .header {
      background: #e91e63;
      color: white;
      text-align: center;
      padding: 40px 20px;
      border-radius: 12px;
      margin-bottom: 30px;
    }
    .header h1 {
      margin: 0;
      font-size: 2.8em;
    }
    .catalogo {
      max-width: 1100px;
      margin: 0 auto;
    }
    .producto {
      background: white;
      border-radius: 16px;
      box-shadow: 0 6px 20px rgba(0,0,0,0.1);
      margin-bottom: 30px;
      overflow: hidden;
    }
    .producto img {
      width: 100%;
      height: 300px;
      object-fit: cover;
    }
    .info {
      padding: 25px;
    }
    .precio {
      font-size: 32px;
      color: #e91e63;
      font-weight: bold;
      margin: 10px 0;
    }
    .old-price {
      text-decoration: line-through;
      color: #999;
      font-size: 20px;
    }
    .descripcion {
      line-height: 1.6;
      margin: 15px 0;
    }
    button {
      background: #e91e63;
      color: white;
      border: none;
      padding: 15px 30px;
      font-size: 18px;
      border-radius: 10px;
      cursor: pointer;
    }
    button:hover {
      background: #c2185b;
    }
  </style>
</head>
<body>

  <div class="header">
    <h1>🔥 CholloShop</h1>
    <p>Tienda online con las mejores ofertas del mercado</p>
  </div>

  <div class="catalogo">

    <!-- Producto 1 -->
    <div class="producto">
      <img src="https://via.placeholder.com/800x400?text=Anillo+de+Plata" alt="Anillo">
      <div class="info">
        <h2>Anillo Elegante con Piedra Brillante - Plata 925</h2>
        <p class="precio">12,99 € <span class="old-price">29,99 €</span></p>
        <p class="descripcion">
          Anillo de alta calidad fabricado en plata 925 con piedra brillante. 
          Diseño moderno y elegante, perfecto para regalo o uso diario.
        </p>
        <p style="color:#4caf50; font-weight:bold;">🚚 Envío gratis en 8-15 días</p>
        <p><strong>Tallas disponibles:</strong> 6 | 7 | 8 | 9</p>
        <button onclick="alert('Producto añadido al carrito ✓')">Añadir al carrito</button>
      </div>
    </div>

    <!-- Puedes copiar y pegar más productos aquí abajo -->

  </div>

</body>
</html>
</html>
