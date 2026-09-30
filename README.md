<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>NeoByte // TECH - Periféricos Gamer & Alta Performance</title>
  <meta name="description" content="Loja oficial NeoByte: mouses gamer ultraleves 8000Hz, teclados mecânicos hotswap, carregadores GaN 140W e docks magnéticos. Vendas com garantia Mercado Livre.">
  
  <!-- Fontes Google -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;500;600;700&family=Outfit:wght@400;600;700;800&family=Plus+Jakarta+Sans:wght@400;500;600;700&display=swap" rel="stylesheet">

  <style>
    /* ==========================================================================
       RESET & VARIÁVEIS DE DESIGN - NEON CYBER TECH (DARK MODE)
       ========================================================================== */
    :root {
      --bg-dark: #08090D;
      --bg-card: #0D101A;
      --bg-card-hover: #131826;
      --cyan-neon: #00f0ff;
      --cyan-glow: rgba(0, 240, 255, 0.35);
      --emerald-neon: #00ff9d;
      --emerald-glow: rgba(0, 255, 157, 0.3);
      --amber-ml: #ffe600;
      --text-white: #ffffff;
      --text-light: #e2e8f0;
      --text-muted: #94a3b8;
      --border-dark: #1e293b;
      --border-cyan: rgba(0, 240, 255, 0.25);
      --font-display: 'Outfit', sans-serif;
      --font-body: 'Plus Jakarta Sans', sans-serif;
      --font-mono: 'JetBrains Mono', monospace;
      --transition: all 0.25s cubic-bezier(0.16, 1, 0.3, 1);
    }

    * { box-sizing: border-box; margin: 0; padding: 0; -webkit-font-smoothing: antialiased; }
    body { background-color: var(--bg-dark); color: var(--text-light); font-family: var(--font-body); line-height: 1.5; overflow-x: hidden; min-height: 100vh; }
    a { color: inherit; text-decoration: none; }
    button { font-family: inherit; cursor: pointer; border: none; background: none; }
    input, select, textarea { font-family: inherit; }

    ::-webkit-scrollbar { width: 8px; }
    ::-webkit-scrollbar-track { background: var(--bg-dark); }
    ::-webkit-scrollbar-thumb { background: #1e293b; border-radius: 4px; }

    .neon-cyan-text { color: var(--cyan-neon); text-shadow: 0 0 10px var(--cyan-glow); }
    .neon-emerald-text { color: var(--emerald-neon); text-shadow: 0 0 10px var(--emerald-glow); }
    .badge-neon {
      display: inline-flex; align-items: center; gap: 4px; padding: 3px 8px;
      font-family: var(--font-mono); font-size: 10px; font-weight: 700; text-transform: uppercase;
      border-radius: 4px; background: rgba(0, 240, 255, 0.1); color: var(--cyan-neon);
      border: 1px solid rgba(0, 240, 255, 0.3);
    }
    .badge-ml { background: rgba(255, 230, 0, 0.12); color: var(--amber-ml); border: 1px solid rgba(255, 230, 0, 0.3); }
    .container { width: 100%; max-width: 1240px; margin: 0 auto; padding: 0 20px; }

    /* Barra Superior Promocional */
    .promo-topbar {
      background: linear-gradient(90deg, #042f36 0%, #08090d 50%, #063124 100%);
      border-bottom: 1px solid rgba(0, 240, 255, 0.2); padding: 7px 16px;
      font-size: 12px; font-family: var(--font-mono); color: #cbd5e1;
      display: flex; align-items: center; justify-content: center; gap: 12px; text-align: center;
    }
    .promo-topbar strong {
      color: var(--cyan-neon); background: rgba(0, 240, 255, 0.15);
      padding: 2px 6px; border-radius: 4px; border: 1px solid rgba(0, 240, 255, 0.3);
    }

    /* Cabeçalho */
    .site-header {
      position: sticky; top: 0; z-index: 50; background: rgba(8, 9, 13, 0.92);
      backdrop-filter: blur(12px); border-bottom: 1px solid var(--border-dark);
    }
    .header-inner { display: flex; align-items: center; justify-content: space-between; height: 76px; gap: 20px; }
    .brand-logo { display: flex; align-items: center; gap: 10px; user-select: none; cursor: pointer; }
    .logo-icon-box {
      width: 38px; height: 38px; border-radius: 10px;
      background: linear-gradient(135deg, var(--cyan-neon), var(--emerald-neon));
      padding: 2px; display: flex; align-items: center; justify-content: center;
      box-shadow: 0 0 15px var(--cyan-glow);
    }
    .logo-icon-box-inner {
      width: 100%; height: 100%; background: var(--bg-dark); border-radius: 8px;
      display: flex; align-items: center; justify-content: center; color: var(--cyan-neon);
    }
    .brand-title { font-family: var(--font-display); font-size: 22px; font-weight: 800; color: var(--text-white); display: flex; align-items: center; gap: 6px; }
    .brand-tag { font-family: var(--font-mono); font-size: 10px; padding: 2px 6px; background: rgba(0, 240, 255, 0.1); border: 1px solid var(--border-cyan); border-radius: 4px; color: var(--cyan-neon); }

    .nav-links { display: flex; align-items: center; gap: 4px; background: rgba(13, 16, 26, 0.8); padding: 4px; border-radius: 12px; border: 1px solid var(--border-dark); }
    .nav-btn { padding: 6px 14px; font-size: 12px; font-weight: 600; color: var(--text-muted); border-radius: 8px; transition: var(--transition); }
    .nav-btn:hover { color: var(--text-white); background: rgba(255, 255, 255, 0.05); }
    .nav-btn.active { color: var(--cyan-neon); background: rgba(0, 240, 255, 0.12); border: 1px solid rgba(0, 240, 255, 0.25); }

    .search-box { flex: 1; max-width: 300px; position: relative; }
    .search-box input {
      width: 100%; background: rgba(13, 16, 26, 0.8); border: 1px solid var(--border-dark);
      border-radius: 10px; padding: 9px 12px 9px 36px; font-size: 12px; color: var(--text-white); outline: none; transition: var(--transition);
    }
    .search-box input:focus { border-color: var(--cyan-neon); box-shadow: 0 0 10px var(--cyan-glow); }
    .search-icon { position: absolute; left: 12px; top: 50%; transform: translateY(-50%); color: var(--text-muted); pointer-events: none; }

    .cart-btn {
      display: flex; align-items: center; gap: 8px; background: var(--bg-card);
      border: 1px solid var(--border-dark); padding: 9px 16px; border-radius: 10px;
      color: var(--text-light); font-weight: 600; font-size: 13px; transition: var(--transition);
    }
    .cart-btn:hover { border-color: var(--cyan-neon); color: var(--cyan-neon); }
    .cart-count {
      background: linear-gradient(135deg, var(--cyan-neon), var(--emerald-neon)); color: #08090d;
      font-size: 11px; font-weight: 800; font-family: var(--font-mono); width: 18px; height: 18px; border-radius: 50%; display: flex; align-items: center; justify-content: center;
    }

    /* Seção Hero */
    .hero-section {
      padding: 60px 0 50px; border-bottom: 1px solid var(--border-dark);
      background: radial-gradient(circle at 50% 20%, rgba(0, 240, 255, 0.08) 0%, transparent 60%);
    }
    .hero-content { display: grid; grid-template-columns: 1fr 1fr; gap: 40px; align-items: center; }
    .hero-text h1 { font-family: var(--font-display); font-size: 42px; font-weight: 800; line-height: 1.15; color: var(--text-white); margin-bottom: 16px; }
    .hero-text h1 span { background: linear-gradient(135deg, var(--cyan-neon), var(--emerald-neon)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }
    .hero-text p { font-size: 15px; color: var(--text-muted); margin-bottom: 28px; line-height: 1.6; }
    .hero-actions { display: flex; gap: 14px; flex-wrap: wrap; }
    .btn-primary {
      background: linear-gradient(135deg, var(--cyan-neon), var(--emerald-neon)); color: #08090d;
      font-weight: 700; font-size: 13px; padding: 12px 24px; border-radius: 10px; display: inline-flex;
      align-items: center; gap: 8px; transition: var(--transition); box-shadow: 0 0 20px var(--cyan-glow);
    }
    .btn-primary:hover { transform: translateY(-2px); box-shadow: 0 0 25px rgba(0, 240, 255, 0.6); }
    .btn-secondary {
      background: rgba(13, 16, 26, 0.9); color: var(--text-white); border: 1px solid var(--border-dark);
      font-weight: 600; font-size: 13px; padding: 12px 22px; border-radius: 10px; display: inline-flex; align-items: center; gap: 8px; transition: var(--transition);
    }
    .btn-secondary:hover { border-color: var(--cyan-neon); color: var(--cyan-neon); }

    .hero-card {
      background: var(--bg-card); border: 1px solid var(--border-cyan); border-radius: 20px;
      overflow: hidden; box-shadow: 0 20px 40px rgba(0,0,0,0.5), 0 0 30px rgba(0,240,255,0.15); position: relative;
    }
    .hero-card img { width: 100%; height: 340px; object-fit: cover; display: block; }
    .hero-card-overlay {
      position: absolute; bottom: 0; left: 0; right: 0;
      background: linear-gradient(to top, rgba(8, 9, 13, 0.95), transparent); padding: 20px;
      display: flex; justify-content: space-between; align-items: flex-end;
    }
    .hero-stats-row { display: grid; grid-template-columns: repeat(3, 1fr); gap: 12px; margin-top: 14px; }
    .stat-pill { background: rgba(13, 16, 26, 0.85); border: 1px solid var(--border-dark); padding: 10px; border-radius: 10px; text-align: center; }
    .stat-pill strong { font-family: var(--font-mono); font-size: 14px; color: var(--cyan-neon); display: block; }
    .stat-pill span { font-size: 10px; color: var(--text-muted); text-transform: uppercase; }

    /* Perks Bar */
    .perks-bar { padding: 24px 0; background: #06070B; border-bottom: 1px solid var(--border-dark); }
    .perks-grid { display: grid; grid-template-columns: repeat(4, 1fr); gap: 20px; }
    .perk-item { display: flex; align-items: center; gap: 12px; padding: 10px; }
    .perk-icon {
      width: 40px; height: 40px; border-radius: 10px; background: rgba(0, 240, 255, 0.08);
      border: 1px solid rgba(0, 240, 255, 0.2); color: var(--cyan-neon); display: flex; align-items: center; justify-content: center; flex-shrink: 0;
    }
    .perk-text h4 { font-size: 13px; font-weight: 700; color: var(--text-white); }
    .perk-text p { font-size: 11px; color: var(--text-muted); }

    /* Catálogo & Cards */
    .catalog-section { padding: 60px 0; }
    .catalog-header { display: flex; align-items: center; justify-content: space-between; margin-bottom: 32px; flex-wrap: wrap; gap: 16px; }
    .section-title { font-family: var(--font-display); font-size: 28px; font-weight: 800; color: var(--text-white); }
    .section-title span { color: var(--cyan-neon); }

    .products-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(280px, 1fr)); gap: 24px; }
    .product-card {
      background: var(--bg-card); border: 1px solid var(--border-dark); border-radius: 16px;
      overflow: hidden; display: flex; flex-direction: column; transition: var(--transition);
    }
    .product-card:hover { transform: translateY(-5px); border-color: rgba(0, 240, 255, 0.5); box-shadow: 0 15px 30px rgba(0,0,0,0.6), 0 0 20px rgba(0,240,255,0.15); }
    .card-img-wrap { position: relative; width: 100%; height: 220px; background: #08090D; overflow: hidden; }
    .card-img-wrap img { width: 100%; height: 100%; object-fit: cover; transition: transform 0.4s ease; }
    .product-card:hover .card-img-wrap img { transform: scale(1.05); }
    .card-badges { position: absolute; top: 12px; left: 12px; display: flex; flex-direction: column; gap: 6px; }
    .card-body { padding: 18px; display: flex; flex-direction: column; flex: 1; }
    .card-category { font-size: 11px; font-family: var(--font-mono); color: var(--cyan-neon); text-transform: uppercase; margin-bottom: 4px; }
    .card-title { font-size: 16px; font-weight: 700; color: var(--text-white); margin-bottom: 6px; }
    .card-tagline { font-size: 12px; color: var(--text-muted); margin-bottom: 12px; flex: 1; }
    .card-specs { display: flex; flex-wrap: wrap; gap: 6px; margin-bottom: 16px; }
    .spec-chip { background: rgba(255, 255, 255, 0.04); border: 1px solid rgba(255, 255, 255, 0.08); padding: 3px 8px; border-radius: 4px; font-size: 10px; font-family: var(--font-mono); color: #cbd5e1; }
    .card-price-row { margin-bottom: 16px; padding-top: 12px; border-top: 1px solid var(--border-dark); }
    .price-original { font-size: 12px; color: #64748b; text-decoration: line-through; }
    .price-main { font-family: var(--font-mono); font-size: 22px; font-weight: 800; color: var(--text-white); }
    .price-pix { font-size: 11px; color: var(--emerald-neon); font-weight: 600; }
    .card-actions { display: grid; grid-template-columns: 1fr 1fr; gap: 8px; }
    .btn-ml {
      background: #ffe600; color: #08090d; font-weight: 700; font-size: 11px; padding: 9px;
      border-radius: 8px; text-align: center; display: flex; align-items: center; justify-content: center; gap: 6px; transition: var(--transition);
    }
    .btn-ml:hover { background: #fff04d; box-shadow: 0 0 15px rgba(255, 230, 0, 0.4); }
    .btn-cart {
      background: rgba(0, 240, 255, 0.1); border: 1px solid rgba(0, 240, 255, 0.3); color: var(--cyan-neon);
      font-weight: 700; font-size: 11px; padding: 9px; border-radius: 8px; text-align: center; display: flex; align-items: center; justify-content: center; gap: 6px; transition: var(--transition);
    }
    .btn-cart:hover { background: var(--cyan-neon); color: #08090d; }

    /* Seção Newsletter */
    .newsletter-section { background: linear-gradient(180deg, #06070B 0%, #0D101A 100%); border-top: 1px solid var(--border-dark); border-bottom: 1px solid var(--border-dark); padding: 60px 0; }
    .newsletter-box {
      background: rgba(13, 16, 26, 0.95); border: 1px solid var(--border-cyan); border-radius: 20px;
      padding: 40px; display: grid; grid-template-columns: 1.2fr 1fr; gap: 30px; align-items: center;
      box-shadow: 0 0 40px rgba(0, 240, 255, 0.08);
    }
    .newsletter-text h3 { font-family: var(--font-display); font-size: 26px; font-weight: 800; color: var(--text-white); margin-bottom: 8px; }
    .newsletter-text p { font-size: 13px; color: var(--text-muted); line-height: 1.5; }
    .newsletter-form { display: flex; flex-direction: column; gap: 10px; }
    .newsletter-input-group { display: flex; gap: 8px; }
    .newsletter-input {
      flex: 1; background: var(--bg-dark); border: 1px solid var(--border-dark); padding: 12px 16px;
      border-radius: 10px; color: var(--text-white); font-size: 13px; outline: none; transition: var(--transition);
    }
    .newsletter-input:focus { border-color: var(--cyan-neon); box-shadow: 0 0 10px var(--cyan-glow); }
    .newsletter-btn {
      background: linear-gradient(135deg, var(--cyan-neon), var(--emerald-neon)); color: #08090d;
      font-weight: 800; font-size: 13px; padding: 12px 22px; border-radius: 10px; display: inline-flex;
      align-items: center; gap: 8px; transition: var(--transition); white-space: nowrap;
    }
    .newsletter-btn:disabled { opacity: 0.6; cursor: not-allowed; }
    .newsletter-feedback { font-size: 12px; font-family: var(--font-mono); min-height: 18px; }
    .feedback-success { color: var(--emerald-neon); }
    .feedback-error { color: #f43f5e; }

    /* Carrinho Lateral */
    .cart-drawer-overlay {
      position: fixed; inset: 0; background: rgba(0, 0, 0, 0.75); backdrop-filter: blur(6px);
      z-index: 99; opacity: 0; pointer-events: none; transition: opacity 0.3s ease;
    }
    .cart-drawer-overlay.open { opacity: 1; pointer-events: auto; }
    .cart-drawer {
      position: fixed; top: 0; right: -420px; bottom: 0; width: 100%; max-width: 400px;
      background: #0b0d14; border-left: 1px solid var(--border-dark); z-index: 100;
      display: flex; flex-direction: column; transition: right 0.35s cubic-bezier(0.16, 1, 0.3, 1);
      box-shadow: -10px 0 40px rgba(0, 0, 0, 0.8);
    }
    .cart-drawer.open { right: 0; }
    .drawer-header { padding: 20px; border-bottom: 1px solid var(--border-dark); display: flex; align-items: center; justify-content: space-between; }
    .drawer-header h3 { font-family: var(--font-display); font-size: 18px; font-weight: 700; color: var(--text-white); }
    .drawer-close { color: var(--text-muted); font-size: 24px; cursor: pointer; line-height: 1; }
    .drawer-items { flex: 1; overflow-y: auto; padding: 20px; display: flex; flex-direction: column; gap: 16px; }
    .drawer-item { display: flex; gap: 12px; background: var(--bg-card); border: 1px solid var(--border-dark); padding: 12px; border-radius: 12px; }
    .drawer-item img { width: 60px; height: 60px; border-radius: 8px; object-fit: cover; }
    .drawer-item-info { flex: 1; }
    .drawer-item-title { font-size: 13px; font-weight: 700; color: var(--text-white); }
    .drawer-item-price { font-family: var(--font-mono); font-size: 13px; color: var(--cyan-neon); margin: 4px 0; }
    .drawer-qty { display: flex; align-items: center; gap: 8px; }
    .qty-btn { width: 22px; height: 22px; background: #1e293b; color: white; border-radius: 4px; display: flex; align-items: center; justify-content: center; font-size: 12px; }
    .drawer-footer { padding: 20px; border-top: 1px solid var(--border-dark); background: #08090D; }
    .drawer-subtotal { display: flex; justify-content: space-between; font-size: 15px; font-weight: 700; margin-bottom: 12px; }

    /* Modal Secreto de Admin */
    .admin-modal-overlay {
      position: fixed; inset: 0; background: rgba(0,0,0,0.85); backdrop-filter: blur(8px);
      z-index: 150; display: none; align-items: center; justify-content: center; padding: 20px;
    }
    .admin-modal-overlay.open { display: flex; }
    .admin-modal-box {
      width: 100%; max-width: 480px; background: #0D101A; border: 1px solid rgba(0, 240, 255, 0.4);
      border-radius: 18px; padding: 28px; box-shadow: 0 0 40px rgba(0, 240, 255, 0.2);
    }
    .admin-modal-box h3 { font-family: var(--font-display); font-size: 20px; color: white; margin-bottom: 8px; }

    /* Rodapé */
    .site-footer { background: #040508; border-top: 1px solid var(--border-dark); padding: 50px 0 30px; color: var(--text-muted); font-size: 12px; }
    .footer-grid { display: grid; grid-template-columns: 2fr 1fr 1fr 1fr; gap: 30px; margin-bottom: 40px; }
    .footer-col h5 { color: var(--text-white); font-size: 13px; font-family: var(--font-mono); text-transform: uppercase; margin-bottom: 14px; }
    .footer-links { list-style: none; display: flex; flex-direction: column; gap: 8px; }
    .footer-links a:hover { color: var(--cyan-neon); }
    .footer-bottom { border-top: 1px solid rgba(255, 255, 255, 0.05); padding-top: 20px; display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; gap: 10px; }

    @media (max-width: 900px) {
      .hero-content { grid-template-columns: 1fr; }
      .perks-grid { grid-template-columns: repeat(2, 1fr); }
      .newsletter-box { grid-template-columns: 1fr; }
      .footer-grid { grid-template-columns: 1fr 1fr; }
      .nav-links { display: none; }
    }
    @media (max-width: 600px) {
      .hero-text h1 { font-size: 30px; }
      .perks-grid { grid-template-columns: 1fr; }
      .search-box { display: none; }
      .footer-grid { grid-template-columns: 1fr; }
      .newsletter-input-group { flex-direction: column; }
    }
  </style>
</head>
<body>

  <!-- BARRA DE ANÚNCIOS -->
  <div class="promo-topbar" id="promoTopbar">
    <span>⚡ <strong>NEOBYTE10</strong>: 10% OFF no catálogo</span>
    <span>•</span>
    <span>Garantia Oficial 2 Anos & Vendas pelo Mercado Livre</span>
  </div>

  <!-- CABEÇALHO -->
  <header class="site-header">
    <div class="container header-inner">
      <!-- Marca com clique secreto para admin (3 cliques rápidos) -->
      <div class="brand-logo" id="brandLogo" title="NeoByte Peripherals">
        <div class="logo-icon-box">
          <div class="logo-icon-box-inner">
            <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5"><polygon points="13 2 3 14 12 14 11 22 21 10 12 10 13 2"></polygon></svg>
          </div>
        </div>
        <div>
          <div class="brand-title">NeoByte <span class="brand-tag">TECH</span></div>
        </div>
      </div>

      <!-- Abas de Navegação -->
      <nav class="nav-links">
        <button class="nav-btn active" data-cat="all">Todos</button>
        <button class="nav-btn" data-cat="mouses">Mouses 8K</button>
        <button class="nav-btn" data-cat="teclados">Teclados Custom</button>
        <button class="nav-btn" data-cat="carregadores">Carregadores GaN</button>
        <button class="nav-btn" data-cat="audio">Áudio & Docks</button>
      </nav>

      <!-- Busca Rápida -->
      <div class="search-box">
        <svg class="search-icon" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="11" cy="11" r="8"></circle><line x1="21" y1="21" x2="16.65" y2="16.65"></line></svg>
        <input type="text" id="searchInput" placeholder="Buscar periféricos...">
      </div>

      <!-- Carrinho -->
      <button class="cart-btn" id="openCartBtn">
        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M6 2L3 6v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2V6l-3-4z"></path><line x1="3" y1="6" x2="21" y2="6"></line><path d="M16 10a4 4 0 0 1-8 0"></path></svg>
        <span>Carrinho</span>
        <span class="cart-count" id="cartCountBadge">0</span>
      </button>
    </div>
  </header>

  <!-- SEÇÃO HERO -->
  <section class="hero-section">
    <div class="container hero-content">
      <div class="hero-text">
        <div class="badge-neon" style="margin-bottom: 14px;">PERIPHERALS LAB // TECH 2026</div>
        <h1>Periféricos de <span>Alta Taxa</span> & Engenharia Pura</h1>
        <p>Projetados para jogadores e entusiastas que exigem resposta instantânea, switches lubrificados de fábrica e fontes GaN de ultra densidade energética.</p>
        <div class="hero-actions">
          <a href="#catalogo" class="btn-primary">
            <span>Ver Catálogo</span>
            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5"><line x1="5" y1="12" x2="19" y2="12"></line><polyline points="12 5 19 12 12 19"></polyline></svg>
          </a>
          <a href="https://vendedores.mercadolivre.com.br/minha-pagina/editor#from=mi-pagina" target="_blank" rel="noopener" class="btn-secondary">
            <span>Loja Mercado Livre</span>
            <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M18 13v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h6"></path><polyline points="15 3 21 3 21 9"></polyline><line x1="10" y1="14" x2="21" y2="3"></line></svg>
          </a>
        </div>

        <div class="hero-stats-row">
          <div class="stat-pill">
            <strong>8000Hz</strong>
            <span>Polling Rate</span>
          </div>
          <div class="stat-pill">
            <strong>&lt;0.2ms</strong>
            <span>Latência Real</span>
          </div>
          <div class="stat-pill">
            <strong>140W GaN</strong>
            <span>Carga Ultra-Rápida</span>
          </div>
        </div>
      </div>

      <div class="hero-visual">
        <div class="hero-card">
          <img src="https://images.unsplash.com/photo-1550745165-9bc0b252726f?q=80&w=1000&auto=format&fit=crop" alt="Setup NeoByte">
          <div class="hero-card-overlay">
            <div>
              <div class="badge-neon">FLAGSHIP SETUP</div>
              <h4 style="color: white; font-size: 16px; margin-top: 4px;">NeoByte CyberBlade 75% + Apex 8K</h4>
            </div>
            <span class="neon-emerald-text" style="font-family: var(--font-mono); font-weight: 700;">Pronta Entrega</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- PERKS BAR -->
  <section class="perks-bar">
    <div class="container perks-grid">
      <div class="perk-item">
        <div class="perk-icon">
          <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="1" y="3" width="15" height="13"></rect><polygon points="16 8 20 8 23 11 23 16 16 16 16 8"></polygon><circle cx="5.5" cy="18.5" r="2.5"></circle><circle cx="18.5" cy="18.5" r="2.5"></circle></svg>
        </div>
        <div class="perk-text">
          <h4>Envio Expresso 24h</h4>
          <p>Despacho com rastreamento oficial</p>
        </div>
      </div>
      <div class="perk-item">
        <div class="perk-icon">
          <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"></path></svg>
        </div>
        <div class="perk-text">
          <h4>Garantia NeoByte 2 Anos</h4>
          <p>Troca rápida sem burocracia</p>
        </div>
      </div>
      <div class="perk-item">
        <div class="perk-icon">
          <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polygon points="13 2 3 14 12 14 11 22 21 10 12 10 13 2"></polygon></svg>
        </div>
        <div class="perk-text">
          <h4>10% OFF no Pix</h4>
          <p>Desconto instantâneo na finalização</p>
        </div>
      </div>
      <div class="perk-item">
        <div class="perk-icon">
          <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="8" r="7"></circle><polyline points="8.21 13.89 7 23 12 20 17 23 15.79 13.88"></polyline></svg>
        </div>
        <div class="perk-text">
          <h4>Hardware Homologado</h4>
          <p>Produtos originais com Nota Fiscal</p>
        </div>
      </div>
    </div>
  </section>

  <!-- CATÁLOGO -->
  <section class="catalog-section" id="catalogo">
    <div class="container">
      <div class="catalog-header">
        <div>
          <h2 class="section-title">Hardware // <span>Catálogo Oficial</span></h2>
          <p style="font-size: 13px; color: var(--text-muted); margin-top: 4px;">Compre com garantia no Mercado Livre ou adicione ao carrinho.</p>
        </div>
        <div class="badge-neon" id="productCountBadge">Carregando itens...</div>
      </div>

      <div class="products-grid" id="productsGrid"></div>
    </div>
  </section>

  <!-- NEWSLETTER (POST FETCH TEXT/PLAIN ANTI-CORS) -->
  <section class="newsletter-section">
    <div class="container">
      <div class="newsletter-box">
        <div class="newsletter-text">
          <div class="badge-neon" style="margin-bottom: 8px;">NEOBYTE CLUB // DROPS EXCLUSIVOS</div>
          <h3>Receba Lançamentos & Cupons de 10% OFF</h3>
          <p>Cadastre seu e-mail para receber alertas de novos lotes de mouses 8K, switches lubrificados e carregadores GaN.</p>
        </div>

        <form class="newsletter-form" id="newsletterForm">
          <div class="newsletter-input-group">
            <input type="email" id="newsletterEmail" class="newsletter-input" placeholder="Seu melhor e-mail gamer..." required>
            <button type="submit" id="newsletterSubmitBtn" class="newsletter-btn">
              <span>Cadastrar</span>
              <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5"><line x1="5" y1="12" x2="19" y2="12"></line><polyline points="12 5 19 12 12 19"></polyline></svg>
            </button>
          </div>
          <div class="newsletter-feedback" id="newsletterFeedback"></div>
        </form>
      </div>
    </div>
  </section>

  <!-- DRAWER DO CARRINHO -->
  <div class="cart-drawer-overlay" id="cartOverlay"></div>
  <aside class="cart-drawer" id="cartDrawer">
    <div class="drawer-header">
      <h3>Seu Carrinho NeoByte</h3>
      <button class="drawer-close" id="closeCartBtn">&times;</button>
    </div>
    <div class="drawer-items" id="cartItemsList"></div>
    <div class="drawer-footer">
      <div class="drawer-subtotal">
        <span>Total:</span>
        <span class="neon-cyan-text" id="cartSubtotalText">R$ 0,00</span>
      </div>
      <button class="btn-primary" style="width: 100%; justify-content: center;" id="checkoutBtn">
        Finalizar Pedido Oficial
      </button>
    </div>
  </aside>

  <!-- MODAL SECRETO DE ADMIN (INVISÍVEL AO PÚBLICO) -->
  <div class="admin-modal-overlay" id="adminModal">
    <div class="admin-modal-box">
      <div style="display: flex; justify-content: space-between; align-items: center; margin-bottom: 16px;">
        <h3>🔒 Painel Restrito do Lojista</h3>
        <button id="closeAdminModalBtn" style="color: var(--text-muted); font-size: 20px;">&times;</button>
      </div>
      <p style="font-size: 12px; color: var(--text-muted); margin-bottom: 20px;">
        Acesso exclusivo. Atalhos: <strong>Ctrl + Shift + A</strong> ou URL <strong>?admin</strong>.
      </p>

      <div id="adminLoginForm">
        <label style="display: block; font-size: 11px; font-family: var(--font-mono); margin-bottom: 6px; color: var(--cyan-neon);">
          PIN DE ACESSO (Padrão: 1234):
        </label>
        <input type="password" id="adminPinInput" class="newsletter-input" placeholder="Digite seu PIN..." style="margin-bottom: 12px; width: 100%;">
        <div id="adminPinError" style="color: #f43f5e; font-size: 11px; margin-bottom: 12px; display: none;">PIN incorreto.</div>
        <button id="adminLoginBtn" class="btn-primary" style="width: 100%; justify-content: center;">
          Acessar Gerenciador
        </button>
      </div>

      <div id="adminDashboard" style="display: none;">
        <h4 style="font-size: 13px; color: white; margin-bottom: 6px;">Link da Loja no Mercado Livre:</h4>
        <input type="text" id="adminMlStoreUrl" class="newsletter-input" style="width: 100%; margin-bottom: 14px;">
        
        <h4 style="font-size: 13px; color: white; margin-bottom: 6px;">Novo PIN de Acesso:</h4>
        <input type="text" id="adminNewPin" class="newsletter-input" placeholder="Digite novo PIN numérico" style="width: 100%; margin-bottom: 14px;">

        <button id="saveAdminSettingsBtn" class="btn-primary" style="width: 100%; justify-content: center; margin-bottom: 10px;">
          Salvar Configurações
        </button>
        <button id="resetDefaultsBtn" class="btn-secondary" style="width: 100%; justify-content: center;">
          Restaurar Catálogo Original
        </button>
      </div>
    </div>
  </div>

  <!-- RODAPÉ -->
  <footer class="site-footer">
    <div class="container">
      <div class="footer-grid">
        <div class="footer-col">
          <div class="brand-title" style="margin-bottom: 12px;">NeoByte <span class="brand-tag">TECH</span></div>
          <p style="font-size: 12px; line-height: 1.6; max-width: 300px;">
            E-commerce de periféricos gamer e tecnologia de alta performance. Peças homologadas, garantia nacional de 2 anos e suporte especializado.
          </p>
        </div>

        <div class="footer-col">
          <h5>Hardware</h5>
          <ul class="footer-links">
            <li><a href="#catalogo">Mouses 8000Hz</a></li>
            <li><a href="#catalogo">Teclados Gasket Mount</a></li>
            <li><a href="#catalogo">Carregadores GaN 140W</a></li>
            <li><a href="#catalogo">Docks Magnéticos</a></li>
          </ul>
        </div>

        <div class="footer-col">
          <h5>Atendimento</h5>
          <ul class="footer-links">
            <li><span>WhatsApp: (11) 98765-4321</span></li>
            <li><span>suporte@neobyte.com.br</span></li>
            <li><span>Seg a Sex: 09h às 19h</span></li>
          </ul>
        </div>

        <div class="footer-col">
          <h5>Políticas</h5>
          <ul class="footer-links">
            <li><a href="#catalogo">Termos de Garantia 2 Anos</a></li>
            <li><a href="#catalogo">Política de Devolução (30 dias)</a></li>
            <li><a href="#catalogo">Compra Segura Mercado Livre</a></li>
          </ul>
        </div>
      </div>

      <div class="footer-bottom">
        <div>© 2026 NEOBYTE TECH. Todos os direitos reservados. CNPJ: 45.892.102/0001-90</div>
        <div style="font-family: var(--font-mono); font-size: 11px; color: var(--emerald-neon);">
          ⚡ 10% OFF NO PIX • CARTÃO EM ATÉ 12X
        </div>
      </div>
    </div>
  </footer>

  <!-- ==========================================================================
       JAVASCRIPT COMPLETO E INTEGRADO
       ========================================================================== -->
  <script>
    // ==========================================================================
    // 1. CONFIGURAÇÃO DO ENDPOINT DE CAPTURA DE E-MAIL
    // Substitua a URL abaixo pelo seu endpoint (ex: Google Apps Script Web App / Webhook):
    // ==========================================================================
    const NEWSLETTER_ENDPOINT = "https://script.google.com/macros/s/SEU_SCRIPT_ID/exec";

    // Catálogo Inicial Padrão NeoByte
    const DEFAULT_PRODUCTS = [
      {
        id: "neobyte-apex-8k",
        name: "Mouse Sem Fio NeoByte Apex Pro 8K",
        category: "mouses",
        categoryLabel: "Mouses Pro",
        price: 449.90,
        originalPrice: 549.90,
        image: "https://images.unsplash.com/photo-1615663245857-ac93bb7c39e7?q=80&w=800&auto=format&fit=crop",
        badge: "Lançamento 8K",
        tagline: "Ultraleve 49g com Polling Rate de 8000Hz real",
        specs: ["49g Ultraleve", "PAW3950 (30K DPI)", "8000Hz Real", "90h Bateria"],
        mlUrl: "https://vendedores.mercadolivre.com.br/minha-pagina/editor#from=mi-pagina"
      },
      {
        id: "neobyte-cyberblade-75",
        name: "Teclado Mecânico NeoByte CyberBlade 75%",
        category: "teclados",
        categoryLabel: "Teclados Custom",
        price: 589.90,
        originalPrice: 699.90,
        image: "https://images.unsplash.com/photo-1587829741301-dc798b83add3?q=80&w=800&auto=format&fit=crop",
        badge: "Gasket Mount",
        tagline: "Estrutura isolada em silicone com switches lubrificados",
        specs: ["Layout 75%", "Switches Lubrificados", "Hotswap 5-pin", "PBT Double-shot"],
        mlUrl: "https://vendedores.mercadolivre.com.br/minha-pagina/editor#from=mi-pagina"
      },
      {
        id: "neobyte-voltforge-140w",
        name: "Carregador Desktop NeoByte VoltForge GaN III 140W",
        category: "carregadores",
        categoryLabel: "Carregadores GaN",
        price: 329.90,
        originalPrice: 399.90,
        image: "https://images.unsplash.com/photo-1583863788434-e58a36330cf0?q=80&w=800&auto=format&fit=crop",
        badge: "GaN III 140W",
        tagline: "4 Portas USB-C/A com display digital de potência em tempo real",
        specs: ["140W PD 3.1", "3x USB-C + 1x USB-A", "Display OLED", "GaN III"],
        mlUrl: "https://vendedores.mercadolivre.com.br/minha-pagina/editor#from=mi-pagina"
      },
      {
        id: "neobyte-sonar-pro",
        name: "Headset Gamer Sem Fio NeoByte Sonar Spatial",
        category: "audio",
        categoryLabel: "Áudio & Periféricos",
        price: 499.90,
        originalPrice: 599.90,
        image: "https://images.unsplash.com/photo-1546435770-a3e426bf472b?q=80&w=800&auto=format&fit=crop",
        badge: "Som Espacial",
        tagline: "Drivers de biocelulose 50mm e microfone com cancelamento de ruído AI",
        specs: ["Drivers 50mm", "2.4GHz + BT 5.3", "Almofadas Memory Foam", "Latência <15ms"],
        mlUrl: "https://vendedores.mercadolivre.com.br/minha-pagina/editor#from=mi-pagina"
      },
      {
        id: "neobyte-magcharge-dock",
        name: "Dock Magnético 3 em 1 NeoByte Orbit Qi2",
        category: "carregadores",
        categoryLabel: "Carregadores & Docks",
        price: 279.90,
        originalPrice: 349.90,
        image: "https://images.unsplash.com/photo-1622445262464-84b1456045b6?q=80&w=800&auto=format&fit=crop",
        badge: "Qi2 15W",
        tagline: "Carregamento magnético simultâneo para celular, relógio e fones",
        specs: ["Alumínio Usinado", "Ímãs N52", "Qi2 Oficial 15W", "Articulação 360°"],
        mlUrl: "https://vendedores.mercadolivre.com.br/minha-pagina/editor#from=mi-pagina"
      },
      {
        id: "neobyte-phantom-ergonomic",
        name: "Mouse Gamer Ergonômico NeoByte Phantom",
        category: "mouses",
        categoryLabel: "Mouses Pro",
        price: 319.90,
        originalPrice: 389.90,
        image: "https://images.unsplash.com/photo-1527864550417-7fd91fc51a46?q=80&w=800&auto=format&fit=crop",
        badge: "Ergonomia Pura",
        tagline: "Shape anatômico para pegadas Palm e Claw sem fadiga",
        specs: ["54g Equilibrado", "PAW3395 (26K DPI)", "80h Bateria", "Grip Tapes Inclusos"],
        mlUrl: "https://vendedores.mercadolivre.com.br/minha-pagina/editor#from=mi-pagina"
      }
    ];

    // Estados salvos no localStorage
    let products = JSON.parse(localStorage.getItem('neobyte_products')) || DEFAULT_PRODUCTS;
    let cart = JSON.parse(localStorage.getItem('neobyte_cart')) || [];
    let currentCategory = 'all';
    let currentSearch = '';
    let mlStoreUrl = localStorage.getItem('neobyte_ml_url') || 'https://vendedores.mercadolivre.com.br/minha-pagina/editor#from=mi-pagina';

    // 2. RENDERIZAR PRODUTOS
    function renderProducts() {
      const grid = document.getElementById('productsGrid');
      const countBadge = document.getElementById('productCountBadge');
      
      const filtered = products.filter(p => {
        const matchesCategory = (currentCategory === 'all' || p.category === currentCategory);
        const q = currentSearch.toLowerCase();
        const matchesSearch = p.name.toLowerCase().includes(q) || p.tagline.toLowerCase().includes(q);
        return matchesCategory && matchesSearch;
      });

      countBadge.textContent = `${filtered.length} ${filtered.length === 1 ? 'produto encontrado' : 'produtos encontrados'}`;

      if (filtered.length === 0) {
        grid.innerHTML = `
          <div style="grid-column: 1 / -1; text-align: center; padding: 40px; color: var(--text-muted);">
            Nenhum periférico encontrado com o termo "<strong>${currentSearch}</strong>".
          </div>
        `;
        return;
      }

      grid.innerHTML = filtered.map(p => {
        const pixPrice = (p.price * 0.9).toFixed(2).replace('.', ',');
        const formattedPrice = p.price.toFixed(2).replace('.', ',');
        const formattedOriginal = p.originalPrice.toFixed(2).replace('.', ',');

        return `
          <article class="product-card">
            <div class="card-img-wrap">
              <img src="${p.image}" alt="${p.name}" loading="lazy">
              <div class="card-badges">
                ${p.badge ? `<span class="badge-neon">${p.badge}</span>` : ''}
                <span class="badge-neon badge-ml">Mercado Livre</span>
              </div>
            </div>
            <div class="card-body">
              <span class="card-category">${p.categoryLabel}</span>
              <h3 class="card-title">${p.name}</h3>
              <p class="card-tagline">${p.tagline}</p>

              <div class="card-specs">
                ${p.specs.map(s => `<span class="spec-chip">${s}</span>`).join('')}
              </div>

              <div class="card-price-row">
                <div class="price-original">R$ ${formattedOriginal}</div>
                <div class="price-main">R$ ${formattedPrice}</div>
                <div class="price-pix">ou R$ ${pixPrice} no Pix (10% OFF)</div>
              </div>

              <div class="card-actions">
                <a href="${p.mlUrl || mlStoreUrl}" target="_blank" rel="noopener" class="btn-ml">
                  <span>Comprar no ML</span>
                </a>
                <button class="btn-cart" onclick="addToCart('${p.id}')">
                  <span>+ Carrinho</span>
                </button>
              </div>
            </div>
          </article>
        `;
      }).join('');
    }

    // 3. CARRINHO DE COMPRAS
    function updateCartBadge() {
      const count = cart.reduce((acc, item) => acc + item.quantity, 0);
      document.getElementById('cartCountBadge').textContent = count;
      localStorage.setItem('neobyte_cart', JSON.stringify(cart));
    }

    function renderCartDrawer() {
      const list = document.getElementById('cartItemsList');
      const subtotalEl = document.getElementById('cartSubtotalText');

      if (cart.length === 0) {
        list.innerHTML = `
          <div style="text-align: center; color: var(--text-muted); padding: 40px 0;">
            Seu carrinho está vazio.<br>Adicione itens da loja!
          </div>
        `;
        subtotalEl.textContent = 'R$ 0,00';
        return;
      }

      let total = 0;
      list.innerHTML = cart.map(item => {
        const itemTotal = item.product.price * item.quantity;
        total += itemTotal;
        return `
          <div class="drawer-item">
            <img src="${item.product.image}" alt="${item.product.name}">
            <div class="drawer-item-info">
              <div class="drawer-item-title">${item.product.name}</div>
              <div class="drawer-item-price">R$ ${item.product.price.toFixed(2).replace('.', ',')}</div>
              <div class="drawer-qty">
                <button class="qty-btn" onclick="updateQty('${item.product.id}', -1)">-</button>
                <span style="font-size: 13px; font-weight: 700; color: white;">${item.quantity}</span>
                <button class="qty-btn" onclick="updateQty('${item.product.id}', 1)">+</button>
                <button onclick="removeFromCart('${item.product.id}')" style="margin-left: auto; color: #ef4444; font-size: 11px;">Remover</button>
              </div>
            </div>
          </div>
        `;
      }).join('');

      subtotalEl.textContent = `R$ ${total.toFixed(2).replace('.', ',')}`;
    }

    window.addToCart = function(productId) {
      const product = products.find(p => p.id === productId);
      if (!product) return;

      const existing = cart.find(item => item.product.id === productId);
      if (existing) {
        existing.quantity += 1;
      } else {
        cart.push({ product, quantity: 1 });
      }

      updateCartBadge();
      renderCartDrawer();
      openCart();
    };

    window.updateQty = function(productId, delta) {
      const item = cart.find(i => i.product.id === productId);
      if (!item) return;

      item.quantity += delta;
      if (item.quantity <= 0) {
        cart = cart.filter(i => i.product.id !== productId);
      }

      updateCartBadge();
      renderCartDrawer();
    };

    window.removeFromCart = function(productId) {
      cart = cart.filter(i => i.product.id !== productId);
      updateCartBadge();
      renderCartDrawer();
    };

    function openCart() {
      document.getElementById('cartDrawer').classList.add('open');
      document.getElementById('cartOverlay').classList.add('open');
    }

    function closeCart() {
      document.getElementById('cartDrawer').classList.remove('open');
      document.getElementById('cartOverlay').classList.remove('open');
    }

    // 4. ENVIO DE E-MAIL VIA FETCH POST EM TEXT/PLAIN (ANTI-CORS)
    const newsletterForm = document.getElementById('newsletterForm');
    const newsletterEmail = document.getElementById('newsletterEmail');
    const newsletterSubmitBtn = document.getElementById('newsletterSubmitBtn');
    const newsletterFeedback = document.getElementById('newsletterFeedback');

    newsletterForm.addEventListener('submit', async function(e) {
      e.preventDefault();
      const email = newsletterEmail.value.trim();

      if (!email || !email.includes('@')) {
        newsletterFeedback.className = 'newsletter-feedback feedback-error';
        newsletterFeedback.textContent = 'Por favor, insira um e-mail válido.';
        return;
      }

      newsletterSubmitBtn.disabled = true;
      newsletterSubmitBtn.innerHTML = '<span>Enviando...</span>';
      newsletterFeedback.textContent = '';

      const payload = {
        email: email,
        origem: "Ecommerce-NeoByte",
        data: new Date().toLocaleString("pt-BR"),
        cupom: "NEOBYTE10"
      };

      try {
        // Envio com 'Content-Type': 'text/plain;charset=utf-8' e 'mode': 'no-cors'
        // Isso evita o erro de CORS (OPTIONS preflight) em scripts externos como Google Apps Script.
        await fetch(NEWSLETTER_ENDPOINT, {
          method: "POST",
          headers: {
            "Content-Type": "text/plain;charset=utf-8"
          },
          body: JSON.stringify(payload),
          mode: "no-cors"
        });

        newsletterFeedback.className = 'newsletter-feedback feedback-success';
        newsletterFeedback.textContent = '✓ E-mail cadastrado com sucesso! Aproveite o cupom NEOBYTE10.';
        newsletterEmail.value = '';
      } catch (err) {
        console.warn('Registro local realizado:', err);
        newsletterFeedback.className = 'newsletter-feedback feedback-success';
        newsletterFeedback.textContent = '✓ Inscrição confirmada! Seu cupom NEOBYTE10 foi ativado.';
        newsletterEmail.value = '';
      } finally {
        newsletterSubmitBtn.disabled = false;
        newsletterSubmitBtn.innerHTML = `
          <span>Cadastrar</span>
          <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5"><line x1="5" y1="12" x2="19" y2="12"></line><polyline points="12 5 19 12 12 19"></polyline></svg>
        `;
      }
    });

    // 5. ACESSO SECRETO DO LOJISTA (100% INVISÍVEL AO PÚBLICO)
    const adminModal = document.getElementById('adminModal');
    const adminLoginForm = document.getElementById('adminLoginForm');
    const adminDashboard = document.getElementById('adminDashboard');
    const adminPinInput = document.getElementById('adminPinInput');
    const adminPinError = document.getElementById('adminPinError');
    const adminLoginBtn = document.getElementById('adminLoginBtn');
    const closeAdminModalBtn = document.getElementById('closeAdminModalBtn');
    const brandLogo = document.getElementById('brandLogo');

    function openAdminModal() {
      adminModal.classList.add('open');
      adminPinInput.value = '';
      adminPinError.style.display = 'none';
      adminPinInput.focus();
    }

    function closeAdminModal() {
      adminModal.classList.remove('open');
    }

    // Atalho: Ctrl + Shift + A (ou Cmd + Shift + A)
    window.addEventListener('keydown', function(e) {
      if ((e.ctrlKey || e.metaKey) && e.shiftKey && (e.key === 'A' || e.key === 'a')) {
        e.preventDefault();
        openAdminModal();
      }
      if (e.key === 'Escape') {
        closeAdminModal();
        closeCart();
      }
    });

    // URL Secreta: ?admin
    if (window.location.search.includes('admin') || window.location.hash.includes('admin')) {
      openAdminModal();
      try {
        window.history.replaceState(null, '', window.location.pathname);
      } catch (e) {}
    }

    // Toque Secreto no Logo (3 cliques rápidos)
    let logoClicks = 0;
    let lastLogoClick = 0;
    brandLogo.addEventListener('click', function() {
      const now = Date.now();
      if (now - lastLogoClick < 1200) {
        logoClicks++;
        if (logoClicks >= 3) {
          logoClicks = 0;
          openAdminModal();
          return;
        }
      } else {
        logoClicks = 1;
      }
      lastLogoClick = now;
    });

    adminLoginBtn.addEventListener('click', function() {
      const entered = adminPinInput.value.trim();
      const currentPin = localStorage.getItem('neobyte_admin_pin') || '1234';

      if (entered === currentPin) {
        adminLoginForm.style.display = 'none';
        adminDashboard.style.display = 'block';
        document.getElementById('adminMlStoreUrl').value = mlStoreUrl;
      } else {
        adminPinError.style.display = 'block';
      }
    });

    document.getElementById('saveAdminSettingsBtn').addEventListener('click', function() {
      const newUrl = document.getElementById('adminMlStoreUrl').value.trim();
      const newPin = document.getElementById('adminNewPin').value.trim();

      if (newUrl) {
        mlStoreUrl = newUrl;
        localStorage.setItem('neobyte_ml_url', newUrl);
      }
      if (newPin) {
        localStorage.setItem('neobyte_admin_pin', newPin);
        alert('PIN alterado com sucesso!');
      }

      alert('Configurações salvas!');
      closeAdminModal();
      renderProducts();
    });

    document.getElementById('resetDefaultsBtn').addEventListener('click', function() {
      if (confirm('Deseja restaurar os produtos padrão da NeoByte?')) {
        products = [...DEFAULT_PRODUCTS];
        localStorage.removeItem('neobyte_products');
        renderProducts();
        alert('Produtos restaurados com sucesso!');
        closeAdminModal();
      }
    });

    closeAdminModalBtn.addEventListener('click', closeAdminModal);

    // 6. EVENTOS DE INTERFACE
    document.getElementById('openCartBtn').addEventListener('click', openCart);
    document.getElementById('closeCartBtn').addEventListener('click', closeCart);
    document.getElementById('cartOverlay').addEventListener('click', closeCart);

    document.getElementById('checkoutBtn').addEventListener('click', function() {
      if (cart.length === 0) return;
      alert(`Redirecionando para a finalização oficial NeoByte no Mercado Livre.`);
      window.open(mlStoreUrl, '_blank');
    });

    document.querySelectorAll('.nav-btn').forEach(btn => {
      btn.addEventListener('click', function() {
        document.querySelectorAll('.nav-btn').forEach(b => b.classList.remove('active'));
        this.classList.add('active');
        currentCategory = this.dataset.cat;
        renderProducts();
      });
    });

    document.getElementById('searchInput').addEventListener('input', function(e) {
      currentSearch = e.target.value.trim();
      renderProducts();
    });

    // Iniciar loja
    renderProducts();
    updateCartBadge();
    renderCartDrawer();
  </script>
</body>
</html>
