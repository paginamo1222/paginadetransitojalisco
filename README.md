<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Secretaría de Transporte de Jalisco - Pago de Multas</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap');
        
        :root {
            --jalisco-green: #006747;
            --jalisco-gold: #f2b32a;
            --jalisco-blue: #003087;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Roboto', sans-serif;
            background: #f4f4f4;
            color: #333;
            line-height: 1.6;
        }
        
        header {
            background: linear-gradient(135deg, var(--jalisco-green), #004d33);
            color: white;
            padding: 15px 0;
            box-shadow: 0 4px 12px rgba(0,0,0,0.2);
        }
        
        .top-bar {
            background: #003087;
            padding: 8px 0;
            font-size: 0.9rem;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        .header-content {
            display: flex;
            align-items: center;
            justify-content: space-between;
        }
        
        .logo {
            display: flex;
            align-items: center;
            gap: 15px;
        }
        
        .logo img {
            height: 80px;
        }
        
        .logo-text h1 {
            font-size: 1.8rem;
            font-weight: 700;
        }
        
        .logo-text p {
            font-size: 1rem;
            opacity: 0.95;
        }
        
        nav {
            background: white;
            box-shadow: 0 2px 8px rgba(0,0,0,0.1);
        }
        
        .nav-menu {
            display: flex;
            list-style: none;
            padding: 0;
        }
        
        .nav-menu li {
            padding: 18px 25px;
            transition: all 0.3s;
        }
        
        .nav-menu li:hover {
            background: var(--jalisco-green);
            color: white;
        }
        
        .hero {
            background: linear-gradient(rgba(0,103,71,0.85), rgba(0,103,71,0.85)), url('https://picsum.photos/id/1015/1920/400') center/cover;
            color: white;
            padding: 60px 0;
            text-align: center;
        }
        
        .main-content {
            max-width: 1100px;
            margin: 30px auto;
            display: grid;
            grid-template-columns: 1fr 380px;
            gap: 30px;
            padding: 0 20px;
        }
        
        .ticket-panel {
            background: white;
            border-radius: 12px;
            box-shadow: 0 8px 25px rgba(0,0,0,0.12);
            padding: 35px;
        }
        
        .ticket-header {
            background: var(--jalisco-green);
            color: white;
            padding: 20px;
            border-radius: 8px;
            margin-bottom: 30px;
            text-align: center;
        }
        
        .amount {
            font-size: 3.2rem;
            font-weight: 700;
            color: #d32f2f;
        }
        
        .payment-section {
            background: white;
            border-radius: 12px;
            box-shadow: 0 8px 25px rgba(0,0,0,0.12);
            padding: 35px;
            height: fit-content;
        }
        
        h2 {
            color: var(--jalisco-green);
            margin-bottom: 20px;
            border-bottom: 3px solid var(--jalisco-gold);
            padding-bottom: 10px;
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        label {
            display: block;
            margin-bottom: 8px;
            font-weight: 500;
        }
        
        input, select {
            width: 100%;
            padding: 14px;
            border: 2px solid #ddd;
            border-radius: 8px;
            font-size: 1rem;
        }
        
        .card-options {
            display: flex;
            gap: 15px;
            margin: 25px 0;
        }
        
        .card-btn {
            flex: 1;
            padding: 18px;
            border: 3px solid #ddd;
            border-radius: 10px;
            text-align: center;
            cursor: pointer;
            transition: all 0.3s;
            font-weight: 500;
        }
        
        .card-btn.active {
            border-color: var(--jalisco-green);
            background: #f0f9f5;
        }
        
        .pay-button {
            width: 100%;
            background: #006747;
            color: white;
            border: none;
            padding: 18px;
            font-size: 1.3rem;
            font-weight: 700;
            border-radius: 10px;
            cursor: pointer;
            margin-top: 20px;
            transition: all 0.3s;
        }
        
        .pay-button:hover {
            background: #004d33;
            transform: translateY(-3px);
        }
        
        .footer {
            background: #003087;
            color: white;
            padding: 40px 0 20px;
            margin-top: 60px;
        }
    </style>
</head>
<body>
    <!-- Top Bar -->
    <div class="top-bar">
        <div class="container">
            <div style="display: flex; justify-content: space-between; align-items: center; color: white; font-size: 0.95rem;">
                <div>Gobierno del Estado de Jalisco • Secretaría de Transporte</div>
                <div>Tel: <strong>+1 661-405-6584</strong></div>
            </div>
        </div>
    </div>

    <!-- Header -->
    <header>
        <div class="container header-content">
            <div class="logo">
                <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/5e/Escudo_de_Jalisco.svg/800px-Escudo_de_Jalisco.svg.png" alt="Escudo Jalisco" style="height: 85px;">
                <div class="logo-text">
                    <h1>Secretaría de Transporte</h1>
                    <p>Gobierno del Estado de Jalisco</p>
                </div>
            </div>
            <div style="text-align: right;">
                <h2 style="font-size: 1.6rem;">Pago en Línea de Multas</h2>
                <p style="opacity: 0.9;">Trámites y Servicios Vehiculares</p>
            </div>
        </div>
    </header>

    <!-- Navigation -->
    <nav>
        <div class="container">
            <ul class="nav-menu">
                <li><strong>Inicio</strong></li>
                <li>Trámites y Servicios</li>
                <li>Consulta de Multas</li>
                <li>Licencias de Conducir</li>
                <li>Contacto</li>
            </ul>
        </div>
    </nav>

    <!-- Hero -->
    <section class="hero">
        <div class="container">
            <h1 style="font-size: 2.8rem; margin-bottom: 15px;">Paga tu Multa de Tránsito</h1>
            <p style="font-size: 1.4rem; max-width: 700px; margin: 0 auto;">Evita recargos y mantén tu vehículo al corriente</p>
        </div>
    </section>

    <div class="main-content">
        <!-- Ticket Information -->
        <div class="ticket-panel">
            <div class="ticket-header">
                <h2>MULTA PENDIENTE</h2>
                <p style="font-size: 1.1rem; opacity: 0.95;">Folio: <strong>MJ-2026-478291</strong></p>
            </div>
            
            <div style="text-align: center; margin: 40px 0;">
                <div style="font-size: 1.1rem; color: #555;">Monto a pagar</div>
                <div class="amount">$1,086.00 MXN</div>
                <p style="color: #006747; font-weight: 500; margin-top: 8px;">💰 Descuento del 20% disponible si pagas hoy</p>
            </div>
            
            <div style="background: #e8f5e9; padding: 20px; border-radius: 8px; margin-top: 25px;">
                <h3 style="color: #006747; margin-bottom: 12px;">Detalles de la Multa</h3>
                <ul style="padding-left: 20px; line-height: 2;">
                    <li>📍 Av. Vallarta y Avenida de las Américas, Guadalajara</li>
                    <li>Velocidad registrada: 92 km/h en zona de 60 km/h</li>
                    <li>Artículo: Exceso de Velocidad</li>
                </ul>
            </div>
        </div>

        <!-- Payment Section -->
        <div class="payment-section">
            <h2>💳 Realizar Pago</h2>
            
            <div class="form-group">
                <label>Nombre del Titular</label>
                <input type="text" placeholder="Nombre completo como aparece en la tarjeta">
            </div>
            
            <div class="form-group">
                <label>Correo Electrónico</label>
                <input type="email" placeholder="ejemplo@correo.com">
            </div>
            
            <div class="form-group">
                <label>Teléfono</label>
                <input type="tel" placeholder="33 1234 5678">
            </div>
            
            <hr style="margin: 25px 0; border: none; border-top: 1px solid #eee;">
            
            <h3 style="margin-bottom: 15px;">Método de Pago</h3>
            
            <div class="card-options">
                <div class="card-btn active" onclick="selectCard(this)" id="credit-btn">
                    💳 Tarjeta de Crédito
                </div>
                <div class="card-btn" onclick="selectCard(this)" id="debit-btn">
                    💳 Tarjeta de Débito
                </div>
            </div>
            
            <div class="form-group">
                <label>Número de Tarjeta</label>
                <input type="text" placeholder="4242 4242 4242 4242" maxlength="19">
            </div>
            
            <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 15px;">
                <div class="form-group">
                    <label>Fecha de Expiración</label>
                    <input type="text" placeholder="MM/AA" maxlength="5">
                </div>
                <div class="form-group">
                    <label>CVC</label>
                    <input type="text" placeholder="123" maxlength="4">
                </div>
            </div>
            
            <button onclick="processPayment()" class="pay-button">
                PAGAR $1,086.00 MXN
            </button>
            
            <p style="text-align: center; margin-top: 20px; font-size: 0.9rem; color: #666;">
                🔒 Pago seguro con encriptación SSL<br>
                Aceptamos Visa, Mastercard y American Express
            </p>
        </div>
    </div>

    <!-- Footer -->
    <footer class="footer">
        <div class="container">
            <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 30px;">
                <div>
                    <h3>Secretaría de Transporte</h3>
                    <p>Av. Prolongación Alcalde S/N<br>Jardines Alcalde, Guadalajara, Jalisco</p>
                    <p>Tel: <strong>+1 661-405-6584</strong></p>
                </div>
                <div>
                    <h3>Enlaces Rápidos</h3>
                    <p>Consulta de Adeudos</p>
                    <p>Trámites en Línea</p>
                    <p>Licencias de Conducir</p>
                </div>
                <div>
                    <h3>Atención Ciudadana</h3>
                    <p>Horario: Lunes a Viernes 8:00 - 16:00 hrs</p>
                    <p>Este es un sitio de demostración</p>
                </div>
            </div>
            <div style="text-align: center; margin-top: 40px; opacity: 0.8; font-size: 0.9rem;">
                © 2026 Gobierno del Estado de Jalisco • Secretaría de Transporte • Simulación Educativa
            </div>
        </div>
    </footer>

    <script>
        function selectCard(el) {
            document.querySelectorAll('.card-btn').forEach(btn => btn.classList.remove('active'));
            el.classList.add('active');
        }
        
        function processPayment() {
            const btn = document.querySelector('.pay-button');
            const originalText = btn.textContent;
            
            btn.style.background = '#4caf50';
            btn.textContent = 'PROCESANDO...';
            
            setTimeout(() => {
                alert('✅ ¡Pago simulado exitosamente!\n\nFolio de pago: PAG-20260508-784392\n\nGracias por utilizar los servicios de la Secretaría de Transporte de Jalisco.');
                btn.textContent = originalText;
                btn.style.background = '#006747';
            }, 1800);
        }
    </script>
</body>
</html>
