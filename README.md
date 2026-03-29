# cholloshop
Tienda online con las mejores ofertas de el mercado 
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>CholloShop - Admin Simple</title>
  <style>
    body { font-family: Arial, sans-serif; background: #f8f9fa; padding: 20px; }
    .container { max-width: 900px; margin: auto; background: white; padding: 25px; border-radius: 15px; box-shadow: 0 5px 20px rgba(0,0,0,0.1); }
    h1 { color: #e91e63; text-align: center; }
    input, textarea { width: 100%; padding: 10px; margin: 10px 0; border: 1px solid #ddd; border-radius: 8px; }
    button { background: #e91e63; color: white; padding: 12px 20px; border: none; border-radius: 8px; cursor: pointer; font-size: 16px; }
    button:hover { background: #c2185b; }
    .producto { margin-top: 40px; border-top: 2px solid #eee; padding-top: 20px; }
    .qr { text-align: center; margin: 30px 0; }
  </style>
</head>
<body>

<div class="container">
  <h1>🔥 CholloShop - Añadir Producto</h1>

  <!-- Código QR (cámbialo cuando tengas tu enlace real) -->
  <div class="qr">
    <p><strong>¡Escanea para ver chollos brutales!</strong></p>
    <img src="https://api.qrserver.com/v1/create-qr-code/?size=250x250&data=https://tutienda.netlify.app" alt="QR">
    <p style="color:#e91e63; font-weight:bold;">
      Mira esta tienda super barata 🔥 Seguro que ves algún chollo interesante
    </p>
  </div>

  <h2>Pega aquí el enlace de Alibaba:</h2>
  <input type="text" id="alibabaLink" placeholder="https://es.alibaba.com/product-detail/..." />

  <button onclick="alert('Enlace guardado. Ahora copia manualmente los datos de Alibaba y pégalos abajo.')">
    Guardar enlace (solo para recordar)
  </button>

  <div class="producto">
    <h2>Datos del producto (tú los editas):</h2>
    
    <label>Título del producto:</label>
    <input type="text" id="titulo" placeholder="Ej: Anillo de Plata 925 con Piedra Brillante">

    <label>Descripción completa (copia de Alibaba):</label>
    <textarea id="descripcion" rows="6" placeholder="Pega aquí toda la descripción larga de Alibaba..."></textarea>

    <label>Precio que tú quieres mostrar (ej: 12.99 €):</label>
    <input type="text" id="precio" placeholder="12.99">

    <label>Tiempo de envío (copia de Alibaba):</label>
    <input type="text" id="envio" placeholder="Envío gratis en 8-15 días">

    <label>Tallas / Variaciones (copia de Alibaba):</label>
    <textarea id="tallas" rows="3" placeholder="Talla 6,7,8,9 | Color: Plata, Oro..."></textarea>

    <label>Opciones de envío:</label>
    <textarea id="opcionesEnvio" rows="3" placeholder="• Estándar: Gratis (8-15 días)&#10;• Rápido: +4.99€ (4-7 días)"></textarea>

    <label>URL de la foto principal:</label>
    <input type="text" id="foto" placeholder="https://imagen-de-alibaba.jpg">

    <button onclick="mostrarProducto()">Ver cómo queda el producto</button>
  </div>

  <!-- Aquí aparecerá la vista previa -->
  <div id="preview" style="margin-top:40px; display:none; border:2px solid #e91e63; padding:20px; border-radius:12px;">
    <h2 id="prevTitulo"></h2>
    <img id="prevFoto" style="width:100%; max-height:400px; object-fit:contain;" alt="producto">
    <p class="precio" id="prevPrecio" style="font-size:28px; color:#e91e63; font-weight:bold;"></p>
    <p><strong>Descripción:</strong> <span id="prevDesc"></span></p>
    <p class="envio" id="prevEnvio" style="color:#4caf50; font-weight:bold;"></p>
    <p><strong>Tallas:</strong> <span id="prevTallas"></span></p>
    <p><strong>Opciones de envío:</strong><br><span id="prevOpciones"></span></p>
  </div>
</div>

<script>
function mostrarProducto() {
  document.getElementById('preview').style.display = 'block';
  document.getElementById('prevTitulo').textContent = document.getElementById('titulo').value;
  document.getElementById('prevPrecio').innerHTML = document.getElementById('precio').value + ' €';
  document.getElementById('prevDesc').textContent = document.getElementById('descripcion').value;
  document.getElementById('prevEnvio').textContent = document.getElementById('envio').value;
  document.getElementById('prevTallas').textContent = document.getElementById('tallas').value;
  document.getElementById('prevOpciones').innerHTML = document.getElementById('opcionesEnvio').value.replace(/\n/g, '<br>');
  document.getElementById('prevFoto').src = document.getElementById('foto').value || 'https://via.placeholder.com/800x600?text=Sin+Foto';
}
</script>

</body>
</html>
