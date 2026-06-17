
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>¡Gran Rifa Semanal Digital! 💰</title>
    
    <!-- Configuración para Redes Sociales (Facebook, Insta, WhatsApp) -->
    <meta property="og:type" content="website">
    <meta property="og:title" content="👑 ¡GRAN RIFA SEMANAL DIGITAL! 💰">
    <meta property="og:description" content="🎰 ¡Solo 100 números! Elegí tu número de la suerte en tiempo real. ¡El pozo está acumulado y crece sin parar! 🔥">
    <meta property="og:url" content="https://gerardoantao.github.io/Redes.rifa/redes.html">
    <meta property="og:image" content="https://gerardoantao.github.io/Redes.rifa/preview.jpg">

    <style>
        html, body {
            margin: 0;
            padding: 0;
            width: 100%;
            min-height: 100%;
            font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
            background: radial-gradient(circle at top, #1e1b4b, #0b0f19, #020617);
            color: #ffffff;
            overflow-x: hidden;
        }
        
        .hero-container {
            width: 100%;
            box-sizing: border-box;
            padding: 40px 20px;
            text-align: center;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        /* Título Neón con animación de pulso continuo */
        @keyframes pulsoNeon {
            0% { text-shadow: 0 0 10px #38bdf8, 0 0 20px #3b82f6; transform: scale(1); }
            50% { text-shadow: 0 0 25px #06b6d4, 0 0 50px #6366f1, 0 0 70px #a855f7; transform: scale(1.02); }
            100% { text-shadow: 0 0 10px #38bdf8, 0 0 20px #3b82f6; transform: scale(1); }
        }

        .emoji-principal {
            font-size: 65px;
            margin-bottom: 15px;
            filter: drop-shadow(0 0 20px #eab308);
            animation: flotar 3s infinite ease-in-out;
        }

        @keyframes flotar {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
            100% { transform: translateY(0px); }
        }

        h1 {
            font-size: 34px;
            font-weight: 900;
            text-transform: uppercase;
            letter-spacing: 1px;
            margin: 0 0 12px 0;
            background: linear-gradient(to right, #38bdf8, #818cf8, #c084fc);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: pulsoNeon 2.5s infinite ease-in-out;
        }

        .tagline {
            font-size: 16px;
            color: #94a3b8;
            max-width: 340px;
            line-height: 1.5;
            margin-bottom: 35px;
        }

        /* CARTEL DEL POZO: Reacciona con brillo al pasar el mouse/dedo */
        .mega-pozo-box {
            background: linear-gradient(135deg, rgba(30, 58, 138, 0.8), rgba(147, 51, 234, 0.4));
            border: 2px solid #a855f7;
            border-radius: 24px;
            padding: 30px 20px;
            width: 95%;
            max-width: 380px;
            box-sizing: border-box;
            box-shadow: 0 0 25px rgba(168, 85, 247, 0.3);
            position: relative;
            margin-bottom: 40px;
            transition: all 0.4s ease; /* Hace que el movimiento sea suave */
            cursor: default;
        }

        /* Efecto cuando pasan el cursor por arriba del pozo */
        .mega-pozo-box:hover {
            transform: translateY(-5px) scale(1.02);
            box-shadow: 0 0 40px rgba(168, 85, 247, 0.7), inset 0 0 20px rgba(255, 255, 255, 0.2);
            border-color: #c084fc;
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
            padding: 5px 14px;
            border-radius: 20px;
            text-transform: uppercase;
            letter-spacing: 1px;
            box-shadow: 0 4px 12px rgba(234, 179, 8, 0.5);
        }

        .pozo-texto {
            font-size: 14px;
            color: #e9d5ff;
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        /* Dinero titilante de casino real */
        .pozo-monto {
            font-size: 46px;
            font-weight: 900;
            color: #ffffff;
            margin: 12px 0;
            text-shadow: 0 4px 15px rgba(0, 0, 0, 0.6);
            letter-spacing: -1px;
            background: linear-gradient(to bottom, #ffffff, #f3e8ff);
            -webkit-background-clip: text;
        }

        .pozo-sub {
            font-size: 13px;
            color: #f472b6;
            font-weight: 600;
            letter-spacing: 0.5px;
        }

        /* GRID DE BENEFICIOS INTERACTIVOS */
        .caracteristicas {
            width: 95%;
            max-width: 380px;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 14px;
            margin-bottom: 40px;
        }

        .card {
            background: rgba(30, 41, 59, 0.6);
            border: 1px solid #334155;
            padding: 18px 12px;
            border-radius: 20px;
            text-align: center;
            transition: all 0.3s ease;
        }

        /* Movimiento reactivo en las tarjetas fijas */
        .card:hover {
            background: rgba(47, 55, 87, 0.8);
            border-color: #38bdf8;
            transform: scale(1.05);
            box-shadow: 0 10px 20px rgba(56, 189, 248, 0.2);
        }

        .card-icono { font-size: 26px; margin-bottom: 6px; }
        .card-t { font-size: 13px; color: #94a3b8; font-weight: 500; }
        .card-v { font-size: 17px; color: #f1f5f9; font-weight: 700; margin-top: 3px; }

        /* EL ÚNICO BOTÓN CON LINK REAL (EL BOTÓN QUE LATE) */
        @keyframes latidoVerde {
            0% { transform: scale(1); box-shadow: 0 4px 25px rgba(34, 197, 94, 0.4); }
            50% { transform: scale(1.04); box-shadow: 0 4px 35px rgba(34, 197, 94, 0.8); border-color: #ffffff; }
            100% { transform: scale(1); box-shadow: 0 4px 25px rgba(34, 197, 94, 0.4); }
        }

        .btn-jugar {
            display: block;
            width: 95%;
            max-width: 380px;
            box-sizing: border-box;
            background: linear-gradient(135deg, #22c55e, #15803d);
            color: #ffffff;
            text-decoration: none;
            font-size: 20px;
            font-weight: 800;
            padding: 22px;
            border-radius: 50px; 
            text-transform: uppercase;
            letter-spacing: 1px;
            animation: latidoVerde 1.8s infinite ease-in-out;
            border: 2px solid #4ade80;
            text-shadow: 0 2px 4px rgba(0,0,0,0.4);
            transition: all 0.2s ease;
        }

        /* Cuando pasan el mouse arriba del botón verde, se ilumina más fuerte aún */
        .btn-jugar:hover {
            transform: scale(1.06);
            background: linear-gradient(135deg, #4ade80, #16a34a);
            cursor: pointer;
        }

        .btn-subtexto {
            font-size: 13px;
            color: #64748b;
            margin-top: 15px;
            font-weight: 500;
        }
    </style>
</head>
<body>

<div class="hero-container">
    <div class="emoji-principal">👑</div>
    <h1>¡Tu Suerte Te Espera!</h1>
    <div class="tagline">Elegí tu número hoy, jugamos este fin de semana con la Lotería Oficial. ¡No te quedes afuera!</div>

    <!-- EL POZO - NO TIENE LINK, SOLO REACCIONA VISUALMENTE -->
    <div class="mega-pozo-box">
        <div class="pozo-tag">🔥 POZO EN TIEMPO REAL</div>
        <div class="pozo-texto">Monto Acumulado</div>
        <!-- Cambiá este número a mano cuando quieras actualizar el pozo -->
        <div class="pozo-monto">$75.000</div>
        <div class="pozo-sub">¡Si queda vacante, SE ACUMULA! 🚀</div>
    </div>

    <!-- CARACTERÍSTICAS - NO TIENEN LINK, SE MUEVEN AL COLOCOAR EL CURSOR -->
    <div class="caracteristicas">
        <div class="card">
            <div class="card-icono">🎟️</div>
            <div class="card-t">Cupo Máximo</div>
            <div class="card-v">100 Números</div>
        </div>
        <div class="card">
            <div class="card-icono">💎</div>
            <div class="card-t">Valor Número</div>
            <div class="card-v">$5.000</div>
        </div>
        <div class="card">
            <div class="card-icono">🎰</div>
            <div class="card-t">Transparencia</div>
            <div class="card-v">Lotería Oficial</div>
        </div>
        <div class="card">
            <div class="card-icono">⚡</div>
            <div class="card-t">Premio Neto</div>
            <div class="card-v">50% Recaudado</div>
        </div>
    </div>

    <!-- ⚠️ EL ÚNICO BOTÓN QUE TIENE LINK ELÉCTRICO PARA IR AL TABLERO -->
    <!-- Reemplazá la frase de abajo por el link real de tu tablero rifa.html -->
    <a href="https://gerardoantao.github.io/mi-rifa-digital/" class="btn-jugar">
        🍀 VER NÚMEROS DISPONIBLES
    </a>
    
    <div class="btn-subtexto">Tocá para abrir el tablero interactivo y reservar tu número</div>
</div>

</body>
</html>
