<!DOCTYPE html>
<html lang="es">
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wiki | Método científico</title>
    <style>
        :root {
            --morado: #51217a;
            --morado-oscuro: #35134f;
            --lila: #eee5f6;
            --fondo: #f7f5fa;
            --texto: #30283a;
            --borde: #e4dbea;
        }
        * { box-sizing: border-box; }
        html { scroll-behavior: smooth; scroll-padding-top: 90px; }
        body {
            margin: 0;
            font-family: "Segoe UI", Arial, sans-serif;
            background: var(--fondo);
            color: var(--texto);
            line-height: 1.7;
        }
        header {
            background: linear-gradient(135deg, var(--morado-oscuro), #8050a5);
            color: white;
            padding: 34px 20px;
            text-align: center;
        }
        header h1 { margin: 0; letter-spacing: 2px; font-size: clamp(1.8rem, 4vw, 2.8rem); }
        nav {
            background: #fff;
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 8px;
            padding: 12px 18px;
            box-shadow: 0 3px 12px rgba(40, 20, 55, .08);
            position: sticky;
            top: 0;
            z-index: 10;
        }
        nav a, aside a {
            color: var(--morado);
            text-decoration: none;
            font-weight: 650;
        }
        nav a { padding: 8px 12px; border-radius: 8px; }
        nav a:hover, aside a:hover { background: var(--lila); color: var(--morado-oscuro); }
        .contenedor {
            width: min(1400px, 100%);
            margin: 28px auto;
            padding: 0 20px;
            display: grid;
            grid-template-columns: 250px minmax(0, 1fr);
            gap: 24px;
            align-items: start;
        }
        aside {
            background: white;
            border: 1px solid var(--borde);
            border-radius: 14px;
            padding: 22px 18px;
            position: sticky;
            top: 86px;
            max-height: calc(100vh - 110px);
            overflow-y: auto;
        }
        aside h2 { color: var(--morado); font-size: 1.2rem; margin: 0 0 12px; }
        aside ul { list-style: none; margin: 0; padding: 0; }
        aside li { margin: 4px 0; }
        aside a { display: block; padding: 7px 9px; border-radius: 7px; font-size: .93rem; }
        main {
            min-width: 0;
            background: white;
            padding: clamp(20px, 4vw, 42px);
            border: 1px solid var(--borde);
            border-radius: 16px;
            box-shadow: 0 8px 28px rgba(47, 23, 61, .07);
        }
        section {
            display: block;
            scroll-margin-top: 90px;
            padding-bottom: 24px;
            margin-bottom: 28px;
            border-bottom: 1px solid var(--borde);
        }
        section:last-child { border-bottom: 0; }
        main h2 {
            color: var(--morado);
            font-size: clamp(1.35rem, 2.5vw, 1.8rem);
            line-height: 1.3;
            margin: 0 0 18px;
            padding-bottom: 12px;
            border-bottom: 2px solid var(--lila);
        }
        main h3 {
            color: #6a348b;
            font-size: 1.12rem;
            line-height: 1.4;
            margin: 28px 0 10px;
        }
        main p { margin: 0 0 16px; overflow-wrap: anywhere; white-space: pre-line; }
        main p:has(+ h3) { margin-bottom: 18px; }
        .imagen, main img {
            display: block;
            max-width: 100%;
            height: auto;
            margin: 20px auto;
            border-radius: 12px;
            object-fit: contain;
            box-shadow: 0 4px 16px rgba(30, 15, 40, .12);
        }
        .imagen { width: 100%; max-height: 360px; object-fit: cover; }
        .info {
            background: #f4edf9;
            border-left: 5px solid var(--morado);
            padding: 16px 18px;
            margin: 22px 0;
            border-radius: 0 10px 10px 0;
        }
        ul, ol { padding-left: 25px; }
        li { margin-bottom: 5px; }
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 18px 0;
            display: block;
            overflow-x: auto;
        }
        th, td { border: 1px solid var(--borde); padding: 10px 12px; text-align: left; }
        th { background: var(--lila); color: var(--morado-oscuro); }
        footer {
            background: #281a32;
            color: white;
            text-align: center;
            padding: 24px 18px;
            margin-top: 34px;
        }
        footer p { margin: 0; }
        @media (max-width: 850px) {
            .contenedor { grid-template-columns: 1fr; margin-top: 16px; padding: 0 12px; }
            aside { position: static; max-height: none; }
            aside ul { display: grid; grid-template-columns: repeat(auto-fit, minmax(180px, 1fr)); gap: 3px; }
            main { padding: 22px 18px; }
            nav { position: static; }
        }
        @media (max-width: 480px) {
            header { padding: 25px 14px; }
            nav a { font-size: .9rem; padding: 7px 9px; }
            main { padding: 18px 14px; }
        }
    </style>
</head>
</head>

<body>

    <header>
        <h1>MI WIKI</h1>
    </header>

    <!-- MENU PRINCIPAL -->
    <nav>
        <a href="#INICIO">INICIO</a>
        <a href="#PORTADA">PORTADA</a>
        <a href="#INTRODUCCION">INTRODUCCIÓN</a>
        <a href="#desarrollo">DESARROLLO</a>
        <a href="#conclusion">CONCLUSIÓN</a>
    </nav>

    <div class="contenedor">

        <!-- MENU LATERAL -->
        <aside>
            <h2>Contenido</h2>
            <ul>
                <li><a href="#INICIO">Inicio</a></li>
                <li><a href="#PORTADA">Portada y participantes</a></li>
                <li><a href="#INTRODUCCION">Introducción</a></li>
                <li><a href="#desarrollo">Desarrollo de la actividad</a></li>
            </ul>
        </aside>

        <main>

            <!-- INICIO -->
            <section id="INICIO">
                <h2>¿LA ARGUMENTACIÓN: PERCEPCIÓN Y REPRESENTACIÓN?</h2>

                <p>
                    EL OBJETIVO ES DESCRIBIR LOS ELEMENTOS QUE INTEGRAN
                    LA PERCEPCIÓN Y LA REPRESENTACIÓN EN EL MÉTODO CIENTÍFICO.
                </p>

                <img
                    class="imagen"
                    src="https://tse4.mm.bing.net/th/id/OIP.ufFYZH1TGWzimZyOwE4HLAHaFf?r=0&rs=1&pid=ImgDetMain&o=7&rm=3"
                    alt="Imagen sobre argumentación, percepción y representación">

                <div class="info">
                    <strong>Dato importante:</strong>
                    El orden y diseño de tu presentación cambian la percepción
                    del público antes de que evalúen la lógica de tu argumento.
                </div>
            </section>

            <!-- PORTADA -->
            <section id="PORTADA">
                <h2>PORTADA</h2>

                <p><strong>ACTIVIDAD 18</strong></p>

                <p><strong>NOMBRE DE LOS PARTICIPANTES:</strong></p>

                <ul>
                    <li>Abril Monserrath Graciada Castro</li>
                    <li>Brenda Paola Hinojosa Platas</li>
                    <li>Aranza Marely Paez Enguilo</li>
                    <li>Brisa Guadalupe Perez Gerardo</li>
                    <li>Beatriz Rosas Becerril</li>
                    <li>Arleth Azalia Zagazeta Linares</li>
                </ul>
            </section>

            <!-- INTRODUCCION -->
            <section id="INTRODUCCION">
                <h2>INTRODUCCIÓN</h2>

                <p>
                    La argumentación, la percepción y la representación son
                    elementos importantes en el método científico. La percepción
                    permite observar e interpretar la realidad mediante los
                    sentidos, mientras que la representación ayuda a expresar
                    lo observado por medio de palabras, imágenes, modelos o
                    esquemas. La argumentación permite explicar y defender
                    ideas utilizando razones y evidencias.
                </p>

                <p>
                    Estos elementos se relacionan porque permiten analizar
                    información, construir explicaciones y comunicar
                    conocimientos de manera clara y fundamentada.
                </p>
            </section>

            <!-- DESARROLLO DE LA ACTIVIDAD -->
            <section id="desarrollo">
                <h2>DESARROLLO DE LA ACTIVIDAD</h2>

                <h3>PAPEL DE LA PERCEPION Y LA REPRESENTACION EN EL METODO CIENTIFICO</h3>
                <p>
                    Es el proceso mediante el cual captamos la realidad a través de los sentidos (vista, oído, tacto, etc.) y la integramos con ayuda de nuestra mente. 
                    En ciencia, no es solo "ver", sino observar de forma intencional, sistemática y crítica.
                    La percepción es el primer contacto con la realidad. Sin ella no hay datos, no hay hechos 
                    que explicar ni problemas que resolver.


                    Funciones de la percepción
                    - Detectar fenómenos: nos permite identificar lo que vamos a estudiar.
                    - Generar preguntas: al observar algo que no entendemos, surge la curiosidad y el problema de investigación.
                    - Recopilar información: aporta los datos empíricos, la base real de todo conocimiento científico.
                    - Orientar la investigación: una buena observación nos ayuda a plantear hipótesis.

                    La percepción no es neutral. Influyen nuestros conocimientos previos, creencias y la 
                    teoría que manejamos. Por eso, en ciencia se usa la observación controlada 
                    (instrumentos, mediciones, registros) para reducir errores.

                    ¿Qué es la representación en el método científico?
                    Es la capacidad de traducir lo percibido a lenguaje, símbolos, conceptos, 
                    modelos o imágenes para hacerlo comprensible, ordenado y comunicable.

                    Lo que percibimos es caótico y particular; la representación lo convierte en
                    ideas estructuradas y compartibles.

                    Funciones de la representación:
                    - Dar orden: organiza lo observado en categorías, conceptos o explicaciones.
                    - Comunicar: permite que otros entiendan lo que descubrimos (informes, gráficos, fórmulas).
                    - Razonar: solo con ideas claras podemos deducir, predecir y relacionar.
                    - Construir conocimiento: integra lo observado con lo que ya sabemos.

                    Formas de representación:

                    - Conceptos y definiciones
                    - Descripciones verbales
                    - Gráficos, tablas y esquemas
                    - Fórmulas matemáticas
                    - Modelos y diagramas

                    ¿Cómo se relacionan?

                    Percepción Representación
                    Capta la realidad Expresa lo captado
                    Datos concretos Ideas estructuradas
                    Base empírica Base conceptual
                    Responde: ¿Qué vemos? Responde: ¿Cómo lo explicamos?

                    Ciclo continuo:

                    Percepción
                    Representación 
                    Razonamiento
                    Nueva percepción
                    Nueva representación...

                    La percepción aporta el contenido real; la representación aporta la forma comprensible. 
                    Sin percepción, la ciencia estaría desconectada de la realidad. Sin representación, lo 
                    observado no podría analizarse ni transmitirse.
                    </p>

                    <img src="data:image/webp;base64,UklGRtwqAABXRUJQVlA4INAqAADwhwCdASpcAeoAPp1CnEolo6YkqhdqwMATiWRu8o5wbMW/yvbkCMtUd/AP13no8m95Pv37t+yPjfwjOjv7Hmk85f931vf6/1eeYN+r36/9dHzI/t/6tnpb/qfqMf3X/o9bR6Dvl1ful8RH9v/7Hpb6ox9C7n/7f/yfD3yX+yvdn4u8E9p31jflf4X28/xf67+Kvxt+h/YF9e7rbsf/E9Aj2J+4/9v01Plv+96BfYr2AP5x/cP+d6//7jwWvtn+n/73+5+AL+bf27/1f4L3g/8b9ufP19Y+wT/Qv8F1o/3m///u0/t1//zoPJni/H3vRF8tLpfpN9T1k1qQs9GBEzF1Rs7E6Fss236KQ/6fh4a4vJvEAQnYjb9mKgpYk2NlD4lOHfiuvof7OcFAKEfaSsG9QGo+PDW4UVti7PskhARH8NdMh2Tg1WEXdKz9DPBSJf0a+nK++zwjsYTB+XEefdUPN7dP/45zFOSBS4NwJb6tG2B1GBVHNTTaeMkSU4klRaOZ4FkQHq5xD0MNGjKeXihizJ26OkMRiwhze7iSBLvyWaR6hm44hwmpZy7YOHa2yXjM0EQo9ys9k1Uw9HHDhJ4ktFlh5M1BrnzgRFQWLjYiezGUJ9Yj1DAZ6RKAWfyDujaHLv66nzBY7t19ZVsWjbWJ7Lg2V/Vp7Pzv6sOW76U7tZnADD4fx2Y6PPEKEfq3cflVL0vInokpDHas0bf4bJGfpsrkWRq0R/3qMTP+u+X/7t+EA0BLnDcrKhtkAWklo3S5nsvUEy/pZbfZCMdswMLuJxGXEJHwz1l0FhLzeLwnoGvhsf9ikC/fFwPzTV/rOhj4g6nc0ypuZhuOCBJ+VjBkWJ6V1ESITYnIUnva+msJ3iOWGRWkqPWP4olIfpQQU3qFShjzly2mQrnM30tcZ/9zaFvRJMCOUCLP6/FYiXsu/oD+bpLiAkFxofsw6Dh2cp0nRjzM7N9HYDV5SwI7+0exXTKInDV31PHcxKFwTKfNmy95dcUe+ZYWYbr0IPO292S+redktzc7/jrgV33DiAQzfByDrZOzdXbsu0gZuiqWRhnSfADNx3KhED+ghjfi8jz6F+P+BPiuswFr4L4ASE4Eq3JdFIeTuxYOzCmzmykSO6HUPWZApB3Xqedam7tmct3ASPsoApNWN5v3OK1hLwCn1QZzr8IU+vtdK3PDXjPwfi7Mx5TVCAGNAbGla/Ne3ffS7IdvgMsJZC3qPGvmJVu/XO1Nn7S45TKJJVPGdR8zaWdKF4kptqng5+uwngIRU9cqOR9p79aXu3MGD8s269cd+3PnjAgWOh8fNDfFjx3cGLeZFeHVnvW6ZYu5QLkb2uFqr/YnqZ0WRqchprlYip2ZVxMzFkWunBEO2H+4dNkQysOYMaQHUuHajhkLoHTxC3fu7/70Jvr7XfzW6U3+ZhCmXSH5IbNj11VSctCz00AeDnX2SERpODMAAP7Nnn/+Hd9n/vaSx//k/ftt+GrOLA8l7joZMXJHDB/38QsNDbVeTsqXXnBMO8s/UP5+3qdqL34iPP8DwC4kpT2FnFp0yaTZqvYcOWjD05K6kGuhKAw7KnnNxS9bcdu6B/wu1bZKRmVMLnffjtZPDKUskZ/4j6m5jMdv0rgJDq59O0y7rLmbCgSjNL5c3nV1WrkYqK5PvIOZDknADWGKVglueVN1O8lYTlW6hXLtjaem6edAw+F+cWWk45en0zGWZn+RMxjxRvpTwb5Ih7W9pP5w9XMy0YA8Tu5fm09qpDEz0es0yQo3+p2hX18NfGtlPpRa4++6pd6O0AiylDuArLVbhBEtPgr0etbi4pGxbCwF9HLl6p1+TwT/C5dY6tzCJh8bXv3Tb/pGehMeIF2XKD/jtCyIoHEhv5SE9NMgWUaX6m+1kT9n3WA+PInIYesCeHaVSPsyLsXdna/ZD4/Pf2Glg237CoHhagbZE+bjHrqiJZp35O7AVwSBLkN4ksFFJdeo5tWt8/rUXfa00iShsgTn7N7/odegKJxRbFfP25ymubCM3Mcz/1+/Xht9xvoyjQjrTmlFlEmBfDOvDmlqVpzXp2DSwzbnCLkhw66oTITkxBnutNhiX4lRs/YWlB+8tKvb+UAug+LtbURbgbO6sbiGT0BrI7G4/K7MspvbJ8ua3Tx+l4l/BJfJKJ/GOyy22FRAGkQM48D/ytpSvzJcKyBCpf3iA76/ienO3l6sTKXVyUSC4UhLj5pXQCB9RRxftqkgAXYaTCyKDGMkrbYH1kpXWcEerX6Fr/VgpvVlpof0ibGOcvdVu9A/uS6CIQwNL4u0xDrC5TQwhgHxo/kPXJSh+TQGceOP51TLjMGqv/B43m63w4uR5B9MOZEPvbvyzvH2iPBsx67GyAc+6syYQY4h74SgZc2Ee21um/Y6p5V4XMALkchsDiNHNHabJQSl5QlwLD0NWVq6GzDmADAaO4XjmzikwVgCkUvmzb4sRM+jAT09eAUcIN0n6fsACUrpFtd23d1199D/u1Oa2fLqvy3V61GlflHZ7T+xk9tJn+goR4LZ3MYitVtXgWdVV+C4mAPF+j/ClICAq4xW4PkjdvBIVGwqkovcC5wbW4IJwvcAtF1Q/p+O07JUYDvu7URKDBQCBZod6F3rmWqRdr6Wfrnm6cFhWdZUXobQIxjFyODyDIz2Fc7/3oGHWpAyXtz78h5gIblZ0foekdXFWKgwd0z36E6/PvYQxFPKhjILv3UiHKb5AneVRp2Z4/H5HZcf5Quy1/7YjZOSTrw1FUhOrR/5r/sl+xSNxtE3GHh0uALjRYKCdbSigK1HypBnkVLjaQkZGHrTB9gfQEOMl23t64u9yu/E5d1eEcw3ue3a6a/M/C39PRmzStvOhyCIqpyll9WS43lDYTtb0JvRdCU2JXJnjfLtghdLLrGvrdW4HS5ZhorBnupa9UhDzcQX5oklvRhQxPztX5kKv7KsqQ7EWIU/Ki1ydLPJ28qwG1FjoIbAHCv+ldngz0pULhH+ZKydPMKTy/n/jMIVT7ntGelQM0p/Fn04npdjlBACEHT7pLOpCRXhJXjWEJv7bz1pE+AwRcfVwTlSskxEKrbTHGIwR8chPjwC6/oL7JbWcoDVEKEgjFdM4nzxebcd3tqzVHGkG2P/xqwTBYCfgM5mUZ5sXrUjIY0CgLb3FsalTLLl4OgXrZfcgylqEp/MEBD+lvh+2F08y20Zl1y2f9xtbeJ1K7e1d5Q/npUq1xnc/jXo7T1mwKxnbUO9q1MID5epg8iRHBnVMmpvt7TCOznSg5aTRxyIsTemrE5qsM5SDhCzZ5gBbkWd/r9VMFGz1fB06WdkJG8BzKNYcih9vbGe77BUiSAS5n3c9ajNp0KBJBI2JVKUvVz2w0deqcS9fRHlsWxm6TVQ/f0CO3ga5nEcDbCzI92CGdag7SXt5nAxwU2VR3crrrcbcv7pnOkWKzThKgFZZSl0OR0cMnlwLIjt5rbTZKjw5n+4vJ+tbRlH9ysQwvD3FFAdOXMYLN/3DeKZ8iPyziFn3w0H+k8WBlBPBRATe9S8k5n4dgpD6Nd1hSvmuIsP+HvKqtamvbElTeL/4li+A7Deb3vSHVWXriUw7SqzQANXQfzCxYImzrY/4Hy3jYUhEQKF2fXQvZTnVckVO1XoQ4F+AHhp/wVPrsRjhiYyEG044nNd0Ybz4xQo3EbsMlSbtGpOBlS2pOTXjqKAMNKhTdoTHgU/AexzLUnYdi+yTcluuRVPOmc5xTXDZORs/WRQ38GxZagPdamAHzyhLIiVVeJO/UhqCj5pAXptrG4DAQK0pebIKkIEqyJYzHZM9dqlW8PH6JIiVR7PRODZFFoV9yLFGj6ZzN+Rb0/3qkk2gCqItSn7faDl45Z5JpnG9C9495uIklzpGPCE8/Wf6XyyTcVQBToHpTi0OfIVoOTOsOo6yCx3DO7L3W0pu9rm/tAJDwVCe9JZzRqtoxmeYXWsmMYMJqczjJUnHCd+EHTkXh/+qUSpamliuW60RbtiPt2YmBtZ72kFCslikmfxhWgUQtj54XWjInHynlRO86BqTkIXoswzqX2r4wz46tdiQaWDbJsc3DcgpwAlB9C0Nn29gvg/DpXr1yOrbxoEQ6PlDJd1MpB1A7j7tGh6LRmjc9Nq1XXSPTOz55BsLTTG+FikGKDNeI/LlzmCEVqDCUWZQRXiZbcuHaY1nZWIYEu91gsmVPTU2Btd3o2fpOtlROK9fLfDq/Xuewgjq6HgyXS+LQv1f8dMY1OE0dGOz9xT+J6f1+57p/CYTxf87iRdEsyfeBq2D786P8CbGTWR7+d48kpJ60rl/xXbh6O+cenAVHAM6Ac6DKm5SNA7+qlkrLdV0RkgftoBeJ3w8JOgwKptpXdbuswuBDP4dOErpWSOrL0fVgxg/J0i+2raoxlmo4fxU41DYPEJiOvvWHLGKGWKa8ec5DXNH0QTEthq2D09eoML3HLR2ivjd7EsjQrSBCChK5NXefDPKXcbRVarxeSJKJzurpMIkZJOgY0fdxgaOcrlZ0x7uo4Wg9PGfythHsQYsZXUOrLfS1sx+Qtr5ftDuDgUkbNXuMNyRE6i/tS0rhFHWGsSSTBG5rxN9Ghg+v20gJMTVsEXloyK1NA+ZzRGUNJbSJn/WiYcyHCwYmyPAzNDiXMueod4e38B+u5STDKezwodOo13BkHcQA9oDOjdIKHPbKlBNCIaxH38nd8B8Aik5Q+xbQucmA5WPaQNpRgl52ycIC1HxULTf9mBBq6y/E5Gq6N8l1c4lacPGK5cqsuRsz1YER1XBZVb0CRSTzJmUZk6zY05yyItJDitiSl9nkX7p1XMsei09mOAKF5Jx7ta9RTabBRkJiVpAz2EeSfBol9MLnsX1Q2uJGHtNveHE0Kiocv38lMVKMect4lY2R6kYlevVshpSXt8IyKqShOPrNbzqLcjXNS1/7dQ5ULXnATmLYOUzz1p2wf8ZtmpJj1Qs27/H56rlhUv9BOWBUH8JZbBQK2teNDIQDL0H/gViL1KzwVeErDi0x7Giv4xMghXtAPNvZ9U9XPDipg7bv9QOrAml2JjEB7f4lpIWcYRrHv8f4LVYNKVs89bqmeoyy4z2oDCk8SzhyQJ3JuKJLux8W/kf44WXGSy+n8F+pBAM07s/wkr7zO0GJTCFpCoC4rLhNsfPRj57BCmjlt73RmjFcro6no9ew0P5NQoZPbIdTYdx8/EVavbapDwJHbqrTek235/bNTUjHV6Zs3uKUh1jH1QbeIoijXsXd1OBR+KHetD3oA8S6ZBafGYr0I9WMpyDHLXphvxBaUAfXdNR66D1Z+juIR/3iDKq/qaiolaKbRqdKpqRS+j9FCJ2osGmJaAv1M6aelsGckfJdHVBivXyBrkHhVoGiS/K7gpcyd+XJfGpXmkt1IcX0mY4Lxf7G4ggXYoUf3Wcc5gJN25TnpfCZKH/T1NUhF9ru9MAXxY4i5SHQgCdRG/OcMkW1CiszQnRV1bTk1zYqyoCfmDl5SzMWcH4DOHlyNI2miAVH5isvg79KaxbVpvPuPmKpifIW95iHUv+qBluctdaY0w5eccUKMnw12dGT2WCjxI4vIJnvXW9HybVeESoVwFX8ovwvyLNWzcb61Lk3D64e9JwSfjYTBZviE62KDCI6b5THHUdmKILVx3nvg3tFiY/4M5DRyqzCkXUmSH6hbGg20FMFQbgiJHBBgZKVh2CKb41lhV+z+7IwT9QS4apRUIAektoYcm4vDT0hOadRut4CizJXW0bynBpcW41GTm1moNrFAHnlVZIc/DD+7/5Lu1F9I6o8D73d5cuQ0F6i18cf0U6IQvV0A664+ycmUEcGuRxGiZxzzT+Ln6xnpL9fYwz1qfsCqSOvebz5+KiObg7YUYDQcqYpwImyD2I+ftElAhNZlV1n9Lwj2lkHatrm239IfC4jugBxGZrzJkvGoqMN1AiD5hiSqOqelG7B0UOC8fER/AjICi5h2OwLVUdWJPmhSdkZeKJWgstRSELNQ53PR0zREA0lTM7KracR+FxNc03OCZ4OROtgyryBvz+ezCGg5WMY6PAzT2+7JZCMlU1X+XHXf4Y/UFammhtaBt3+D7UQ18ZtUH2IPvMi3Fxu3U4lBWv2d/x/xOJX4HUl61BnPW/q11ovbfcMsEJqmJoyFinDJeoR7PebRK4T8Ps9FU1CRza++AGPll3ecP590nIf5y4C3B1GCFVV4j+yDue72hU8cofv7xiK4ez+saID/inD6Il9M8lQ+tKZiQNd7JcIOWLSSVbW7R7tgXcyw+jkFa0buQB1ooKBCP2oKPgl3DzdEBBErk0jzJ0PhiY6fGfE6WH2J68XkZ5dXDFIzveo2kiuBlnTYIgACXOMWk/xYP24YxpHmHAId7pG/kp0dLiTK9ELBt6wBQ9SzvJkSOd13JAVsacqefeuwxzHftb1NH3Nji5XLYOeh7cwND1aqoEsIi8YnAVWhvcEW9Fz8oUEjzwYMN+U4ctYawr2fkvguRO/q7vjl31cDsDf/BFPH7L3I6w81hPAZY17ufz/q+ZpxZ54IHbojI1zR0E6Apti5ZXVM0s9ytCPplKdj5qczhMrPT8XLIMfrcEoN2etJRLN6HBf/Um0QWaxL42jRy4oL4DnwAQE/fZ2TteqEIlL/gMd+uqWzqAQCWKE1b4wAOtK0p5cee+MQJ8aGXOou7J+QEzgCXOjrXRjTd+fLvrrsO5RW+UimUMUFcMC3Axi3EV7bYWIov+6mgFUEEAp0XCZNaxFTZ5R6N7KYCYxY440hXgBAPsU5Pn3BueUBR3yLs5EZJAcXT4NnUPY2FQ42iefRZkdAN7Jm4MYByASlWrDRpvz6pRDveQfgh81k2qPrTKkoCRbDYZFXRKrzvO1n65cFT7Pktpqw3uLJEzxJSGgX24AgLnbfMbHEMicTXw0JFOTLJKhE5NSHlFERbUEXaIghq0g6klCuSCkmv8CovU+3ACewJgTQwiKsGJoI7Hw81XUIyhEX5dnCxymM93A2H4otZH1F0r7eQJtOgnN2/qZ5C14WwpKNmDPM135/nR5TLy3vdNfdElqWL8Mgs/iVPi+2r+bH5dnH6VCZJwMwWA9gHKfKIjlm5Zxhh6lwO8KsjM7ChDrhI3kNFubQ4XIsb1EoWhkumPe0+hX0u2vbzCSqfj242Nipccx6/s1Ysb9pIGStBQCQ7VjxpmPWGV3jt9zxOLEW4+qJzLzHqp8W08Y6py5mswkv5V+zcwvYimMl3CklgwoLGh/VG5fGbrhsTil/MgUsx1XiiNODR79TuZPAsHAsungbL7gDgf779uDzC0FXktgOZHJtIzGlanzgQfibCgr5FHaGEGQIIga/bR52JXTKyiLGBLHb1/kX9hD1qFKvxd17cky+IiHGQMh4eU5z14KKVa1Ts0SbA4Y5ydjX2nj9LXdrxbuxA2XhQQzOaelQu23PkReEAUGeDcF4XDGZULhzVne11TUxEzQO+DLO/DMp6WR4+Z18ZHJCBc6hzfIgqDTLgjcc2TKO+pgOjYK7Iiu54czjMWLmihSl6US8Z57p+P9zypuXU+PUq1ssapxylLteL0DQENMzDvC5ojYYjAK+L3F08vn3Y/8g2C+yWXMhUpI/WuWQUcynagGGdydhYWnJwoyy3mgnRWGXpythUOLgwGcQn1Gtk829w0N+mnl65JBx5JBGp6qLf9bu0mCtPQWAlpD7XeTGfweVlQ0I1wPMrRLJMi0atPV+x5GNLVOx+rxPyikuntUO2MYl0DCmDPuSTU8b/QKQXaMMo4BeUPmqVRDdDWu1rDTNc+9PBx9CJzpQbObPxMx3kIXKOF/MtUx/9L1Ea1ytNoyRAvwzc5jtmoBpbowvEBj3Vg0s0a70bzCseLRgI1q3R2PnocGWFKWAM1VCF+DSu3r3kZV8LsmzsvS2YO5kOcZpcNFaJ1YSuGoTf3Z46ip2ZpuE9fDYbifk7yqbPfG0pRh7Z8iJEDkksZSNauctCtGmi24xR+SNezG/7vodAQgpnI4S7YfmgLGoqxnCYFJFhDOqt15z9J99QG/m22rfNCqOcAoqFiGBGj/yZn//5c449mqlejc/SNcfU+/6fvZleMFDxOLmqmYUHH3y2LqrE8FyqQEDQUVfHaeL2MS7VikowPx5vQx3Fr6qIGZsf9bL1fCyUxoX4z2zfOOp/fR6gyDZHGJuoLMtzVR1+zQHjxN/78+j9m+vQY0/QkqGjEjOzE/RvWEX1UJZHgDGojXC8cPKCBm1KhJyui6hS+iC6vQ5RlbqBVgwtph9UAPKOs59C4TIEaLpl4uerKABA03yLEaUXUjd4uiznc6SBu4fYsBnL70+br4qwkNE3remWFkL210f0nuMlNVO5VpJHpkNdm8gUk9yPIwR38+HHBwyz5Y2QTDcqLp2b9wKK28kMwFmdWtHZzmzih5zcdZhXe3qBTo8b0VzfAcYyu4LFKVf7LNOSZhyQb/dgfK77MsevJheqYCsI419DH/e0sLumioqzKg2SzLKxcejfLYMxcjfhhhZSy0DMT0XAB3gjXUSHjRzfrwh5EQQF/vUwivpFH/PfPUX2I1F5HElOz5s7KVZcgbwMdnramW9ZwvuhARJNaZ0UYhJ8LVyZvDkPF+1iCa16w54fyJMsRdthvfKX43adVCIS8MPpAxnC4ED2CalYfsmWHQ/vjR4h+0Znh+z+vRZvy1DoZnZMI57TqAWob5Gcu6awwcQU+YbENRCWnYl1rztXASwXgi2GM6IHGBrV11d/MIOVoMv0SkY0YRi586/R1hO4FlO9TPhnFcGJgUzlcsOR5MPNIb2ORw5FBm26DERCsLP1TqQTWuNNRzZwFrkMXdRNBdpymU+Tss1N8ZL/LOqSrsC0lA+jrYSQqJrhxcGfdlRxzIBf5OIWgQLGA2nb9Ydqpwsk/FrzW9nBE5fa+PNqTQx07rqsKu3wtq3Y6RIcphqInqkIczIZj1dSxID/+QHm+SQp7xyTzfcyb8/zP4JyOc/jH8TC4KRQ93W5I/Cl+g6v9Sr/bGZwXCS0WGcYKMNMNj58zbbPTtLqitaqQIrfu4bnWvENGeFYQkW7+hWQmj5P0P6K/qGTLdaER48maX4So60ik4qlO7t9agH7aNSebD/lnBzq27+/5S2YMAb/+/Xy4rg4yI4pt2d2IIiSWA7xg+/6sIhZWazYcd+nwudVwMTq7AtoYawaF87ur97Ha3/UgjU/QNN+Of+rlnJstrbzyhT3D8rQGysKVemgvMYF9b75zCIacs8UBMvJQxrSYLFFn3g5Eqb+9wzef9lXlLG+rwlaBEGasJOVVzfniJ222dtGn20mF0/5CpoOJZWgt6vmOhUV7sI/ETr1md44f9rp2Cq16Wr/plHn4FRUV8wbK92jbiOAywX/9mHgG3LyvZ66mVTek3t0cJscFSau1bOEs2UBCxY/agEeNsQEEkOztgmpHfyhrn/hfYx1d5CCDf7GbcKCfAnAyKFMGGwcQb+cgU5sQ6cicfndMtbM/tWaL/Axo/AwD7UzZAvsHEA3M3vHvobmFo3MVX+5AzLLMmKlsIgQAnUAMxoTH6mNCD7J+kUuOw2tyzgsH13goJbJ38RAO6ePAOUXIEiaQaC+NBg/53VSGJJ6ieZPec0ccYgwC667f48qLteDm15tvJ6xtqHM88gLsFmUWkCdCgc/NuXls3dqxJVj+AhSmhE9zFrWUJTnTBo2UciQUBbjNvjQBqlBRbE8zNWccgA7AXHfDBzIqKMlzFd81ZLT4RCnmtBewaTYk74xQxAQA6DnwVyT1BK6kG/87xDgt1WvG2LojAXR9m/RLsvn3TDBfUIgcW3O+1Tb1NEAXPjAmGKQQe+uQhtFwZJ95SB3neaxSY11+mL+OryDIIjmC4ZBEnZnHeGMs7gTSX44xGQOx61ypcczP/hoLtI1ec6Rj0xQIO8TGWDyf80UYe2Od4qYJHkhnEvzBHtNUGh+om6BI9kF2RvAER386W4/kpbYfpNT8y7XHwZC8RC18nMsiPA/S3wtJyyZ9MhwEU4vVzqibIarmlHDN6OZuh/EvU1FGjpWeA/g+fF+q3AMBUP9pt4EfGoRRFCf6BvELY4uohh7+0obUeZUBb8lgOga2UD9lWwby8IdE/XAj7z7sjFcaX4oJxsSCpD58u3+AKYNv83bBvzX30EPY406xEqpju86FsW9COiO4EywxnbFVfTrt57vS78d/rqkgvv+MZfJ5NyWUhfPH/upJnOAxxz9El205f7JXfBafZ2HcVvE+KoekLGUeopP3ZRfyEVd/zW9Zo8MfKter5yth/wFT17uUhrMOYcZorgApS1mBdJtN0CiCVaD3uuNXJLp6NVPj9zFmGTKm6qxYA4U16nMhHsDY/GzlpoflRH42g1Pe8FPWhg6mG+6Bwq+EAC2Ij+OcL2rYXqpYYZVuNr3Yi7K6GBGwpMdCTpxc+DQr3QM469LqW5naYsBdbqBHBBkMQxjCt8iSIUPFtoAffNG976GwAh2Cpv3/oe5KlZrN+Oj0Y/20frxXGHzdaNLyk5fPWC4FpY7Yn5uVZICO+GKJpiELaohGymzvHEMIUceTVdcH/aOuowKKYLjwWBwT9nj61ETa3v57TQwCnncaOCn8uPbsCDRjVqqsZ2CP6tCoYThR+KrqFldVjrzglc12bbhgb8TiijixPnBQy3tPiNEAB8YgG/3CLSc0QkbaCSy+Z2zI4OAy3v7m+NMRgbwicvSP3+KRW0SGYu9SCOImgYupucZTWkD0llbpiCW6tTnvOH11j/0VHqT1MAYorCv+lxz+xtohqUSo9u6+8Lgya4oH0NWQ/4OVx/ftPwCEaDm+q6Eb7xd+A5YGD3v6IMTMzX7/4kMDmdR09LXqfV6QaG+OLfxeB3QP4oK6X1DQIE/hTjEDBj2IvVrecCvIa89/u7Lp/fVmYzCZO1ncx8L0Th6RVwvrJPr/NKjqhPSPapxSQ3mRYXzpZqyZcEglXhsHZv8wPkLGIZQu5VahMgwxsMKPMEFJzrUXToVGsk8FB+F5M/DoOV/ymuqViR729HD2bhptc1QTGFss3TfhSeXcwf+WM2a+wmyKsI/94ySh9Bx3AX7awG3kinDHHWdxuIe0YPVK0zM3WoeLDBccXJpbrjotVkj5+cvkLlDoxddalN0tbir9xZGnpDZzmK+7EQROhwToES6Xy8zlgCiAnsNaLME0yDnqIw3Di5kUq7nEocxGLfw4SIgO73Mg2kax629LOU2vwRt/QLgUtHrcF6d71gWif/hZfK9X7mPlEj/C+zxP94ls/kLQdd0rUjKJPZFTSPyUMTQh/jK8saVtBllFi4M3hIAlt+4wPaoEO+sP2Qb3n9xo+k7Bs/sJVKKraelwBvbvxZTIgVyorWmm3iLOtPdjskD19dQQPRnYLKRbH/G8PJ+08AgCdBXsP+n7h2HWnUDuBtjkQkc67avznGIxvsmDhXDm3ErFInoO/K8dx0r9vqRLY6193v0ogfVt5+hSCvaoSqiIlEKoHvpfGccU4m/F5A2luDrXvJkFHmK0bnMPPeA3SQ7kqjSBSq1Ojd0OHbFFVJJTA+boOBnrBcutJociEVT6wTgzzaQxm0Za5CcY9nQD4K8DIeXc7r6iafAguiOdu37dOG1pSQBUG/yhzdXqY6ZbyELol5zeBsPgUGMkb2roVfj9iuhYBZdkDkKsCvnKfpY64FPZQ96Wq9ML342fmcLC17W+9TGMkjob0BeUxgx0qdoy5IXnW/9gEchM5Vklyi3w8t79Hwv6zX0e/i6lyL7Kn951avlqug+Gx+jr2k/MjQ9zvhMFX+lW4cleULh1YF2jmApYWOxC+W4DfieRdZ7UBFHinqe3FpTs2rD6HLKDSGPohE5B6BHFcDZ+QYqX5qWA7x/f6K4U+Fezn4l8Oh9EAiK3aPh+O34/vI8RYZxtBGrzIyoA5Ze7APp/mU4VdBg4r1oprd0gq1qZxGURA/OhgeIGZob2uEC//a+JgqyUd2q1lNNFHlYigBmL9JXgdNx3GSsX2y/3n+SykGpF0+HcS1dohgcv121PaUlNaWM7hlYu5gAwd626n6zh28DyHqgeceij+ZZWt4cgKDi9KjYjJIm6uMOHVwWkBfBM5oGj47YiiaY0qaIVNEVU5IpNf4x/HA38FXHlHXGTjK61HO//yNobiUAViF7bAnmEHxXP/Ouz3jWFI1FfH+QYrjqcAkDUL4ABV/hF7PVjKpC0c+knWD8mVedlEtvZ8q/Whlv+E/w7x85vljj+Rf58Cq0tAJ8N+ot/ujYl0eVYvFOVRH4pr4zNDCZFHTaAS5mZxtW5H665reMfXFclHtdQtuI899nc+p1hgxmpWLNHy+dm7qzoyRmt3immH4VL+7yDUN5MdNLuHA5XJULjURHaBTF9rvD+AbirN9l+UXzSK3EzOQ1Ch/Ixj09M3jV2wHcTefi6nE/szbgfCo1dQtygJ3ss+yEcWv+21/vTqVqxp3Zf/eXg8RSpXPHui00EpBfGtC380Bv+LBV8RDadlr6dqvRBu8cGghODN1HdWLtTV2Vuti0kDE3YHfxoTbUGUV7+zUDsgSEO1jKsDa+mMl8hZl0H47JUZ6GHlIAFGRRDN/cJvcl+F3f8mhlpLRiubdIlRoj7crzT0MhyKjLwoXJFcv4WhZwuaORo5vPSD1V5x6IIJ8xrmtlNLG4PrbpO0Ag1AEtNs2moprMMYKfR9UGYEcAsJOFrDgnaWK/OnN6N90qO+M00uJaQBMkvpXzsYOcS5BV7bsmXqV5argzRrusj8IFgoxWouM8MB7NXofKIryd0Hvndsjh+uo2BEEGFLVl+5Nm5fhvLbxQBCgCXYFeJLHqVlI6GzCVrwBNqXN4XJryKeQ6aRR7JmOn2fLGIoUKw7chawUY3BT2F7wffNwh2IXbf5tjn6QgwRSjDTKm+yufkXuoL+h4Pnb0slRnm+io2M9Zx2dTnyemBOER6adxRVIetL05UkN2KHcDmqKpgApn1SwwHa39T28vmG3r8OxqZ4I0XvV3kbZzCmVi63WSsgKem4z6rntMFwr1aR3DFsM8O3mb5VmpgbYckN5n+PgPc7wmkGLYkaB7b5IDEDg6zGJHGr9/Zfbzxxro/dbJ/z5+jbrAWWFlm5EMi0c04/xszTIDEOr8u+ZNJOKDfrBa7oOA9oOTrfAP94hx+kQNpxa/bR9+bw3JiBXUcges1NKcCkqdrRolM/PUKnh6/CVneBo2Jggio9MFOIEsf0K5X0BxaTFd+vA5jJ2S47YRi9NGFirUSG1b2FgrYosBF9GZCmxfZf8Z2y7OOWZIiHj5KV1HmjNH0W//O7N7wnR8csMO/Vc5mgOjwc4dLj6r8UJpaxLynMx5joFy6/xzVTEe/aDofYZa+mVRhKmiqGOrZFnJlodkVRYhJ1NYJ6Rzo/BaWhvwXURwDsCfSG0si4oQ4IiknJbHMawwbJYkJRHgjVgLRN5VERdgYiJuiOxSVtoepsFe9qZW0UkxlhoqFDwQfMHmtoazm4qBkXa1pJjZKYuzCxpHZHEAEJAI0Hxv6nDctfaUzPmT/xaSkWfx1qZIRp/OsneGMFIfCsv4JkX1OxCfxdLEgQ4/6rv1QcgpeVIYp97HsMyEdSXW7K3oIR/GFNwN7qxVn5QlwegsvbQJH9A30dbuCi0JQIK86QrzFok0/6njNkdybija+o44FOhaArzJu/AS5r7CSDI2lPHW+yFgIYIoDHgCA6UsOBHRMXtfUU12Ov/s3LbasIhDqJ+Q+vFozPaepINnX4w2RRRDnDv1qyDpiTtGSYCewyCBgETL8xLiDEWoUzaEdzYOmyBsTh1rQW2xi2sxClvdgqYu0rJj5pX5CfL+7ej4n4dh7PuiIK/xvwhrTuLzRbFZ0cixnpQbGBmkB7+ERfeCnnUWXz+lpVMwAvX4PfLtJY0llgsPSDaebuI2t7J0qwFhytntCgkZ6dUbjZwl7f4IbUx54P/z+vXrJQ5yeXuuOqSUZQ+MlqecTYTl+aG6bdJXyo1oklrJZWAI/wM2FYPAGzbTzmFgC4pcFxWAYB4e6yD0T3aTztBNNxtlSEoNSQbtAx4LV8hfWY7WTJPn2hVv4GrM1/chDIIReHD7h+iL8DIv4O5YBX3MTF8b1YFPq+gf/jvFJj+l0PF3ny1ukjIAiBZcTl/TyxKjDFSvZYBDBOAA9UrQ/tja7j9WOPodGUyEAsAHRkWuzGIePe3TFYwsMex8cv11hhNewXyOjiaDxnnpAS/lwrse+HHEU098iWTKEGzth5a16pFh801QaPJLp0Q095yYic9JCGJkQfJrC+mPLsby8jhCbZyUBxNmkGXhyczwHlvEHkYtYfjdEZF9sDCrJ1WDOhUsp0tECGw0vErPjWtfJlhDsowtk0LYN9FyiDuuQNEywO6ewU1zanlcFoLoRUqdZXHaRYvAgjbDU+3OkTPoE+Ops30EBl20uuZqr972dPjp8hJrxvaIH/eJUnPFk2BFa+WvIMIT29ayN+s/zwQaqGRKfIvaYSOAhtvUDSy8KyLQyi4fto/P2xtjeuZXaLGa7JGV5oIJ4OVmLMB+KJpKY0hR2vkcCXj6yldy8B1lwvvQDZMB6/sUxA26OTx3sWNRs1n8vfQwAZiFjOl92mHz7mDn9QgA" alt="Descripción de la imagen">
                
                <h3>RELACION DE LA TEORIA CON LA PERCEPCION Y LA REPRESENTACION</h3>
                <p>
                    Relación de la teoría con la percepción y la representación.
                    La relación entre la teoría, la percepción y la representación es fundamental en la 
                    psicología. 
                    La teoría condiciona la percepción 
                    No percibimos el mundo "en bruto". Lo que vemos, oímos o interpretamos está atravesado 
                    por marcos teóricos previos. El ejemplo clásico es el de la carga teórica de la observación 
                    teoría-ladenness: dos científicos pueden mirar el mismo dato y "ver" cosas distintas porque 
                    sus teorías les dicen qué es relevante. No es que la teoría invente la realidad, sino que 
                    organiza y selecciona lo que percibimos.
                    La percepción alimenta la teoría 
                    En sentido inverso, la teoría no flota en el vacío: se construye, se contrasta y se 
                    corrige a partir de la experiencia perceptiva. La percepción aporta la evidencia empírica 
                    que valida o refuta un modelo. Aquí hay un diálogo circular: la teoría guía qué observar, pero la observación puede derribar la teoría.
                    La representación es el puente
                    La representación es un punto intermedio: la forma en que convertimos la percepción en algo comunicable y pensable, ya sea un concepto, una imagen, un modelo, lenguaje. Toda representación 
                    es ya una interpretación: selecciona, simplifica y organiza lo percibido según una teoría.
                    La teoría estructura como percibimos, la percepción aporta evidencia a la teoría, y la representación media entre ambas al traducir la experiencia en conocimiento.
                </p>
                <img src="https://image.slidesharecdn.com/lapercepcion-210910023533/85/La-percepcion-6-320.jpg" alt="Descripción de la imagen">

                <h3>DEFINICION DE RAZONAMIENTO</h3>
                <p>
                    Definición de razonamiento 
El razonamiento es un proceso mental mediante el cual las personas relacionan ideas, analizan información, 
comparan situaciones y utilizan sus conocimientos para llegar a una conclusión. Es una capacidad fundamental 
del ser humano, ya que permite comprender lo que sucede a nuestro alrededor, resolver problemas, tomar decisiones y explicar diferentes fenómenos de la realidad.Este proceso se relaciona con el pensamiento, la observación, la memoria, la experiencia y el conocimiento. Gracias a estos elementos, las personas pueden interpretar la información que reciben y determinar qué conclusiones pueden obtener a partir de ella. Sin embargo, para razonar correctamente es importante contar con información suficiente, 
analizar los hechos y evitar llegar a conclusiones apresuradas.
                </p>
                <img src="https://www.psicoactiva.com/wp-content/uploads/2023/06/tipos-de-razonamiento.png" alt="Descripción de la imagen">


                <h3>TIPOS DE RAZONAMIENTO</h3>
                <p>
                    Tipos de razonamiento

1\. Razonamiento deductivo: Parte de una idea general para llegar a una conclusión particular.

Ejemplo: Todos los seres humanos necesitan agua. Ana es humana, por lo tanto, necesita agua.

2\. Razonamiento inductivo: Parte de casos particulares para obtener una conclusión general o probable.

Ejemplo: He observado que varios perros ladran; por lo tanto, los perros suelen ladrar.

3\. Razonamiento analógico: Compara situaciones semejantes para encontrar similitudes y proponer posibles soluciones.

Ejemplo: Si estudiar diariamente ayudó a un compañero, también podría ayudarme a mí.

4\. Razonamiento abductivo: Busca la explicación más probable para un hecho observado.

Ejemplo: El suelo está mojado, probablemente llovió.
                </p>
                <img src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgyobz5xtxGqUSwYpSumQ13TmYZcSTN5T0PiPT-L2zBrbDzwclDCUbAMn2VrcF_9-nwWZBMY40PnHgZjAD1PrS9gVDEZG5duCu3h10n93OF9Ld7MwMrNWaM_Krb8pR-qgN5WNZvGke1Te3WJi3KdVQi0uqSA0y-DZB5xjy2R4ZNTVb0fk_add0p40rnya8/w640-h447/ChatGPT%20Image%2021%20abr%202025,%2004_31_54%20p.m..png" alt="Descripción de la imagen">


                <h3>CONSTRUCCION DEL RAZONAMIENTO</h3>
                <P> 
                    El razonamiento es el proceso mediante el cual partimos de información disponible para llegar a conclusiones nuevas. Las dos grandes rutas son la inducción y la deducción, y se distinguen por la dirección del movimiento y por el tipo de garantía que ofrecen sus conclusiones.
Razonamiento deductivo: de lo general a lo particular
Parte de premisas generales (leyes, principios, definiciones) y, mediante reglas lógicas, llega a una conclusión particular que se sigue necesariamente. Si las premisas son verdaderas y la forma es válida, la conclusión no puede ser falsa.
Ejemplo:
Todos los seres humanos son mortales.
Sócrates es un ser humano.
Sócrates es mortal.
La fuerza del razonamiento deductivo reside en su necesidad lógica: la conclusión está ya contenida, de algún modo, en las premisas. No aporta información nueva sobre el mundo, sino que la hace explícita. Su límite es que no puede generar conocimiento empírico nuevo: si las premisas son falsas, la conclusión también lo será aunque el razonamiento sea válido.
Razonamiento inductivo: de lo particular a lo general
Parte de observaciones particulares (casos, ejemplos, datos) y generaliza hacia una conclusión probable sobre una clase más amplia. Aquí la conclusión va más allá de lo que las premisas garantizan, por lo que es probable, no necesaria.
Ejemplo: 
Observación 1: El cuervo que vi hoy es negro.
Observación 2: El cuervo que vi ayer es negro.
Observación 3: Todos los cuervos observados hasta ahora son negros.
Conclusión probable: Todos los cuervos son negros.
La fuerza de la inducción está en que amplía nuestro conocimiento del mundo: permite formular hipótesis, leyes y teorías a partir de la experiencia. Su debilidad es que nunca ofrece certeza absoluta: siempre cabe la posibilidad de un contraejemplo (el famoso "cisne negro" que derriba la generalización).


Truco para recordar:
Deductivo = aplicas una regla que ya conoces → resultado seguro y esperado.
Inductivo = juntas varios casos y sacas una regla → resultado probable y nuevo.


                </P>
                <img src="https://www.psiconetwork.com/wp-content/uploads/2024/11/Psicologia-del-razonamiento.jpg" alt="Descripción de la imagen">


                <h3>CONCEPTUALIZACION DEL RAZONAMIENTO INDUCTIVO Y DEL RAZONAMIENTO DEDUCTIVO</h3>
                <P>
Aquí tienes el desarrollo teórico y extenso sobre la conceptualización del razonamiento, unificando su definición, evolución, componentes y tipos en un solo bloque estructurado.
------------------------------
## Conceptualización Profunda del Razonamiento
El razonamiento es la actividad mental y cognitiva de más alto nivel que poseen los seres humanos. Consiste en la capacidad de estructurar ideas, conectar juicios, aplicar principios lógicos y procesar información con el fin de resolver problemas, tomar decisiones, comprender el entorno y generar nuevo conocimiento.
A diferencia de la mera percepción o la memoria, el razonamiento no solo retiene o recibe datos, sino que los transforma mediante reglas de inferencia. Desde la perspectiva psicológica y cognitiva, es el núcleo de la inteligencia; desde la perspectiva filosófica, es el vehículo formal de la verdad y la argumentación.
------------------------------
## Componentes y Mecanismos de la Estructura Racional
Cualquier proceso de razonamiento, independientemente de su tipo, opera bajo un sistema de tres componentes fundamentales:

* Las Premisas: Son las proposiciones, afirmaciones o datos de partida que sirven como base. Se asumen como verdaderas o válidas dentro del contexto del argumento y representan el conocimiento previo.
* El Nexo Lógico (o Inferencia): Es el proceso mental de vinculación. Es la regla o camino que conecta las premisas entre sí para demostrar que una idea lleva inevitablemente (o probablemente) a otra.
* La Conclusión: Es la proposición final que emerge del análisis de las premisas. Representa el nuevo conocimiento, la decisión tomada o la solución al problema planteado.

------------------------------
## Clasificación Detallada de los Tipos de Razonamiento## 1. Razonamiento Deductivo

* Definición: Es el proceso que se mueve de lo general a lo particular. Si las premisas generales son verdaderas y el método de inferencia es formalmente válido, la conclusión es necesariamente verdadera.
* Mecanismo: Se basa en leyes, axiomas o teorías preestablecidas. El ejemplo clásico es el silogismo aristotélico ("Todos los humanos son mortales; Sócrates es humano; por lo tanto, Sócrates es mortal").
* Limitación: No produce conocimiento verdaderamente nuevo; solo hace explícito algo que ya estaba implícito en las premisas.

## 2. Razonamiento Inductivo

* Definición: Es el proceso inverso, que se mueve de lo particular a lo general. Observa patrones, regularidades o casos aislados para proyectar una ley o conclusión general.
* Mecanismo: Funciona por acumulación de evidencia. Si observas que el agua hierve a 100°C hoy, mañana y en diferentes muestras, induces que el agua siempre hierve a esa temperatura bajo las mismas condiciones.
* Limitación: La conclusión es probable, nunca absoluta. Basta con encontrar un solo caso que no cumpla la regla (un "cisne negro") para invalidar la generalización.

## 3. Razonamiento Analógico

* Definición: Es el pensamiento que conecta lo particular con lo particular basándose en la semejanza.
* Mecanismo: Establece que si dos sistemas, objetos o situaciones comparten varias características conocidas, es muy probable que también compartan una característica nueva o desconocida. Se usa constantemente en la vida diaria, el aprendizaje y la jurisprudencia (aplicar sentencias pasadas a casos actuales similares).
* Limitación: Es un método intuitivo y de descubrimiento, pero posee un nivel de certeza bajo porque las similitudes superficiales pueden ocultar diferencias estructurales profundas.

## 4. Razonamiento Hipotético-Deductivo

* Definición: Es el pilar fundamental del método científico. Combina la intuición, la inducción y la deducción en un ciclo continuo.
* Mecanismo: Comienza con la observación de un fenómeno (inducción), propone una hipótesis explicativa provisional, deduce cuáles serían las consecuencias lógicas si esa hipótesis fuera cierta, y finalmente diseña experimentos para contrastar esas deducciones con la realidad.

------------------------------
## Resumen Comparativo de Modelos Racionales

| Dimensión Epistemológica | Razonamiento Deductivo | Razonamiento Inductivo | Razonamiento Analógico | Razonamiento Hipotético-Deductivo |
|---|---|---|---|---|
| Flujo del Pensamiento | General → Particular | Particular → General | Particular → Particular | Ciclo: Observación → Hipótesis → Prueba |
| Grado de Certeza | Absoluta (Lógica pura) | Probable (Estadística/Empírica) | Estimativa (Intuitiva) | Verificable (Científica) |
| Función Principal | Validar y demostrar | Descubrir y generalizar | Comparar y transferir | Explicar fenómenos del mundo |
| Origen del Criterio | Leyes, axiomas y reglas | Evidencia empírica repetida | Similitudes y patrones | Teorías puestas a prueba |

Ahora que tenemos todo el panorama completo y extendido, ¿te gustaría aplicar esta estructura para analizar un ejemplo o caso de estudio específico, o prefieres explorar cómo la inteligencia artificial imita estos procesos humanos?


                </P>
                <img src="https://cdn-v1.udocz-assets.com/uploads/book/cover/302830/302830.jpg" alt="Descripción de la imagen">

                
                <h3>DIFERENCIAS EN LOS TERMINOS Y CARACTERISTICAS DEL RAZONAMINETO INDUCTIVO Y DEDUCTIVO</h3>
                <P>
El razonamiento inductivo y el razonamiento deductivo son dos formas fundamentales de pensamiento utilizadas dentro del método científico para la construcción del conocimiento. Aunque tradicionalmente se afirma que el razonamiento inductivo va de lo particular a lo general y el deductivo de lo general a lo particular, esta explicación resulta limitada, ya que ambos pueden presentarse en diferentes combinaciones. Lo que realmente los distingue es la relación que existe entre las premisas y la conclusión. 

Razonamiento inductivo
El razonamiento inductivo se caracteriza por partir de observaciones, experiencias o casos conocidos para formular una conclusión más amplia. En este tipo de razonamiento, las premisas aportan evidencia que apoya la conclusión, pero no garantizan que sea absolutamente verdadera. Por ello, sus conclusiones son probables y pueden modificarse cuando aparece nueva información. Su principal función es generar hipótesis, explicaciones y generalizaciones que permitan ampliar el conocimiento científico. 

Características principales:
Se basa en la observación de hechos o fenómenos.
Identifica características comunes entre varios casos.
Generaliza esas características hacia otros elementos o situaciones.
Sus conclusiones tienen un carácter probable.
Permite formular hipótesis y teorías científicas.
Favorece el descubrimiento de nuevos conocimientos.

Razonamiento deductivo
El razonamiento deductivo parte de principios, leyes o premisas previamente aceptadas para llegar a una conclusión específica. Su característica principal es que pretende que la conclusión se derive necesariamente de las premisas. Esto significa que, si las premisas son verdaderas y el razonamiento es válido, la conclusión también será verdadera. Por esta razón, el razonamiento deductivo se utiliza para demostrar, comprobar y validar conocimientos dentro de una investigación científica. 

Características principales:
Parte de conocimientos generales o establecidos.
Sigue una estructura lógica y ordenada.
Busca demostrar la validez de una conclusión.
Ofrece un mayor grado de certeza.
Permite comprobar hipótesis y teorías.
Se utiliza para fundamentar argumentos científicos. 

Cuadro Comparativo:
Aspecto	Razonamiento inductivo	Razonamiento deductivo
Punto de partida	Observaciones y casos particulares	Premisas o principios establecidos
Dirección del pensamiento	Amplía el conocimiento hacia nuevas conclusiones	Aplica conocimientos generales a casos concretos
Tipo de conclusión	Probable	Necesaria o lógica
Finalidad	Formular hipótesis y generalizaciones	Comprobar y demostrar conclusiones
Nivel de certeza	Menor certeza	Mayor certeza lógica
Uso en la investigación	Descubrimiento y generación de conocimiento	

Ejemplos
Ejemplo de razonamiento inductivo
Juan es mexicano y amable.
Pedro es mexicano y amable.
Pablo es mexicano y amable.
Conclusión: Todos los mexicanos son amables. 
Ejemplo de razonamiento deductivo
Todos los felinos son mamíferos.
Silvestre es un felino.
Conclusión: Silvestre es un mamífero. 

Importancia dentro del método científico
Tanto el razonamiento inductivo como el deductivo son indispensables en la investigación científica. El razonamiento inductivo permite observar la realidad y generar explicaciones o hipótesis, mientras que el razonamiento deductivo ayuda a comprobarlas y validarlas mediante procedimientos lógicos. La combinación de ambos contribuye a la construcción de conocimientos confiables, objetivos y fundamentados científicamente. 

                </P>
                <img src="https://expertouniversitario.es/wp-content/uploads/2023/01/inductiva-o-deductiva.png" alt="Descripción de la imagen">


                <h3>CONCEPTUALIZACION DE ANALISIS Y SINTESIS</h3>
                <P>
El análisis y la síntesis son los dos procesos cognoscitivos fundamentales e interdependientes que utiliza el ser humano para descifrar la complejidad de la realidad, estructurar el conocimiento científico y construir teorías sólidas. No actúan de forma aislada, sino como un circuito dinámico donde uno necesita del otro para alcanzar una comprensión verdadera.
El Proceso de Análisis: Descomposición y Examen
El análisis es el proceso mental que consiste en descomponer de forma intencional un objeto de estudio, fenómeno o sistema en cada una de sus partes constitutivas para examinarlas de manera aislada.
Función en el pensamiento: Permite aislar variables, identificar componentes básicos y entender los mecanismos internos que hacen funcionar a un todo.
En el conocimiento científico: Se asocia con las formas lógicas del pensamiento. Es la herramienta que ayuda a delimitar los conceptos, desglosar juicios particulares, examinar ideas de manera rigurosa y clasificar los datos empíricos obtenidos en la fase de observación 
El Proceso de Síntesis: Integración y Totalidad
La síntesis es el proceso inverso y complementario que consiste en integrar, unificar y entrelazar los componentes o datos previamente dispersos de un objeto para estudiarlos en su totalidad.
Función en el pensamiento: No es una simple acumulación de partes, sino la reconstrucción lógica de un fenómeno que permite descubrir las conexiones internas y el sentido global del objeto.
En el conocimiento científico: Representa el paso hacia las funciones avanzadas del pensamiento [Es el momento donde la tesis (lo planteado) y la antítesis (lo cuestionado o contrastado) se fusionan para conformar leyes, hipótesis validadas y teorías científicas maduras
2. Objetivo y Finalidad de la Argumentación en una Investigación
La argumentación en el diseño de una investigación es el eje racional que sostiene todo el proyecto. Su finalidad última no es simplemente exponer datos, sino demostrar con rigor científico, lógico y metodológico la validez, viabilidad y relevancia de un estudio frente a una comunidad académica o social.


A continuación, se detallan sus objetivos principales estructurados para su desarrollo web:
Justificar la Relevancia del Problema (El "Por Qué")
La argumentación es el espacio obligatorio para ofrecer una defensa convincente sobre la selección de un tema. Su objetivo es dotar de objetividad a un paso que inicialmente puede nacer de una inquietud subjetiva o un "capricho intelectual". Una buena argumentación demuestra que el problema detectado tiene un arraigo real en la sociedad (un problema social) o en la disciplina (un vacío de conocimiento).
Demostrar el Aporte Disciplinar (El "Para Qué")
Una investigación no se justifica solo por la gravedad de un problema, sino por lo que el estudio aporta al campo de conocimiento. La argumentación debe delimitar y esclarecer cómo el proyecto logrará:
Ofrecer nuevos discernimientos teóricos.
Actualizar y sistematizar datos disponibles que ya han quedado obsoletos.
Proponer innovaciones técnicas o metodológicas replicables para futuros investigadores.
Sustentar la Validez de las Hipótesis y Conclusiones
En ciencia, una afirmación carece de valor si no está respaldada. El objetivo de la argumentación es construir un puente sólido entre la teoría y la evidencia empírica. A través de juicios verdaderos, antecedentes comprobados y leyes establecidas, el investigador argumenta para demostrar que sus hipótesis no son conjeturas al azar, sino respuestas provisionales con un altísimo grado de probabilidad y verosimilitud.
Garantizar la Coherencia y Articulación del Diseño
Finalmente, la argumentación tiene una finalidad estructural interna: asegurar la congruencia lógica de todo el documento. Debe tejer una línea conductora perfecta donde el título, la pregunta de investigación, los objetivos (generales y específicos) y el marco conceptual se justifiquen y respondan mutuamente de manera transparente, evitando contradicciones y garantizando que el proyecto sea técnicamente viable.

                </P>
                <img src="https://tse2.mm.bing.net/th/id/OIP.lwBdhXaskKMklVkeQrUxNgHaFP?r=0&rs=1&pid=ImgDetMain&o=7&rm=3" alt="Descripción de la imagen">


                <h3>OBJETIVO O FINALIDAD EN LA ARGUMENTACION DE UNA INVESTIGACION</h3>
                <P>
El objetivo primordial y definitivo de la argumentación en una investigación científica o académica consiste en articular un entramado lógico, metodológico y conceptual para justificar la relevancia de un problema, demostrar la validez de una hipótesis y defender una postura crítica ante los pares científicos. Este proceso trasciende la mera recopilación, descripción o exposición lineal de datos aislados; su verdadera esencia radica en transformar la información bruta en conocimiento validado a través de un razonamiento transparente, riguroso y replicable. Para alcanzar esta meta, el investigador debe seleccionar, jerarquizar y conectar de manera estratégica evidencias empíricas sólidas, datos estadísticos verificables, testimonios documentales y marcos teóricos vigentes.
A través de esta articulación sustantiva, la argumentación cumple una triple función dentro del aparato crítico del documento: en primer lugar, opera de manera persuasiva y convectora, buscando que la comunidad científica reconozca la legitimidad, veracidad y rigor metodológico de las conclusiones presentadas; en segundo lugar, ejerce una función dialéctica y refutativa, puesto que implica contrastar de forma directa los hallazgos propios con hipótesis rivales, lagunas cognitivas o contradicciones en la literatura existente para poder superarlas o matizarlas con base en la nueva evidencia; y en tercer lugar, actúa como un motor de integración epistémica, el cual permite engarzar los resultados particulares obtenidos en el estudio con las teorías universales de la disciplina. En última instancia, la finalidad última de argumentar formalmente es garantizar que los nuevos descubrimientos dejen de ser meras opiniones subjetivas y adquieran el estatus de conocimiento científico confiable, abriendo así el camino para nuevas líneas de discusión, 
aplicaciones prácticas o la reconfiguración de los paradigmas teóricos establecidos.

                </P>
                <img src="https://th.bing.com/th/id/R.eeb4a98a971100a76448fe856315fac7?rik=mkIaDTSMpOAQ7w&pid=ImgRaw&r=0" alt="Descripción de la imagen">


                <h3>UBICACION EN LA METODOLOGIA CIENTIFICA</h3>
                <P>
La metodología de la ciencia se ubica como el núcleo estratégico, normativo y procedimental del conocimiento científico, funcionando como el puente indispensable entre la teoría pura y la práctica empírica. Dentro del árbol general de la ciencia, no es simplemente un listado de pasos mecánicos, sino una disciplina filosófica y operativa que se sitúa jerárquicamente por debajo de la epistemología (la teoría del conocimiento) y por encima de las técnicas de investigación (las herramientas concretas). Mientras que la epistemología se encarga de definir los fundamentos, la validez, el alcance del saber científico y responde a la pregunta de qué es la verdad, la metodología se ocupa del cómo se alcanza, diseña y justifica ese conocimiento de manera sistemática.
A su vez, la metodología coordina el nivel técnico-instrumental, que abarca los métodos particulares, el software de análisis, los experimentos y las encuestas utilizadas para recolectar datos sobre la realidad. Su papel fundamental en la investigación científica consiste en proveer la rigurosidad necesaria para que los descubrimientos sean replicables, verificables y objetivos, organizando el pensamiento humano mediante enfoques estructurados como el deductivo, el inductivo o el hipotético-deductivo. En resumen, la metodología de la ciencia es la encargada de traducir las grandes teorías e interrogantes abstractas de la filosofía en estrategias de diseño metodológico concretas (ya sean cuantitativas, cualitativas o mixtas), garantizando que las conclusiones obtenidas en el laboratorio o en el campo cuenten con validez interna, validez externa y legitimidad dentro de la comunidad científica internacional.


                </P>
                 <img src="https://thumbs.dreamstime.com/b/animaci%C3%B3n-de-icono-color-investigaci%C3%B3n-mercado-objetivo-animado-target-market-research-signo-aislado-sobre-fondo-blanco-207646294.jpg" alt="Descripción de la imagen">



            </section>


            <!-- IMPORTANCIA -->
            <section id="importancia">
                <h2>Importancia</h2>

                <p>
                    La percepción, la representación y la argumentación son
                    importantes porque permiten observar el entorno, organizar
                    información, comprender fenómenos y comunicar ideas con
                    claridad. También ayudan a analizar críticamente la
                    información y a tomar decisiones fundamentadas.
                </p>

                <div class="info">
                    <strong>¿Sabías que?</strong>
                    En una investigación científica, una idea necesita
                    evidencias y argumentos para respaldar las conclusiones.
                </div>
            </section>

            <!-- CONCLUSION -->
            <section id="conclusion">
                <h2>Conclusión</h2>

                <p>
                    La percepción, la representación y la argumentación se
                    complementan en el método científico. Gracias a ellas
                    podemos observar la realidad, organizar lo que conocemos
                    y explicar nuestras ideas con razones y evidencias.
                    Su uso permite construir y comunicar conocimientos
                    de manera más clara y fundamentada.


                    REFERENCIAS: 

                    Dávila Newman, G. (2006). El razonamiento inductivo y deductivo dentro del proceso investigativo en ciencias experimentales y sociales. Laurus, 12(Ext.), 180–205. https://rua2024.unam.mx/portal/recursos/ficha/6345/el-razonamiento-inductivo-y-deductivo-dentro-del-proceso-investigativo-en-ciencias-experimentales-y-sociales

Hernández Sampieri, R., Fernández Collado, C., & Baptista Lucio, P. (2010). Metodología de la investigación (5.ª ed.). McGraw-Hill Interamericana.

Padilla, H. (1989). El pensamiento científico: Área de metodología de la ciencia. Trillas.

Copi, I. M., Cohen, C., y McMahon, K. (2014). Introducción a la lógica (14.ª ed.). Pearson.
Copi, I. M. (2013). Introducción a la lógica. Limusa.
Hernández Sampieri, R., Fernández Collado, C., y Baptista Lucio, M. P. (2014). Metodología de la investigación (6.ª ed.). McGraw-Hill Education.
Aristóteles. (1982). Tratados de lógica (Órganon). Gredos.
                </p>
            </section>

        </main>
    </div>

    <footer>
        <p>© 2026 Mi Wiki | Elaborado por: Equipo de la Actividad 18</p>
    </footer>

</body>
</html>
