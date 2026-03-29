!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi Tienda de Importaciones</title>
    <style>
        body { font-family: 'Segoe UI', sans-serif; background-color: #f4f4f9; margin: 0; padding: 20px; }
        .container { max-width: 1000px; margin: auto; display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 20px; }
        
        /* Tarjeta de Producto */
        .product-card { background: white; border-radius: 12px; overflow: hidden; box-shadow: 0 4px 15px rgba(0,0,0,0.1); transition: transform 0.3s; }
        .product-card:hover { transform: translateY(-5px); }
        .product-image { width: 100%; height: 250px; object-fit: cover; }
        
        .product-info { padding: 20px; }
        .product-title { font-size: 1.4rem; margin: 0 0 10px; color: #333; }
        .product-price { font-size: 1.8rem; color: #27ae60; font-weight: bold; margin-bottom: 10px; }
        .product-meta { font-size: 0.9rem; color: #666; margin-bottom: 15px; }
        
        /* Botón de Enlace */
        .btn-buy { display: block; text-align: center; background: #ff6a00; color: white; padding: 12px; text-decoration: none; border-radius: 6px; font-weight: bold; }
        .btn-buy:hover { background: #e65f00; }
    </style>
</head>
<body>

    <h1 style="text-align: center; color: #333;">Mis Productos Destacados</h1>

    <div class="container">
        <div class="product-card">
            <img src="https://via.placeholder.com/400x300" alt="Producto" class="product-image">
            <div class="product-info">
                <h2 class="product-title">Nombre Personalizado del Producto</h2>
                <div class="product-price">$45.00</div>
                <div class="product-meta">
                    <span>🚚 Tiempo de envío: 15-20 días</span><br>
                    <span>📦 Disponibilidad: En stock</span>
                </div>
                <p>Descripción optimizada por ti para convencer al cliente, resaltando beneficios y no solo características.</p>
                <a href="TU_ENLACE_
