# Redes.1.html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>¡Gran Rifa Semanal 100! 💰</title>
    <style>
        html, body {
            margin: 0;
            padding: 0;
            width: 100%;
            min-height: 100%;
            font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
            background: radial-gradient(circle at top, #1e1b4b, #0f172a, #020617); /* Fondo galáctico/casino profundo */
            color: #ffffff;
            overflow-x: hidden;
        }
        
        .hero-container {
            width: 100%;
            box-sizing: border-box;
            padding: 30px 20px;
            text-align: center;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        /* Animación de parpadeo neón para el título */
        @keyframes pulso {
            0% { transform: scale(1); text-shadow: 0 0 10px #38bdf8; }
            50% { transform: scale(1.03); text-shadow: 0 0 25px #06b6d4, 0 0 40px #3b82f6; }
            100% { transform: scale(1); text-shadow: 0 0 10px #38bdf8; }
        }

        .emoji-principal {
            font-size: 60px;
            margin-bottom: 10px;
            filter: drop-shadow(0 0 15px rgba(234, 179, 8, 0.6));
        }

        h1 {
            font-size: 32px;
            font-weight: 900;
            text-transform: uppercase;
            letter-spacing: 1px;
            margin: 0 0 10px 0;
            background: linear-gradient(to right, #38bdf8, #60a5fa, #c084fc);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: pulso 3s infinite ease-in-out;
        }

        .tagline {
            font-size: 16px;
            color: #94a3b8;
            max-width: 320px;
            line-height: 1.4;
            margin-bottom: 30px;
        }

        /* Cartel de Pozo Enorme y Adictivo */
        .mega-pozo-box {
            background: linear-gradient(135deg, rgba(30, 58, 138, 0.9), rgba(147, 51, 234, 0.4));
            border: 2px solid #a855f7;
            border-radius: 24px;
            padding: 25px 20px;
            width: 90%;
            max-width: 360px;
            box-sizing: border-box;
            box-shadow: 0 0 30px rgba(168, 85, 247, 0.4), inset 0 0 15px rgba(255,255,255,0.1);
            position: relative;
            margin-bottom: 35px;
        }

        .pozo-tag {
            position: absolute;
            top: -12px;
            left: 50%;
            transform: translateX(-50%);
            background: #eab308;
            color: #0f172a;
            font-size: 11px;
            font-weight: 900;
            padding: 4px 12px;
            border-radius: 20px;
            text-transform: uppercase;
            letter-spacing: 1px;
            box-shadow: 0 4px 10px rgba(234, 179, 8, 0.4);
        }

        .pozo-texto {
            font-size: 14px;
            color: #e9d5ff;
            text-transform: uppercase;
            letter-spacing: 2px;
            margin-top: 5px;
        }

        .pozo-monto {
            font-size: 42px;
            font-weight: 900;
            color: #ffffff;
            margin: 10px 0;
            text-shadow: 0 2px 10px rgba(0,0,0,0.5);
            letter-spacing: -1px;
        }

        .pozo-sub {
            font-size: 13px;
            color: #f472b6;
            font-weight: 600;
        }

        /* Grid de Beneficios / Datos clave rápidos */
        .caracteristicas {
            width: 90%;
            max-width: 360px;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 12px;
            margin-bottom: 35px;
        }

        .card {
            background: rgba(30, 41, 59, 0.7);
            border: 1px solid #334155;
            padding: 15px 10px;
            border-radius: 16px;
            text-align: center;
        }
        .card-icono { font-size: 24px; margin-bottom: 5px; }
        .card-t { font-size: 13px; color: #94a3b8; font-weight: 500; }
        .card-v { font-size: 16px; color: #f1f5f9; font-weight: 700; margin-top: 3px; }

        /* BOTÓN DE ACCIÓN PRINCIPAL MAGNETICO */
        @keyframes latido {
            0% { transform: scale(1); box-shadow: 0 4px 20px rgba(37, 211, 102, 0.4); }
            50% { transform: scale(1.05); box-shadow: 0 4px 30px rgba(37, 211, 102, 0.8); }
            100% { transform: scale(1); box-shadow: 0 4px 20px rgba(37, 211, 102, 0.4); }
        }

        .btn-jugar {
            display: block;
            width: 90%;
            max-width: 360px;
            box-sizing: border-box;
            background: linear-gradient(135deg, #22c55e, #16a34a);
            color: #ffffff;
            text-decoration: none;
            font-size: 20px;
            font-weight: 800;
            padding: 20px;
            border-radius: 50px; /* Bordes bien redondeados tipo cápsula moderna */
            text-transform: uppercase;
            letter-spacing: 1px;
            animation: latido 2s infinite ease-in-out;
            border: 2px solid #4ade80;
            text-shadow: 0 1px 3px rgba(0,0,0,0.3);
        }

        .btn-subtexto {
            font-size: 12px;
            color: #64748b;
            margin-top: 12px;
            font-weight: 500;
        }
    </style>
</head>
<body>

<div class="hero-container">
    <div class="emoji-principal">👑</div>
    <h1>¡Tu Suerte Te Espera!</h1>
    <div class="tagline">Elegí tu número hoy, jugamos este fin de semana con la Lotería Oficial. ¡Quedan pocos lugares!</div>

    <!-- EL GANCHO CENTRAL: EL POZO ACUMULADO -->
    <div class="mega-pozo-box">
        <div class="pozo-tag">🔥 RECAUDACIÓN EN VIVO</div>
        <div class="pozo-texto">Pozo Estimado Actual</div>
        <!-- PONÉ ACÁ EL MONTO A MANO PARA HACERLO ATRACTIVO SI QUERÉS, O DEJA UN ESTIMADO BASE -->
        <div class="pozo-monto">$75.000</div>
        <div class="pozo-sub">¡Si queda vacante, SE ACUMULA! 🚀</div>
    </div>

    <!-- BENEFICIOS / REGLAS RÁPIDAS -->
    <div class="caracteristicas">
        <div class="card">
            <div class="card-icono">🎟️</div>
            <div class="card-t">Solo hay</div>
            <div class="card-v">100 Números</div>
        </div>
        <div class="card">
            <div class="card-icono">💎</div>
            <div class="card-t">Valor Número</div>
            <div class="card-v">$5.000</div>
        </div>
        <div class="card">
            <div class="card-icono">🎰</div>
            <div class="card-t">Transparente</div>
            <div class="card-v">Lotería Oficial</div>
        </div>
        <div class="card">
            <div class="card-icono">⚡</div>
            <div class="card-t">Premio Neto</div>
            <div class="card-v">50% de Todo</div>
        </div>
    </div>

    <!-- EL BOTÓN QUE LOS LLEVA A COMPRAR -->
    <!-- ⚠️ REEMPLAZÁ EL LINK DE ABAJO POR EL LINK REAL DE TU TABLERO DE RIFAS -->
    <a href="https://TU_USUARIO.github.io/mi-rifa-digital/index.html" class="btn-jugar">
        🍀 VER NÚMEROS DISPONIBLES
    </a>
    
    <div class="btn-subtexto">Tocá para abrir el tablero táctil y reservar tu número de la suerte</div>
</div>

</body>
</html>
