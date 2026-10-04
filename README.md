<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Utilidades Curiúva: casa, roupas, acessórios, perfumes, maquiagens, garrafas Stanley, impressões, Xerox, mochilas e bolsas.">
    <meta name="theme-color" content="#7d1738">
    <title>Utilidades Curiúva | Miah Oliver Studio</title>
    <style>
        :root {
            color-scheme: light;
            --wine: #7d1738;
            --wine-dark: #581027;
            --rose: #fff5f8;
            --gold: #d9ad68;
            --ink: #351523;
            --muted: #735e67;
            --white: #fff;
            --shadow: 0 12px 32px rgba(75, 20, 42, .12);
        }

        * {
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
            scroll-padding-top: 90px;
        }

        body {
            margin: 0;
            background: var(--rose);
            color: var(--ink);
            font-family: Arial, Helvetica, sans-serif;
            line-height: 1.6;
        }

        a {
            color: inherit;
        }

        .site-header {
            padding: 22px 20px;
            background: linear-gradient(125deg, var(--wine-dark), var(--wine));
            color: var(--white);
            text-align: center;
        }

        .site-header h1 {
            margin: 0;
            font-size: clamp(1.6rem, 4vw, 2.35rem);
            letter-spacing: .07em;
        }

        .site-header p {
            margin: 3px 0 0;
            color: #f2d7df;
        }

        .site-nav {
            position: sticky;
            top: 0;
            z-index: 10;
            display: flex;
            justify-content: center;
            gap: 6px;
            overflow-x: auto;
            padding: 10px 16px;
            background: var(--white);
            box-shadow: 0 3px 14px rgba(53, 21, 35, .1);
            scrollbar-width: thin;
        }

        .site-nav a {
            flex: 0 0 auto;
            padding: 8px 12px;
            border-radius: 999px;
            color: var(--wine);
            font-size: .92rem;
            font-weight: 700;
            text-decoration: none;
        }

        .site-nav a:hover,
        .site-nav a:focus-visible {
            background: var(--rose);
            outline: none;
        }

        .hero {
            display: grid;
            grid-template-columns: minmax(0, 1fr) minmax(280px, .95fr);
            align-items: center;
            gap: clamp(24px, 5vw, 64px);
            max-width: 1120px;
            margin: 0 auto;
            padding: clamp(36px, 7vw, 76px) 24px;
        }

        .hero-copy .eyebrow {
            margin: 0 0 8px;
            color: var(--wine);
            font-size: .8rem;
            font-weight: 700;
            letter-spacing: .16em;
            text-transform: uppercase;
        }

        .hero h2 {
            margin: 0 0 14px;
            color: var(--wine-dark);
            font-size: clamp(2rem, 5vw, 3.2rem);
            line-height: 1.12;
        }

        .hero-copy > p:not(.eyebrow) {
            max-width: 520px;
            margin: 0;
            color: var(--muted);
            font-size: 1.08rem;
        }

        .hero-actions {
            display: flex;
            flex-wrap: wrap;
            gap: 12px;
            margin-top: 24px;
        }

        .hero-link {
            display: inline-block;
            padding: 12px 20px;
            border-radius: 999px;
            background: var(--wine);
            color: var(--white);
            font-weight: 700;
            text-decoration: none;
            transition: background .2s ease, transform .2s ease;
        }

        .hero-link:hover,
        .whatsapp-link:hover {
            transform: translateY(-2px);
            background: var(--wine-dark);
        }

        .whatsapp-link {
            display: inline-block;
            padding: 12px 20px;
            border-radius: 999px;
            background: #168c4a;
            color: var(--white);
            font-weight: 700;
            text-decoration: none;
            transition: background .2s ease, transform .2s ease;
        }

        .hero-image {
            display: block;
            width: 100%;
            height: auto;
            border: 5px solid var(--white);
            border-radius: 18px;
            box-shadow: var(--shadow);
        }

        .categories {
            padding: 56px 24px 68px;
            background: var(--white);
        }

        .section-heading {
            max-width: 680px;
            margin: 0 auto 30px;
            text-align: center;
        }

        .section-heading h2 {
            margin: 0 0 8px;
            color: var(--wine-dark);
            font-size: clamp(1.7rem, 4vw, 2.3rem);
        }

        .section-heading p {
            margin: 0;
            color: var(--muted);
        }

        .category-grid {
            display: grid;
            grid-template-columns: repeat(3, minmax(0, 1fr));
            gap: 16px;
            max-width: 1050px;
            margin: 0 auto;
        }

        .category-card {
            min-height: 145px;
            padding: 22px;
            border: 1px solid #f0dce3;
            border-radius: 14px;
            background: #fffafb;
            scroll-margin-top: 90px;
            transition: transform .2s ease, box-shadow .2s ease;
        }

        .category-card:hover {
            transform: translateY(-3px);
            box-shadow: var(--shadow);
        }

        .category-card h3 {
            margin: 0 0 7px;
            color: var(--wine);
            font-size: 1.12rem;
        }

        .category-card p {
            margin: 0;
            color: var(--muted);
            font-size: .95rem;
        }

        .site-footer {
            padding: 26px 20px;
            background: var(--wine-dark);
            color: var(--white);
            text-align: center;
        }

        .site-footer p {
            margin: 4px 0;
        }

        .site-footer .tagline {
            color: #f2d7df;
            font-size: .92rem;
        }

        @media (max-width: 760px) {
            .hero {
                grid-template-columns: 1fr;
                gap: 28px;
            }

            .hero-image {
                max-width: 560px;
                margin: 0 auto;
            }

            .category-grid {
                grid-template-columns: repeat(2, minmax(0, 1fr));
            }
        }

        @media (max-width: 480px) {
            .site-header {
                padding: 18px 14px;
            }

            .site-nav {
                justify-content: flex-start;
            }

            .hero,
            .categories {
                padding-right: 16px;
                padding-left: 16px;
            }

            .category-grid {
                grid-template-columns: 1fr;
            }

            .category-card {
                min-height: auto;
            }
        }

        @media (prefers-reduced-motion: reduce) {
            *,
            *::before,
            *::after {
                scroll-behavior: auto !important;
                transition-duration: .01ms !important;
            }
        }
    </style>
</head>
<body>
    <header class="site-header" id="inicio">
        <h1>UTILIDADES CURIÚVA</h1>
        <p>Miah Oliver Studio</p>
    </header>

    <nav class="site-nav" aria-label="Menu principal">
        <a href="#inicio">Início</a>
        <a href="#casa">Casa</a>
        <a href="#roupas">Roupas</a>
        <a href="#acessorios">Acessórios</a>
        <a href="#perfumes">Perfumes</a>
        <a href="#maquiagens">Maquiagens</a>
        <a href="#stanley">Stanley</a>
        <a href="#xerox">Xerox</a>
        <a href="#mochilas">Mochilas</a>
        <a href="#bolsas">Bolsas</a>
    </nav>

    <main>
        <section class="hero" aria-labelledby="hero-title">
            <div class="hero-copy">
                <p class="eyebrow">Miah Oliver Studio</p>
                <h2 id="hero-title">Utilidades para o seu dia a dia</h2>
                <p>Encontre produtos para casa, presentes, acessórios e muito mais. Qualidade, variedade e atendimento feito com carinho.</p>
                <div class="hero-actions">
                    <a class="hero-link" href="#categorias">Conheça nossas categorias</a>
                    <a class="whatsapp-link" href="https://wa.me/5541988704110?text=Ol%C3%A1%2C%20quero%20saber%20mais%20sobre%20os%20produtos." target="_blank" rel="noopener noreferrer" aria-label="Fale com a Utilidades Curiúva pelo WhatsApp">Fale pelo WhatsApp</a>
                </div>
            </div>
            <img class="hero-image" src="FOTO.jpg" alt="Divulgação da loja Utilidades Curiúva e seus produtos e serviços">
        </section>

        <section class="categories" id="categorias" aria-labelledby="categories-title">
            <div class="section-heading">
                <h2 id="categories-title">O que você encontra</h2>
                <p>Uma seleção de produtos e serviços para facilitar sua rotina e deixar seus momentos especiais.</p>
            </div>
            <div class="category-grid">
                <article class="category-card" id="casa">
                    <h3>Casa</h3>
                    <p>Utensílios e itens úteis para o seu lar.</p>
                </article>
                <article class="category-card" id="roupas">
                    <h3>Roupas</h3>
                    <p>Peças para compor seu estilo.</p>
                </article>
                <article class="category-card" id="acessorios">
                    <h3>Acessórios</h3>
                    <p>Detalhes e presentes para todas as ocasiões.</p>
                </article>
                <article class="category-card" id="perfumes">
                    <h3>Perfumes</h3>
                    <p>Fragrâncias para você e para presentear.</p>
                </article>
                <article class="category-card" id="maquiagens">
                    <h3>Maquiagens</h3>
                    <p>Opções para realçar sua beleza.</p>
                </article>
                <article class="category-card" id="stanley">
                    <h3>Garrafas Stanley</h3>
                    <p>Garrafas e acessórios para acompanhar sua rotina.</p>
                </article>
                <article class="category-card" id="xerox">
                    <h3>Impressões e Xerox</h3>
                    <p>Serviços de impressão e cópias digitais.</p>
                </article>
                <article class="category-card" id="mochilas">
                    <h3>Mochilas</h3>
                    <p>Praticidade para trabalho, estudo e passeios.</p>
                </article>
                <article class="category-card" id="bolsas">
                    <h3>Bolsas</h3>
                    <p>Modelos para levar seus itens com estilo.</p>
                </article>
            </div>
        </section>
    </main>

    <footer class="site-footer">
        <p><strong>Utilidades Curiúva | Miah Oliver Studio</strong></p>
        <p class="tagline">Melhor atendimento, melhor qualidade e melhor preço da cidade.</p>
    </footer>
</body>
</html>
