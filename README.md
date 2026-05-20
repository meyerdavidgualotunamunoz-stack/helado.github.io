# helado.github.io
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Guaba Ice</title>
  <style>
    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      font-family:Arial, sans-serif;
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
      height:250px;
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
      width:90%;
      max-width:800px;
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

    form{
      display:flex;
      flex-direction:column;
      gap:20px;
    }

    input, select, textarea{
      padding:15px;
      border-radius:20px;
      border:2px solid #bef264;
      font-size:18px;
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
  <h1>🍦 Guaba Ice 🍦</h1>
  <p>✨ El auténtico sabor tropical de la guaba ✨</p>
  <button class="btn">✨ Ordenar Ahora ✨</button>
</header>

<section class="titulo">
  <h2>Nuestros Helados Especiales</h2>
  <p>Disfruta nuestros deliciosos helados artesanales elaborados con guaba natural.</p>
</section>

<section class="productos">

  <div class="card">
    <img src="https://images.unsplash.com/photo-1497034825429-c343d7c6a68f?q=80&w=800&auto=format&fit=crop">
    <div class="card-content">
      <h3>Helado Cremoso de Guaba</h3>
      <div class="precio">$1.00</div>
      <button class="btn">🍦 Comprar Ahora 🍦</button>
    </div>
  </div>

  <div class="card">
    <img src="https://images.unsplash.com/photo-1516559828984-fb3b99548b21?q=80&w=800&auto=format&fit=crop">
    <div class="card-content">
      <h3>Paleta de Guaba</h3>
      <div class="precio">$1.00</div>
      <button class="btn">🍦 Comprar Ahora 🍦</button>
    </div>
  </div>

  <div class="card">
    <img src="https://images.unsplash.com/photo-1567206563064-6f60f40a2b57?q=80&w=800&auto=format&fit=crop">
    <div class="card-content">
      <h3>Especial Guaba</h3>
      <div class="precio">$2.00</div>
      <button class="btn">🍦 Comprar Ahora 🍦</button>
    </div>
  </div>

</section>

<section class="pedido">
  <h2>🍨 Haz tu Pedido 🍨</h2>

  <form>
    <input type="text" placeholder="Tu nombre">
    <input type="text" placeholder="Dirección de entrega">
    <input type="tel" placeholder="Número de teléfono">

    <select>
      <option>Selecciona tu helado</option>
      <option>Helado Cremoso de Guaba</option>
      <option>Paleta de Guaba</option>
      <option>Especial Guaba</option>
    </select>

    <textarea rows="4" placeholder="Escribe aquí tu pedido"></textarea>

    <button class="btn">✨ 🍦 Enviar Pedido 🍦 ✨</button>
  </form>
</section>

<section class="beneficios">
  <h2>🌿 ¿Por qué elegir Guaba Ice? 🌿</h2>

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

<section class="beneficios">
  <h2>📲 Comparte Nuestra Tienda 📲</h2>

  <div class="benefit-container">
    <div class="benefit">
      <h3>🌐 Compartir Link</h3>
      <p>Copia y envía el enlace de tu tienda a tus amigos y clientes.</p>
      <button class="btn" onclick="copiarLink()">🔗 Copiar Enlace</button>
    </div>

    <div class="benefit">
      <h3>💬 Compartir por WhatsApp</h3>
      <p>Envía tu tienda rápidamente por WhatsApp.</p>
      <button class="btn" onclick="window.open('https://wa.me/?text=Visita%20mi%20tienda%20de%20helados%20Guaba%20Ice')">📤 Compartir</button>
    </div>
  </div>
</section>

<footer>
  <h2>🍦 Guaba Ice</h2>
  <p>📍 Tienda Virtual - San Francisco de Borja</p>
  <p>© 2026 Guaba Ice - Todos los derechos reservados.</p>
</footer>

<script>
function copiarLink(){
  navigator.clipboard.writeText(window.location.href);
  alert('🔗 Enlace copiado correctamente');
}
</script>

</body>
</html>
