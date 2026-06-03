
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Codesweed</title>
  <style>
    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      font-family:Arial, sans-serif;
    }

    html {
      scroll-behavior: smooth;
    }

    body{
      background:linear-gradient(to bottom,#d9f99d,#fef9c3,#ffffff);
      color:#333;
    }

    header{
      background:linear-gradient(to right,#15803d,#84cc16,#fde047);
      color:white;
      text-align:center;
      padding:60px 20px;
      border-bottom-left-radius:60px;
      border-bottom-right-radius:60px;
      box-shadow:0 10px 30px rgba(0,0,0,0.2);
    }

    header h1{
      font-size:70px;
      margin-bottom:15px;
      animation:pulse 2s infinite;
    }

    @keyframes pulse{
      0%{transform:scale(1);} 
      50%{transform:scale(1.05);} 
      100%{transform:scale(1);} 
    }

    header p{
      font-size:25px;
      margin-bottom:20px;
    }

    .btn{
      background:white;
      color:#15803d;
      padding:15px 30px;
      border:none;
      border-radius:50px;
      font-size:20px;
      font-weight:bold;
      cursor:pointer;
      transition:0.3s;
      text-decoration: none;
      display: inline-block;
    }

    .btn:hover{
      transform:scale(1.1);
    }

    .titulo{
      text-align:center;
      padding:50px 20px 20px;
    }

    .titulo h2{
      font-size:50px;
      color:#15803d;
      margin-bottom:15px;
    }

    .productos{
      display:flex;
      justify-content:center;
      flex-wrap:wrap;
      gap:30px;
      padding:40px;
    }

    .card{
      background:white;
      width:320px;
      border-radius:40px;
      overflow:hidden;
      box-shadow:0 10px 25px rgba(0,0,0,0.2);
      transition:0.4s;
      border:4px solid #bef264;
    }

    .card:hover{
      transform:translateY(-10px) scale(1.03);
    }

    .card img{
      width:100%;
      height:380px;
      object-fit:cover;
    }

    .card-content{
      padding:25px;
      text-align:center;
    }

    .card h3{
      font-size:30px;
      color:#15803d;
    }

    .precio{
      color:#65a30d;
      font-size:28px;
      margin:15px 0;
      font-weight:bold;
    }

    .pedido{
      background:white;
      margin:40px auto;
      width:95%;
      max-width:1000px;
      padding:40px;
      border-radius:40px;
      box-shadow:0 10px 25px rgba(0,0,0,0.2);
      border:4px solid #bef264;
    }

    .pedido h2{
      text-align:center;
      color:#15803d;
      font-size:45px;
      margin-bottom:30px;
    }

    .opciones-pedido {
      display: flex;
      gap: 30px;
      flex-wrap: wrap;
    }

    .columna-pedido {
      flex: 1;
      min-width: 280px;
      background: #fefce8;
      padding: 25px;
      border-radius: 30px;
      border: 2px dashed #84cc16;
    }

    .columna-pedido h3 {
      text-align: center;
      color: #15803d;
      font-size: 24px;
      margin-bottom: 5px;
    }

    .columna-pedido .subprecio {
      text-align: center;
      color: #65a30d;
      font-size: 16px;
      font-weight: bold;
      margin-bottom: 20px;
    }

    form{
      display:flex;
      flex-direction:column;
      gap:15px;
    }

    input, select, textarea{
      padding:15px;
      border-radius:20px;
      border:2px solid #bef264;
      font-size:16px;
      background: white;
      width: 100%;
    }

    .columna-pedido .btn {
      background: #15803d;
      color: white;
      width: 100%;
      text-align: center;
    }

    .columna-pedido .btn:hover {
      background: #166534;
    }

    .beneficios{
      padding:50px 20px;
      text-align:center;
    }

    .beneficios h2{
      color:#15803d;
      font-size:45px;
      margin-bottom:30px;
    }

    .benefit-container{
      display:flex;
      justify-content:center;
      flex-wrap:wrap;
      gap:20px;
    }

    .benefit{
      background:white;
      width:300px;
      padding:25px;
      border-radius:30px;
      box-shadow:0 5px 15px rgba(0,0,0,0.15);
      transition:0.3s;
    }

    .benefit:hover{
      transform:scale(1.05);
    }

    footer{
      background:linear-gradient(to right,#15803d,#84cc16,#fde047);
      color:white;
      text-align:center;
      padding:40px;
      border-top-left-radius:60px;
      border-top-right-radius:60px;
      margin-top:40px;
    }
  </style>
</head>
<body>

<header>
  <h1>🍦 Codesweed 🍦</h1>
  <p>✨ El auténtico sabor tropical de la guaba y más frutas exóticas ✨</p>
  <a href="#seccion-helados" class="btn">✨ Ordenar Ahora ✨</a>
</header>

<section class="titulo" id="seccion-helados">
  <h2>Nuestros Helados Especiales</h2>
  <p>Disfruta nuestros deliciosos helados artesanales elaborados con fruta natural.</p>
</section>

<section class="productos">

  <div class="card">
    <img src="imagenes/images4gu.png" alt="Helado de Guaba">
    <div class="card-content">
      <h3>Helado de Guaba</h3>
      <div class="precio">$1.00</div>
      <a href="#seccion-pedido" class="btn">🍦 Comprar Ahora 🍦</a>
    </div>
  </div>

  <div class="card">
    <img src="imagenes/heladog.png" alt="Helado de Achotillo">
    <div class="card-content">
      <h3>Helado de Achotillo</h3>
      <div class="precio">$1.00</div>
      <a href="#seccion-pedido" class="btn">🍦 Comprar Ahora 🍦</a>
    </div>
  </div>

  <div class="card">
    <img src="imagenes/mango.jpg" alt="Paleta de Mango">
    <div class="card-content">
      <h3>Paleta de Mango</h3>
      <div class="precio">$1.00</div>
      <a href="#seccion-pedido" class="btn">🍦 Comprar Ahora 🍦</a>
    </div>
  </div>

  <div class="card">
    <img src="imagenes/Paletag.png" alt="Paleta de Guaba">
    <div class="card-content">
      <h3>Paleta de Guaba</h3>
      <div class="precio">$1.00</div>
      <a href="#seccion-pedido" class="btn">🍦 Comprar Ahora 🍦</a>
    </div>
  </div>

  <div class="card">
    <img src="imagenes/paletagg.png" alt="Paleta de Achotillo">
    <div class="card-content">
      <h3>Paleta de Achotillo</h3>
      <div class="precio">$1.00</div>
      <a href="#seccion-pedido" class="btn">🍦 Comprar Ahora 🍦</a>
    </div>
  </div>

</section>

<section class="pedido" id="seccion-pedido">
  <h2>🍨 Haz tu Pedido 🍨</h2>

  <div class="opciones-pedido">
    
    <div class="columna-pedido">
      <h3>🛒 Pedido por Unidad</h3>
      <div class="subprecio">Precio regular: $1.00 c/u</div>
      
      <form>
        <input type="text" placeholder="Tu nombre" required>
        <input type="text" placeholder="Dirección de entrega" required>
        <input type="tel" placeholder="Número de teléfono" required>

        <select required>
          <option value="">Selecciona tu helado</option>
          <option>Helado de Guaba</option>
          <option>Helado de Achotillo</option>
          <option>Paleta de Mango</option>
          <option>Paleta de Guaba</option>
          <option>Paleta de Achotillo</option>
        </select>

        <textarea rows="3" placeholder="Detalles adicionales de tu pedido..."></textarea>
        <button type="submit" class="btn">✨ Enviar Pedido por Unidad ✨</button>
      </form>
    </div>

    <div class="columna-pedido">
      <h3>📦 Pedido al por Mayor</h3>
      <div class="subprecio">Precio distribuidor: $0.90 c/u (Mín. 25 unidades)</div>
      
      <form>
        <input type="text" placeholder="Nombre de tu negocio o persona" required>
        <input type="text" placeholder="Dirección de entrega" required>
        <input type="tel" placeholder="Número de teléfono" required>

        <select required>
          <option value="">¿Qué sabor deseas al por mayor?</option>
          <option>Sabor Surtido (Variados)</option>
          <option>Helado de Guaba</option>
          <option>Helado de Achotillo</option>
          <option>Paleta de Mango</option>
          <option>Paleta de Guaba</option>
          <option>Paleta de Achotillo</option>
        </select>

        <input type="number" min="25" placeholder="Cantidad de helados (Mínimo 25)" required>

        <textarea rows="2" placeholder="Instrucciones específicas para el empaque mayorista..."></textarea>
        <button type="submit" class="btn" style="background:#84cc16;">✨ Solicitar al por Mayor ✨</button>
      </form>
    </div>

  </div>
</section>

<section class="beneficios">
  <h2>🌿 ¿Por qué elegir Codesweed? 🌿</h2>

  <div class="benefit-container">
    <div class="benefit">
      <h3>🌿 Natural</h3>
      <p>Helados elaborados con fruta fresca y natural.</p>
    </div>

    <div class="benefit">
      <h3>🍨 Cremosos</h3>
      <p>Textura suave y deliciosa en cada cucharada.</p>
    </div>

    <div class="benefit">
      <h3>🚚 Delivery</h3>
      <p>Pedidos rápidos desde nuestra tienda virtual.</p>
    </div>
  </div>
</section>

<footer>
  <h2>🍦 Codesweed</h2>
  <p>📍 Tienda Virtual - San Francisco de Borja</p>
  <p>© 2026 Codesweed - Todos los derechos reservados.</p>
</footer>

</body>
</html>
