<!DOCTYPE html>
<html lang="pt-BR" class="scroll-smooth">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>ATELIER MADEIRA — Bancos Artesanais de Madeira Maciça</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Playfair+Display:ital,wght@0,500;0,600;1,400&display=swap" rel="stylesheet" />
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            sand: '#FAF8F5',
            sandDark: '#F1ECE4',
            charcoal: '#1F1E1C',
            wood: '#8B5A2B',
            woodHover: '#704720',
            woodLight: '#F4EDE4',
            freeGreen: '#2E6F40',
            freeGreenBg: '#EBF5EE'
          },
          fontFamily: {
            sans: ['Inter', 'sans-serif'],
            serif: ['Playfair Display', 'serif']
          }
        }
      }
    };
  </script>
</head>
<body class="bg-sand text-charcoal font-sans antialiased selection:bg-wood selection:text-white">

  <!-- Barra de Aviso Superior -->
  <div class="bg-charcoal text-sand text-xs sm:text-sm py-2.5 px-4 text-center tracking-wide">
    <span>Artesanal em Madeira Maciça &bull; Suporta até 150 kg &bull; </span>
    <span class="font-semibold text-amber-200">Frete Grátis a partir de R$ 150,00 (ou na Banqueta Alta 70 cm)</span>
  </div>

  <!-- Cabeçalho Minimalista -->
  <header class="sticky top-0 z-30 bg-sand/90 backdrop-blur-md border-b border-stone-200/80">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 h-16 sm:h-20 flex items-center justify-between">
      <!-- Marca -->
      <a href="#" class="flex items-center gap-2.5 group">
        <div class="w-9 h-9 rounded-xl bg-wood text-white flex items-center justify-center shadow-sm transition-transform group-hover:scale-105">
          <!-- Ícone minimalista de banco -->
          <svg class="w-5 h-5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round">
            <ellipse cx="12" cy="6" rx="7" ry="2.2" />
            <path d="M7 7.5L5 20" />
            <path d="M17 7.5L19 20" />
            <path d="M6.2 14.5H17.8" />
          </svg>
        </div>
        <div>
          <span class="font-serif text-lg sm:text-xl font-semibold tracking-tight text-charcoal block leading-none">ATELIER MADEIRA</span>
          <span class="text-[10px] uppercase tracking-[0.2em] text-stone-500 block mt-0.5">Design Artesanal</span>
        </div>
      </a>

      <!-- Navegação Desktop -->
      <nav class="hidden md:flex items-center gap-8 text-sm font-medium text-stone-600">
        <a href="#colecao" class="hover:text-wood transition-colors">Coleção</a>
        <a href="#proporcoes" class="hover:text-wood transition-colors">Comparativo de Altura</a>
        <a href="#diferenciais" class="hover:text-wood transition-colors">Artesanato</a>
      </nav>

      <!-- Botão Carrinho -->
      <button onclick="toggleCart(true)" aria-label="Abrir carrinho" class="relative inline-flex items-center gap-2.5 bg-white hover:bg-stone-50 text-charcoal border border-stone-200/90 px-4 py-2.5 rounded-full shadow-sm transition-all active:scale-95">
        <svg class="w-5 h-5 text-wood" fill="none" stroke="currentColor" stroke-width="1.8" viewBox="0 0 24 24">
          <path stroke-linecap="round" stroke-linejoin="round" d="M16 11V7a4 4 0 00-8 0v4M5 9h14l1 12H4L5 9z" />
        </svg>
        <span class="text-sm font-medium hidden sm:inline">Sacola</span>
        <span id="cart-badge" class="inline-flex items-center justify-center min-w-[22px] h-[22px] px-1.5 text-xs font-semibold rounded-full bg-wood text-white">0</span>
      </button>
    </div>
  </header>

  <!-- Seção Hero Minimalista -->
  <section class="relative overflow-hidden border-b border-stone-200/70">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 py-12 sm:py-20 lg:py-24">
      <div class="grid grid-cols-1 lg:grid-cols-12 gap-10 lg:gap-12 items-center">
        <!-- Texto Hero -->
        <div class="lg:col-span-7 space-y-6">
          <div class="inline-flex items-center gap-2 px-3.5 py-1.5 rounded-full bg-woodLight text-wood text-xs font-semibold tracking-wide uppercase">
            <span>Edição Permanente &bull; Feito à Mão</span>
          </div>

          <h1 class="font-serif text-4xl sm:text-5xl lg:text-[54px] font-medium text-charcoal leading-[1.12] tracking-tight">
            Estilo rústico e minimalista em <span class="italic text-wood">madeira maciça</span>.
          </h1>

          <p class="text-stone-600 text-base sm:text-lg max-w-xl leading-relaxed font-normal">
            Bancos torneados artesanalmente com acabamento acetinado natural. Projetados para valorizar desde cantos de leitura até bancadas e ilhas gourmet — já chegam montados e prontos para usar.
          </p>

          <!-- Botões de Ação -->
          <div class="flex flex-wrap items-center gap-3.5 pt-2">
            <a href="#colecao" class="inline-flex items-center justify-center gap-2 bg-wood hover:bg-woodHover text-white font-medium text-sm sm:text-base px-7 py-3.5 rounded-full shadow-sm transition-all active:scale-95">
              <span>Ver Coleção</span>
              <svg class="w-4 h-4" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" d="M19 9l-7 7-7-7" />
              </svg>
            </a>
            <a href="#proporcoes" class="inline-flex items-center justify-center bg-white hover:bg-stone-50 text-charcoal border border-stone-200 font-medium text-sm sm:text-base px-6 py-3.5 rounded-full transition-all">
              Comparar Medidas
            </a>
          </div>

          <!-- Destaques Rápidos -->
          <div class="grid grid-cols-3 gap-3 sm:gap-6 pt-6 border-t border-stone-200/80 max-w-lg">
            <div>
              <p class="text-xs uppercase tracking-wider text-stone-400 font-medium">Resistência</p>
              <p class="text-sm sm:text-base font-semibold text-charcoal mt-0.5">Suporta 150 kg</p>
            </div>
            <div>
              <p class="text-xs uppercase tracking-wider text-stone-400 font-medium">Material</p>
              <p class="text-sm sm:text-base font-semibold text-charcoal mt-0.5">Madeira Maciça</p>
            </div>
            <div>
              <p class="text-xs uppercase tracking-wider text-stone-400 font-medium">Montagem</p>
              <p class="text-sm sm:text-base font-semibold text-charcoal mt-0.5">Pronto p/ Uso</p>
            </div>
          </div>
        </div>

        <!-- Ilustração Proporcional dos 3 Bancos no Hero -->
        <div class="lg:col-span-5">
          <div class="bg-white rounded-3xl border border-stone-200/80 p-6 sm:p-8 shadow-sm relative">
            <div class="flex items-center justify-between text-xs text-stone-400 mb-4">
              <span class="uppercase tracking-widest font-medium">Escala Real Proporcional</span>
              <span class="text-wood font-medium">30cm &bull; 50cm &bull; 70cm</span>
            </div>

            <!-- SVG ilustrativo proporcional fiel aos bancos torneados com anéis decorativos -->
            <div class="w-full flex items-end justify-center pt-4 pb-2">
              <svg viewBox="0 0 380 260" class="w-full max-w-md h-auto" aria-label="Ilustração comparativa dos bancos de 30cm, 50cm e 70cm">
                <defs>
                  <linearGradient id="woodTop" x1="0%" y1="0%" x2="100%" y2="0%">
                    <stop offset="0%" stop-color="#B0743E" />
                    <stop offset="50%" stop-color="#8B5A2B" />
                    <stop offset="100%" stop-color="#6E441E" />
                  </linearGradient>
                  <linearGradient id="woodLeg" x1="0%" y1="0%" x2="100%" y2="0%">
                    <stop offset="0%" stop-color="#A66B37" />
                    <stop offset="60%" stop-color="#835224" />
                    <stop offset="100%" stop-color="#5E3917" />
                  </linearGradient>
                </defs>

                <!-- Linha de chão -->
                <line x1="20" y1="230" x2="360" y2="230" stroke="#E5DFD5" stroke-width="2" stroke-linecap="round" />

                <!-- 1. BANCO BAIXO (30cm) -->
                <g transform="translate(32, 0)">
                  <!-- Pernas traseiras -->
                  <path d="M26 154 L18 228" stroke="#5E3917" stroke-width="7" stroke-linecap="round" />
                  <path d="M62 154 L70 228" stroke="#5E3917" stroke-width="7" stroke-linecap="round" />
                  <!-- Travessas -->
                  <line x1="16" y1="196" x2="72" y2="196" stroke="#70451D" stroke-width="4.5" stroke-linecap="round" />
                  <!-- Pernas dianteiras -->
                  <path d="M22 154 L10 230" stroke="url(#woodLeg)" stroke-width="8.5" stroke-linecap="round" />
                  <path d="M66 154 L78 230" stroke="url(#woodLeg)" stroke-width="8.5" stroke-linecap="round" />
                  <!-- Frisos torneados -->
                  <line x1="8" y1="221" x2="15" y2="221" stroke="#3D230C" stroke-width="1.5" />
                  <line x1="73" y1="221" x2="80" y2="221" stroke="#3D230C" stroke-width="1.5" />
                  <!-- Assento -->
                  <rect x="14" y="144" width="60" height="11" rx="5.5" fill="url(#woodTop)" />
                  <ellipse cx="44" cy="144" rx="30" ry="4" fill="#BD8048" />
                  <!-- Cota 30cm -->
                  <text x="44" y="248" text-anchor="middle" fill="#1F1E1C" font-size="11" font-weight="600">30 cm</text>
                  <text x="44" y="132" text-anchor="middle" fill="#8B5A2B" font-size="10" font-weight="500">R$ 90</text>
                </g>

                <!-- 2. BANCO MÉDIO (50cm) -->
                <g transform="translate(142, 0)">
                  <!-- Pernas traseiras -->
                  <path d="M28 104 L18 228" stroke="#5E3917" stroke-width="7" stroke-linecap="round" />
                  <path d="M72 104 L82 228" stroke="#5E3917" stroke-width="7" stroke-linecap="round" />
                  <!-- Travessas -->
                  <line x1="16" y1="184" x2="84" y2="184" stroke="#70451D" stroke-width="4.5" stroke-linecap="round" />
                  <!-- Pernas dianteiras -->
                  <path d="M24 104 L10 230" stroke="url(#woodLeg)" stroke-width="8.5" stroke-linecap="round" />
                  <path d="M76 104 L90 230" stroke="url(#woodLeg)" stroke-width="8.5" stroke-linecap="round" />
                  <!-- Frisos torneados -->
                  <line x1="8" y1="221" x2="15" y2="221" stroke="#3D230C" stroke-width="1.5" />
                  <line x1="85" y1="221" x2="92" y2="221" stroke="#3D230C" stroke-width="1.5" />
                  <line x1="20" y1="126" x2="27" y2="126" stroke="#3D230C" stroke-width="1.5" />
                  <line x1="73" y1="126" x2="80" y2="126" stroke="#3D230C" stroke-width="1.5" />
                  <!-- Assento -->
                  <rect x="14" y="94" width="72" height="11" rx="5.5" fill="url(#woodTop)" />
                  <ellipse cx="50" cy="94" rx="36" ry="4.5" fill="#BD8048" />
                  <!-- Cota 50cm -->
                  <text x="50" y="248" text-anchor="middle" fill="#1F1E1C" font-size="11" font-weight="600">50 cm</text>
                  <text x="50" y="82" text-anchor="middle" fill="#8B5A2B" font-size="10" font-weight="500">R$ 120</text>
                </g>

                <!-- 3. BANQUETA ALTA (70cm) -->
                <g transform="translate(262, 0)">
                  <!-- Pernas traseiras -->
                  <path d="M28 54 L17 228" stroke="#5E3917" stroke-width="7" stroke-linecap="round" />
                  <path d="M72 54 L83 228" stroke="#5E3917" stroke-width="7" stroke-linecap="round" />
                  <!-- Travessas -->
                  <line x1="15" y1="176" x2="85" y2="176" stroke="#70451D" stroke-width="4.5" stroke-linecap="round" />
                  <!-- Pernas dianteiras -->
                  <path d="M24 54 L9 230" stroke="url(#woodLeg)" stroke-width="8.5" stroke-linecap="round" />
                  <path d="M76 54 L91 230" stroke="url(#woodLeg)" stroke-width="8.5" stroke-linecap="round" />
                  <!-- Frisos torneados -->
                  <line x1="7" y1="221" x2="14" y2="221" stroke="#3D230C" stroke-width="1.5" />
                  <line x1="86" y1="221" x2="93" y2="221" stroke="#3D230C" stroke-width="1.5" />
                  <!-- Assento -->
                  <rect x="14" y="44" width="72" height="11" rx="5.5" fill="url(#woodTop)" />
                  <ellipse cx="50" cy="44" rx="36" ry="4.5" fill="#BD8048" />
                  <!-- Cota 70cm -->
                  <text x="50" y="248" text-anchor="middle" fill="#1F1E1C" font-size="11" font-weight="600">70 cm</text>
                  <text x="50" y="30" text-anchor="middle" fill="#2E6F40" font-size="10" font-weight="700">R$ 150 • FRETE GRÁTIS</text>
                </g>
              </svg>
            </div>

            <div class="mt-4 pt-4 border-t border-stone-100 flex items-center justify-between text-xs text-stone-500">
              <span>Acabamento artesanal torneado</span>
              <span class="font-medium text-charcoal">A partir de R$ 90,00</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Vitrine de Produtos -->
  <section id="colecao" class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 py-16 sm:py-24">
    <div class="flex flex-col md:flex-row md:items-end justify-between gap-4 mb-12">
      <div>
        <span class="text-xs font-semibold uppercase tracking-[0.2em] text-wood">Nossa Coleção</span>
        <h2 class="font-serif text-3xl sm:text-4xl font-medium text-charcoal mt-1.5">Três alturas, a mesma essência</h2>
      </div>
      <p class="text-stone-500 text-sm sm:text-base max-w-md">
        Escolha a medida ideal para o seu ambiente. Pedidos a partir de <strong class="text-charcoal font-medium">R$ 150,00</strong> ganham <strong class="text-freeGreen font-medium">Frete Grátis</strong> automaticamente.
      </p>
    </div>

    <!-- Grid de 3 Cards de Produtos -->
    <div id="products-grid" class="grid grid-cols-1 md:grid-cols-3 gap-7 lg:gap-8">
      <!-- Renderizado dinamicamente via JS -->
    </div>
  </section>

  <!-- Calculadora Rápida de Frete na Página -->
  <section class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 pb-16">
    <div class="bg-white rounded-3xl border border-stone-200/80 p-6 sm:p-10 shadow-sm">
      <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
        <div class="lg:col-span-7 space-y-2">
          <div class="inline-flex items-center gap-2 text-xs font-semibold uppercase tracking-wider text-wood">
            <svg class="w-4 h-4" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" d="M5 8h14M5 8a2 2 0 110-4h14a2 2 0 110 4M5 8v10a2 2 0 002 2h10a2 2 0 002-2V8m-9 4h4" />
            </svg>
            <span>Envio Seguro & Embalagem Reforçada</span>
          </div>
          <h3 class="font-serif text-2xl sm:text-3xl font-medium text-charcoal">Simule o prazo e frete para seu CEP</h3>
          <p class="text-stone-500 text-sm sm:text-base">
            Bancos de 30 cm (R$ 90) e 50 cm (R$ 120) possuem frete econômico calculado pelo CEP. Na compra da Banqueta Alta de 70 cm (R$ 150) ou combinando 2 bancos menores, o <strong class="text-freeGreen font-medium">frete é por nossa conta</strong>.
          </p>
        </div>

        <div class="lg:col-span-5">
          <form onsubmit="handlePageCepSubmit(event)" class="flex flex-col sm:flex-row gap-2.5">
            <input
              type="text"
              id="page-cep-input"
              maxlength="9"
              placeholder="Digite seu CEP (ex: 01310-100)"
              oninput="maskCep(this)"
              class="w-full px-4 py-3 rounded-xl bg-sand border border-stone-200 text-charcoal placeholder-stone-400 text-sm focus:outline-none focus:border-wood transition-colors"
            />
            <button type="submit" class="px-6 py-3 rounded-xl bg-charcoal hover:bg-stone-800 text-white font-medium text-sm whitespace-nowrap transition-colors">
              Calcular
            </button>
          </form>
          <div id="page-cep-result" class="mt-3 text-sm text-stone-600 hidden"></div>
        </div>
      </div>
    </div>
  </section>

  <!-- Guia de Proporções e Uso -->
  <section id="proporcoes" class="bg-sandDark/60 border-y border-stone-200/70 py-16 sm:py-24">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center max-w-2xl mx-auto mb-14">
        <span class="text-xs font-semibold uppercase tracking-[0.2em] text-wood">Guia de Escolha</span>
        <h2 class="font-serif text-3xl sm:text-4xl font-medium text-charcoal mt-2">Qual altura combina com seu espaço?</h2>
        <p class="text-stone-600 text-sm sm:text-base mt-3">
          Cada banco foi dimensionado ergonomicamente para oferecer conforto e estabilidade no dia a dia.
        </p>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
        <!-- Guia 30cm -->
        <div class="bg-white rounded-2xl p-6 sm:p-7 border border-stone-200/70">
          <div class="flex items-center justify-between mb-4">
            <span class="px-3 py-1 rounded-full bg-sand text-charcoal text-xs font-semibold">Altura 30 cm</span>
            <span class="text-xs text-stone-400">Assento Ø 21 cm</span>
          </div>
          <h3 class="font-semibold text-lg text-charcoal">Banco Baixo (Pequeno)</h3>
          <p class="text-stone-500 text-sm mt-2 leading-relaxed">
            Leve e super fácil de transportar. Perfeito como apoio para os pés ao lado do sofá, mesa lateral para plantas ou assento infantil.
          </p>
          <div class="mt-5 pt-4 border-t border-stone-100 flex items-center justify-between text-sm">
            <span class="text-stone-400">Investimento</span>
            <span class="font-semibold text-charcoal">R$ 90,00 <span class="text-xs font-normal text-stone-400">+ frete</span></span>
          </div>
        </div>

        <!-- Guia 50cm -->
        <div class="bg-white rounded-2xl p-6 sm:p-7 border border-stone-200/70">
          <div class="flex items-center justify-between mb-4">
            <span class="px-3 py-1 rounded-full bg-sand text-charcoal text-xs font-semibold">Altura 50 cm</span>
            <span class="text-xs text-stone-400">Assento Ø 28 cm</span>
          </div>
          <h3 class="font-semibold text-lg text-charcoal">Banco Médio</h3>
          <p class="text-stone-500 text-sm mt-2 leading-relaxed">
            A altura padrão de cadeiras. Ideal para mesas de jantar, escrivaninhas de estudo, penteadeiras ou para acomodar visitas extras.
          </p>
          <div class="mt-5 pt-4 border-t border-stone-100 flex items-center justify-between text-sm">
            <span class="text-stone-400">Investimento</span>
            <span class="font-semibold text-charcoal">R$ 120,00 <span class="text-xs font-normal text-stone-400">+ frete</span></span>
          </div>
        </div>

        <!-- Guia 70cm -->
        <div class="bg-white rounded-2xl p-6 sm:p-7 border-2 border-wood/30 relative">
          <div class="flex items-center justify-between mb-4">
            <span class="px-3 py-1 rounded-full bg-woodLight text-wood text-xs font-semibold">Altura 70 cm</span>
            <span class="text-xs text-stone-400">Assento Ø 28 cm</span>
          </div>
          <h3 class="font-semibold text-lg text-charcoal">Banqueta Alta (Grande)</h3>
          <p class="text-stone-500 text-sm mt-2 leading-relaxed">
            Desenvolvida para bancadas de cozinha americana, ilhas gourmet e balcões altos (entre 95 cm e 105 cm de altura).
          </p>
          <div class="mt-5 pt-4 border-t border-stone-100 flex items-center justify-between text-sm">
            <span class="px-2.5 py-0.5 rounded-full bg-freeGreenBg text-freeGreen text-xs font-semibold">Frete Grátis</span>
            <span class="font-semibold text-charcoal">R$ 150,00</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Seção Diferenciais Artesanais -->
  <section id="diferenciais" class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 py-16 sm:py-24">
    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-6">
      <div class="bg-white p-6 rounded-2xl border border-stone-200/70 space-y-3">
        <div class="w-10 h-10 rounded-xl bg-woodLight text-wood flex items-center justify-center">
          <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="1.8" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" d="M5 3v4M3 5h4M6 17v4m-2-2h4m5-16l2.286 6.857L21 12l-5.714 2.143L13 21l-2.286-6.857L5 12l5.714-2.143L13 3z" />
          </svg>
        </div>
        <h4 class="font-semibold text-charcoal">Acabamento Artesanal</h4>
        <p class="text-sm text-stone-500 leading-relaxed">Torneados cuidadosamente com frisos clássicos e verniz acetinado que realça os veios naturais da madeira.</p>
      </div>

      <div class="bg-white p-6 rounded-2xl border border-stone-200/70 space-y-3">
        <div class="w-10 h-10 rounded-xl bg-woodLight text-wood flex items-center justify-center">
          <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="1.8" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" d="M9 12l2 2 4-4m5.618-4.016A11.955 11.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.02 12.02 0 003 9c0 5.591 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.042-.133-2.052-.382-3.016z" />
          </svg>
        </div>
        <h4 class="font-semibold text-charcoal">Suporta até 150 kg</h4>
        <p class="text-sm text-stone-500 leading-relaxed">Estrutura firme em madeira maciça com travessas inferiores reforçadas para máxima estabilidade e segurança.</p>
      </div>

      <div class="bg-white p-6 rounded-2xl border border-stone-200/70 space-y-3">
        <div class="w-10 h-10 rounded-xl bg-woodLight text-wood flex items-center justify-center">
          <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="1.8" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" d="M20 7l-8-4-8 4m16 0l-8 4m8-4v10l-8 4m0-10L4 7m8 4v10M4 7v10l8 4" />
          </svg>
        </div>
        <h4 class="font-semibold text-charcoal">Pronto para Usar</h4>
        <p class="text-sm text-stone-500 leading-relaxed">Sem parafusos ou manuais complicados. Seu banco chega 100% montado, direto da marcenaria para sua casa.</p>
      </div>

      <div class="bg-white p-6 rounded-2xl border border-stone-200/70 space-y-3">
        <div class="w-10 h-10 rounded-xl bg-freeGreenBg text-freeGreen flex items-center justify-center">
          <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="1.8" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" d="M12 8v13m0-13V6a2 2 0 112 2h-2zm0 0V5.5A2.5 2.5 0 109.5 8H12zm-7 4h14M5 12a2 2 0 110-4h14a2 2 0 110 4M5 12v7a2 2 0 002 2h10a2 2 0 002-2v-7" />
          </svg>
        </div>
        <h4 class="font-semibold text-charcoal">Frete Grátis a partir de R$ 150</h4>
        <p class="text-sm text-stone-500 leading-relaxed">Adquira a Banqueta Alta de 70 cm ou combine modelos menores para aproveitar entrega gratuita em todo o Brasil.</p>
      </div>
    </div>
  </section>

  <!-- Rodapé Minimalista -->
  <footer class="bg-white border-t border-stone-200/80 py-12">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col sm:flex-row items-center justify-between gap-6">
      <div class="text-center sm:text-left">
        <span class="font-serif text-lg font-semibold text-charcoal">ATELIER MADEIRA</span>
        <p class="text-xs text-stone-500 mt-1">Mobiliário artesanal em madeira maciça &bull; Feito no Brasil</p>
      </div>
      <div class="flex items-center gap-6 text-xs text-stone-500">
        <span>Suporte: contato@ateliermadeira.com.br</span>
        <span>&copy; 2026 Todos os direitos reservados</span>
      </div>
    </div>
  </footer>

  <!-- MODAL DE DETALHES TÉCNICOS DO PRODUTO -->
  <div id="product-modal" class="fixed inset-0 z-50 hidden items-center justify-center p-4 bg-charcoal/50 backdrop-blur-xs">
    <div class="bg-white rounded-3xl max-w-2xl w-full overflow-hidden shadow-2xl border border-stone-200 animate-[fadeIn_0.2s_ease-out]">
      <div id="product-modal-content"></div>
    </div>
  </div>

  <!-- DRAWER LATERAL DO CARRINHO -->
  <div id="cart-overlay" onclick="toggleCart(false)" class="fixed inset-0 z-40 bg-charcoal/40 backdrop-blur-xs hidden transition-opacity"></div>
  <aside id="cart-drawer" class="fixed top-0 right-0 z-50 h-full w-full max-w-md bg-white shadow-2xl border-l border-stone-200 transform translate-x-full transition-transform duration-300 flex flex-col">
    <!-- Cabeçalho Drawer -->
    <div class="px-6 py-5 border-b border-stone-100 flex items-center justify-between">
      <div>
        <h3 class="font-serif text-xl font-medium text-charcoal">Sua Sacola</h3>
        <p id="drawer-subtitle" class="text-xs text-stone-400 mt-0.5">0 itens selecionados</p>
      </div>
      <button onclick="toggleCart(false)" aria-label="Fechar sacola" class="p-2 rounded-full hover:bg-stone-100 text-stone-500 transition-colors">
        <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24">
          <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
        </svg>
      </button>
    </div>

    <!-- Barra de Progresso Frete Grátis -->
    <div id="free-shipping-bar-container" class="px-6 py-3.5 bg-sand border-b border-stone-200/70">
      <div class="flex items-center justify-between text-xs font-medium mb-1.5">
        <span id="free-shipping-msg" class="text-charcoal">Faltam R$ 150,00 para Frete Grátis</span>
        <span id="free-shipping-pct" class="text-wood font-semibold">0%</span>
      </div>
      <div class="w-full h-2 bg-stone-200 rounded-full overflow-hidden">
        <div id="free-shipping-progress" class="h-full bg-wood rounded-full transition-all duration-300" style="width: 0%"></div>
      </div>
    </div>

    <!-- Lista de Itens do Carrinho -->
    <div id="cart-items-container" class="flex-1 overflow-y-auto px-6 py-4 space-y-4">
      <!-- Renderizado dinamicamente -->
    </div>

    <!-- Rodapé do Carrinho (CEP, Totais e Botão Checkout) -->
    <div id="cart-footer" class="border-t border-stone-200 bg-sand/60 px-6 py-5 space-y-4">
      <!-- Calculadora de CEP no Drawer -->
      <div>
        <label for="drawer-cep-input" class="block text-xs font-medium text-stone-600 mb-1.5">Calcular Frete (CEP)</label>
        <div class="flex gap-2">
          <input
            type="text"
            id="drawer-cep-input"
            maxlength="9"
            placeholder="00000-000"
            oninput="maskCep(this)"
            class="flex-1 px-3.5 py-2 rounded-xl bg-white border border-stone-200 text-sm text-charcoal focus:outline-none focus:border-wood"
          />
          <button onclick="calculateDrawerCep()" class="px-4 py-2 rounded-xl bg-charcoal hover:bg-stone-800 text-white text-xs font-medium transition-colors">
            OK
          </button>
        </div>
        <p id="drawer-cep-status" class="text-xs text-stone-500 mt-1.5"></p>
      </div>

      <!-- Resumo de Valores -->
      <div class="space-y-1.5 text-sm pt-2 border-t border-stone-200/80">
        <div class="flex justify-between text-stone-600">
          <span>Subtotal</span>
          <span id="cart-subtotal">R$ 0,00</span>
        </div>
        <div class="flex justify-between items-center text-stone-600">
          <span>Frete</span>
          <span id="cart-shipping" class="font-medium">Calcule o CEP</span>
        </div>
        <div class="flex justify-between text-base font-semibold text-charcoal pt-2 border-t border-stone-200/80">
          <span>Total</span>
          <span id="cart-total">R$ 0,00</span>
        </div>
      </div>

      <button onclick="openCheckoutModal()" id="btn-checkout" class="w-full py-3.5 px-6 rounded-full bg-wood hover:bg-woodHover disabled:opacity-40 disabled:pointer-events-none text-white font-medium text-sm shadow-sm transition-all active:scale-98">
        Finalizar Pedido
      </button>
    </div>
  </aside>

  <!-- MODAL DE CHECKOUT SIMULADO -->
  <div id="checkout-modal" class="fixed inset-0 z-50 hidden items-center justify-center p-4 bg-charcoal/50 backdrop-blur-xs">
    <div class="bg-white rounded-3xl max-w-lg w-full max-h-[92vh] overflow-y-auto shadow-2xl border border-stone-200 p-6 sm:p-8">
      <div id="checkout-form-view">
        <div class="flex items-center justify-between pb-4 border-b border-stone-100">
          <div>
            <span class="text-[11px] font-semibold uppercase tracking-widest text-wood">Finalização Segura</span>
            <h3 class="font-serif text-2xl font-medium text-charcoal">Dados de Entrega</h3>
          </div>
          <button onclick="closeCheckoutModal()" class="p-2 rounded-full hover:bg-stone-100 text-stone-500">
            <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
            </svg>
          </button>
        </div>

        <form onsubmit="submitOrder(event)" class="space-y-4 mt-5">
          <div>
            <label class="block text-xs font-medium text-stone-700 mb-1">Nome Completo *</label>
            <input type="text" id="chk-name" required placeholder="Ex: Mariana Oliveira" class="w-full px-4 py-2.5 rounded-xl bg-sand border border-stone-200 text-sm focus:outline-none focus:border-wood" />
          </div>

          <div class="grid grid-cols-1 sm:grid-cols-2 gap-3">
            <div>
              <label class="block text-xs font-medium text-stone-700 mb-1">CEP *</label>
              <input type="text" id="chk-cep" required maxlength="9" oninput="maskCep(this); syncCheckoutCep(this.value)" placeholder="00000-000" class="w-full px-4 py-2.5 rounded-xl bg-sand border border-stone-200 text-sm focus:outline-none focus:border-wood" />
            </div>
            <div>
              <label class="block text-xs font-medium text-stone-700 mb-1">WhatsApp / Telefone *</label>
              <input type="tel" id="chk-phone" required placeholder="(11) 99999-9999" class="w-full px-4 py-2.5 rounded-xl bg-sand border border-stone-200 text-sm focus:outline-none focus:border-wood" />
            </div>
          </div>

          <div>
            <label class="block text-xs font-medium text-stone-700 mb-1">Endereço Completo (Rua, Número, Bairro, Cidade/UF) *</label>
            <input type="text" id="chk-address" required placeholder="Rua das Acácias, 240 - Jardim Paulista, São Paulo/SP" class="w-full px-4 py-2.5 rounded-xl bg-sand border border-stone-200 text-sm focus:outline-none focus:border-wood" />
          </div>

          <!-- Forma de Pagamento -->
          <div class="pt-2">
            <label class="block text-xs font-medium text-stone-700 mb-2">Forma de Pagamento</label>
            <div class="grid grid-cols-2 gap-3">
              <label class="cursor-pointer">
                <input type="radio" name="paymentMethod" value="pix" checked onchange="updateCheckoutSummary()" class="peer sr-only" />
                <div class="p-3.5 rounded-2xl border border-stone-200 peer-checked:border-wood peer-checked:bg-woodLight/50 transition-all">
                  <div class="flex items-center justify-between">
                    <span class="text-sm font-semibold text-charcoal">Pix</span>
                    <span class="text-[10px] font-bold px-2 py-0.5 rounded-full bg-freeGreenBg text-freeGreen">-5% OFF</span>
                  </div>
                  <p class="text-xs text-stone-500 mt-1">Aprovação imediata</p>
                </div>
              </label>

              <label class="cursor-pointer">
                <input type="radio" name="paymentMethod" value="card" onchange="updateCheckoutSummary()" class="peer sr-only" />
                <div class="p-3.5 rounded-2xl border border-stone-200 peer-checked:border-wood peer-checked:bg-woodLight/50 transition-all">
                  <span class="text-sm font-semibold text-charcoal block">Cartão</span>
                  <p class="text-xs text-stone-500 mt-1">Até 3x sem juros</p>
                </div>
              </label>
            </div>
          </div>

          <!-- Resumo Final no Checkout -->
          <div class="bg-sand rounded-2xl p-4 space-y-1.5 text-sm border border-stone-200/70">
            <div class="flex justify-between text-stone-600">
              <span>Produtos</span>
              <span id="chk-subtotal">R$ 0,00</span>
            </div>
            <div class="flex justify-between text-stone-600">
              <span>Frete</span>
              <span id="chk-shipping">R$ 0,00</span>
            </div>
            <div id="chk-discount-row" class="flex justify-between text-freeGreen font-medium">
              <span>Desconto Pix (5%)</span>
              <span id="chk-discount">- R$ 0,00</span>
            </div>
            <div class="flex justify-between text-base font-bold text-charcoal pt-2 border-t border-stone-200">
              <span>Total a Pagar</span>
              <span id="chk-total">R$ 0,00</span>
            </div>
          </div>

          <button type="submit" class="w-full py-3.5 px-6 rounded-full bg-wood hover:bg-woodHover text-white font-medium text-sm shadow-sm transition-all">
            Confirmar Pedido
          </button>
        </form>
      </div>

      <!-- Tela de Sucesso do Pedido -->
      <div id="checkout-success-view" class="hidden text-center py-6 space-y-4">
        <div class="w-16 h-16 rounded-full bg-freeGreenBg text-freeGreen mx-auto flex items-center justify-center">
          <svg class="w-8 h-8" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" d="M5 13l4 4L19 7" />
          </svg>
        </div>
        <h3 class="font-serif text-2xl font-medium text-charcoal">Pedido Confirmado!</h3>
        <p id="order-confirmation-text" class="text-sm text-stone-600 max-w-sm mx-auto leading-relaxed"></p>
        <div class="bg-sand rounded-2xl p-4 text-xs text-stone-500 max-w-sm mx-auto">
          Código do pedido: <strong id="order-code" class="text-charcoal font-semibold">#AM-2026</strong> &bull; Enviamos os detalhes para o seu WhatsApp.
        </div>
        <button onclick="resetAfterOrder()" class="mt-2 inline-flex items-center justify-center px-7 py-3 rounded-full bg-charcoal text-white text-sm font-medium hover:bg-stone-800 transition-colors">
          Continuar Navegando
        </button>
      </div>
    </div>
  </div>

  <!-- Toast de Notificação -->
  <div id="toast" class="fixed bottom-5 left-1/2 -translate-x-1/2 z-50 bg-charcoal text-white text-sm px-5 py-3 rounded-full shadow-lg opacity-0 pointer-events-none transition-all duration-300 flex items-center gap-2">
    <span class="w-2 h-2 rounded-full bg-amber-400"></span>
    <span id="toast-message">Produto adicionado à sacola</span>
  </div>

  <script>
    // Catálogo dos 3 bancos de madeira maciça conforme especificações das imagens
    const PRODUCTS = [
      {
        id: 'banco-baixo-30',
        name: 'Banco Baixo',
        subtitle: 'Modelo Pequeno • 30 cm',
        heightCm: 30,
        diameterCm: 21,
        price: 90.00,
        freeShipping: false,
        badge: 'Compacto & Versátil',
        shortDesc: 'Compacto, leve e fácil de transportar. Ideal para apoio de pés, cantos de leitura ou crianças.',
        fullDesc: 'Produzido artesanalmente em madeira maciça selecionada com acabamento acetinado natural. Com 30 cm de altura e assento de 21 cm de diâmetro, é leve para movimentar pela casa e extremamente resistente.',
        idealFor: 'Apoio de pés, cantos de leitura, quarto infantil e suporte decorativo',
        svgScale: 'small'
      },
      {
        id: 'banco-medio-50',
        name: 'Banco Médio',
        subtitle: 'Modelo Intermediário • 50 cm',
        heightCm: 50,
        diameterCm: 28,
        price: 120.00,
        freeShipping: false,
        badge: 'Altura Padrão',
        shortDesc: 'Altura versátil, ideal para mesas de jantar, escrivaninhas ou uso diário em diversos ambientes.',
        fullDesc: 'O equilíbrio perfeito entre ergonomia e estética rústica minimalista. Com 50 cm de altura e assento amplo de 28 cm de diâmetro, acomoda confortavelmente em mesas de jantar, escritórios e varandas.',
        idealFor: 'Mesas de jantar, escrivaninhas, penteadeiras e salas de estar',
        svgScale: 'medium'
      },
      {
        id: 'banqueta-alta-70',
        name: 'Banqueta Alta',
        subtitle: 'Modelo Grande • 70 cm',
        heightCm: 70,
        diameterCm: 28,
        price: 150.00,
        freeShipping: true,
        badge: 'FRETE GRÁTIS',
        shortDesc: 'Perfeita para bancadas, ilhas gourmet e balcões. Design torneado com apoio para os pés.',
        fullDesc: 'Nossa peça de maior destaque para áreas gourmet e cozinhas integradas. Com 70 cm de altura, assento de 28 cm de diâmetro e travessas inferiores que servem de apoio confortável para os pés.',
        idealFor: 'Bancadas americanas, ilhas gourmet, bares e balcões altos',
        svgScale: 'tall'
      }
    ];

    const FREE_SHIPPING_THRESHOLD = 150.00;

    // Estado da aplicação
    let cart = [];
    let currentCep = '';
    let simulatedShippingRate = null; // null = CEP ainda não calculado

    // Gera SVG proporcional exclusivo para cada banco (30cm, 50cm, 70cm)
    function getStoolSvg(scale, uid = '') {
      // Todos compartilham a mesma linha de base (y=215) para evidenciar visualmente a diferença real de altura
      if (scale === 'small') {
        return `
          <svg viewBox="0 0 220 230" class="w-44 h-44 mx-auto drop-shadow-xs">
            <line x1="35" y1="215" x2="185" y2="215" stroke="#E5DFD5" stroke-width="2" stroke-linecap="round" />
            <!-- Cota lateral 30cm -->
            <line x1="172" y1="138" x2="172" y2="215" stroke="#C5B9A8" stroke-width="1.2" stroke-dasharray="3 3" />
            <text x="178" y="180" fill="#8B5A2B" font-size="11" font-weight="600">30cm</text>
            <!-- Pernas traseiras -->
            <path d="M84 146 L72 213" stroke="#5E3917" stroke-width="8" stroke-linecap="round" />
            <path d="M136 146 L148 213" stroke="#5E3917" stroke-width="8" stroke-linecap="round" />
            <!-- Travessa -->
            <line x1="70" y1="184" x2="150" y2="184" stroke="#70451D" stroke-width="5.5" stroke-linecap="round" />
            <!-- Pernas dianteiras -->
            <path d="M80 146 L62 215" stroke="#8B5A2B" stroke-width="10" stroke-linecap="round" />
            <path d="M140 146 L158 215" stroke="#8B5A2B" stroke-width="10" stroke-linecap="round" />
            <!-- Detalhes torneados -->
            <line x1="60" y1="205" x2="68" y2="205" stroke="#3D230C" stroke-width="1.8" />
            <line x1="152" y1="205" x2="160" y2="205" stroke="#3D230C" stroke-width="1.8" />
            <!-- Assento 21cm -->
            <rect x="68" y="135" width="84" height="12" rx="6" fill="#9A6432" />
            <ellipse cx="110" cy="135" rx="42" ry="5" fill="#BA7E46" />
          </svg>
        `;
      }

      if (scale === 'medium') {
        return `
          <svg viewBox="0 0 220 230" class="w-44 h-44 mx-auto drop-shadow-xs">
            <line x1="35" y1="215" x2="185" y2="215" stroke="#E5DFD5" stroke-width="2" stroke-linecap="round" />
            <!-- Cota lateral 50cm -->
            <line x1="176" y1="88" x2="176" y2="215" stroke="#C5B9A8" stroke-width="1.2" stroke-dasharray="3 3" />
            <text x="181" y="155" fill="#8B5A2B" font-size="11" font-weight="600">50cm</text>
            <!-- Pernas traseiras -->
            <path d="M80 96 L68 213" stroke="#5E3917" stroke-width="8" stroke-linecap="round" />
            <path d="M140 96 L152 213" stroke="#5E3917" stroke-width="8" stroke-linecap="round" />
            <!-- Travessa -->
            <line x1="65" y1="172" x2="155" y2="172" stroke="#70451D" stroke-width="5.5" stroke-linecap="round" />
            <!-- Pernas dianteiras -->
            <path d="M76 96 L58 215" stroke="#8B5A2B" stroke-width="10" stroke-linecap="round" />
            <path d="M144 96 L162 215" stroke="#8B5A2B" stroke-width="10" stroke-linecap="round" />
            <!-- Detalhes torneados -->
            <line x1="56" y1="205" x2="64" y2="205" stroke="#3D230C" stroke-width="1.8" />
            <line x1="156" y1="205" x2="164" y2="205" stroke="#3D230C" stroke-width="1.8" />
            <line x1="71" y1="118" x2="79" y2="118" stroke="#3D230C" stroke-width="1.8" />
            <line x1="141" y1="118" x2="149" y2="118" stroke="#3D230C" stroke-width="1.8" />
            <!-- Assento 28cm -->
            <rect x="60" y="85" width="100" height="12" rx="6" fill="#9A6432" />
            <ellipse cx="110" cy="85" rx="50" ry="5.5" fill="#BA7E46" />
          </svg>
        `;
      }

      // tall (70cm)
      return `
        <svg viewBox="0 0 220 230" class="w-44 h-44 mx-auto drop-shadow-xs">
          <line x1="35" y1="215" x2="185" y2="215" stroke="#E5DFD5" stroke-width="2" stroke-linecap="round" />
          <!-- Cota lateral 70cm -->
          <line x1="178" y1="36" x2="178" y2="215" stroke="#C5B9A8" stroke-width="1.2" stroke-dasharray="3 3" />
          <text x="183" y="130" fill="#2E6F40" font-size="11" font-weight="700">70cm</text>
          <!-- Pernas traseiras -->
          <path d="M80 44 L66 213" stroke="#5E3917" stroke-width="8" stroke-linecap="round" />
          <path d="M140 44 L154 213" stroke="#5E3917" stroke-width="8" stroke-linecap="round" />
          <!-- Travessa -->
          <line x1="63" y1="164" x2="157" y2="164" stroke="#70451D" stroke-width="5.5" stroke-linecap="round" />
          <!-- Pernas dianteiras -->
          <path d="M76 44 L56 215" stroke="#8B5A2B" stroke-width="10" stroke-linecap="round" />
          <path d="M144 44 L164 215" stroke="#8B5A2B" stroke-width="10" stroke-linecap="round" />
          <!-- Detalhes torneados -->
          <line x1="54" y1="205" x2="62" y2="205" stroke="#3D230C" stroke-width="1.8" />
          <line x1="158" y1="205" x2="166" y2="205" stroke="#3D230C" stroke-width="1.8" />
          <!-- Assento 28cm -->
          <rect x="60" y="33" width="100" height="12" rx="6" fill="#9A6432" />
          <ellipse cx="110" cy="33" rx="50" ry="5.5" fill="#BA7E46" />
        </svg>
      `;
    }

    function formatBRL(value) {
      return value.toLocaleString('pt-BR', { style: 'currency', currency: 'BRL' });
    }

    // Renderiza a vitrine de produtos
    function renderProducts() {
      const grid = document.getElementById('products-grid');
      grid.innerHTML = PRODUCTS.map(product => {
        const isFreeShipping = product.freeShipping;
        return `
          <article class="group bg-white rounded-3xl border ${isFreeShipping ? 'border-wood/40 ring-1 ring-wood/10' : 'border-stone-200/80'} p-6 sm:p-7 flex flex-col justify-between shadow-xs hover:shadow-md transition-all duration-300">
            <div>
              <!-- Topo do Card: Selos -->
              <div class="flex items-center justify-between gap-2 mb-4">
                <span class="px-3 py-1 rounded-full text-xs font-semibold ${isFreeShipping ? 'bg-freeGreenBg text-freeGreen' : 'bg-sand text-stone-600'}">
                  ${product.badge}
                </span>
                <span class="text-xs font-medium text-stone-400">
                  ${product.heightCm} cm &times; Ø ${product.diameterCm} cm
                </span>
              </div>

              <!-- Área Visual do Banco -->
              <div onclick="openProductModal('${product.id}')" class="cursor-pointer bg-sand/70 group-hover:bg-sand rounded-2xl py-6 px-4 mb-6 transition-colors relative">
                ${getStoolSvg(product.svgScale, product.id)}
                <span class="absolute bottom-3 right-3 text-[11px] font-medium text-stone-400 group-hover:text-wood transition-colors flex items-center gap-1">
                  Ver detalhes
                  <svg class="w-3.5 h-3.5" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M15 12a3 3 0 11-6 0 3 3 0 016 0z" />
                    <path stroke-linecap="round" stroke-linejoin="round" d="M2.458 12C3.732 7.943 7.523 5 12 5c4.478 0 8.268 2.943 9.542 7-1.274 4.057-5.064 7-9.542 7-4.477 0-8.268-2.943-9.542-7z" />
                  </svg>
                </span>
              </div>

              <!-- Título e Descrição -->
              <div class="space-y-1.5">
                <p class="text-xs uppercase tracking-wider text-wood font-medium">${product.subtitle}</p>
                <h3 class="font-serif text-2xl font-medium text-charcoal">${product.name}</h3>
                <p class="text-sm text-stone-500 leading-relaxed pt-1">
                  ${product.shortDesc}
                </p>
              </div>
            </div>

            <!-- Preço e Ações -->
            <div class="mt-6 pt-5 border-t border-stone-100 space-y-4">
              <div class="flex items-baseline justify-between">
                <div>
                  <span class="text-2xl font-semibold text-charcoal">${formatBRL(product.price)}</span>
                  ${isFreeShipping
                    ? `<span class="block text-xs font-semibold text-freeGreen mt-0.5">+ Frete Grátis para todo o Brasil</span>`
                    : `<span class="block text-xs text-stone-400 mt-0.5">+ frete (grátis a partir de R$ 150)</span>`
                  }
                </div>
                <span class="text-[11px] text-stone-400 bg-sand px-2.5 py-1 rounded-lg">Até 150 kg</span>
              </div>

              <!-- Seletor de Quantidade + Botão Adicionar -->
              <div class="flex items-center gap-2.5">
                <div class="flex items-center border border-stone-200 rounded-full bg-sand/50 px-1.5 py-1">
                  <button type="button" onclick="changeCardQty('${product.id}', -1)" aria-label="Diminuir quantidade" class="w-8 h-8 rounded-full hover:bg-white text-charcoal font-medium transition-colors">&minus;</button>
                  <span id="card-qty-${product.id}" class="w-7 text-center text-sm font-semibold text-charcoal">1</span>
                  <button type="button" onclick="changeCardQty('${product.id}', 1)" aria-label="Aumentar quantidade" class="w-8 h-8 rounded-full hover:bg-white text-charcoal font-medium transition-colors">+</button>
                </div>

                <button type="button" onclick="addToCartFromCard('${product.id}')" class="flex-1 py-3 px-4 rounded-full bg-wood hover:bg-woodHover text-white font-medium text-sm transition-all active:scale-95 shadow-xs">
                  Adicionar ao Carrinho
                </button>
              </div>
            </div>
          </article>
        `;
      }).join('');
    }

    // Controle de quantidade no card antes de adicionar
    function changeCardQty(productId, delta) {
      const el = document.getElementById(`card-qty-${productId}`);
      let current = parseInt(el.textContent, 10) || 1;
      current = Math.max(1, Math.min(20, current + delta));
      el.textContent = current;
    }

    function addToCartFromCard(productId) {
      const el = document.getElementById(`card-qty-${productId}`);
      const qty = parseInt(el.textContent, 10) || 1;
      addToCart(productId, qty);
      el.textContent = '1';
    }

    // Modal de Detalhes Técnicos
    function openProductModal(productId) {
      const product = PRODUCTS.find(p => p.id === productId);
      if (!product) return;

      const modal = document.getElementById('product-modal');
      const content = document.getElementById('product-modal-content');

      content.innerHTML = `
        <div class="grid grid-cols-1 md:grid-cols-2">
          <div class="bg-sand p-8 flex flex-col items-center justify-center relative">
            <span class="self-start px-3 py-1 rounded-full text-xs font-semibold ${product.freeShipping ? 'bg-freeGreenBg text-freeGreen' : 'bg-white text-stone-600'}">
              ${product.badge}
            </span>
            <div class="my-4">${getStoolSvg(product.svgScale, 'modal')}</div>
            <p class="text-xs text-stone-500 text-center">Ilustração em escala proporcional &bull; Madeira Maciça</p>
          </div>

          <div class="p-6 sm:p-8 flex flex-col justify-between space-y-5">
            <div>
              <div class="flex items-start justify-between gap-2">
                <div>
                  <span class="text-xs uppercase tracking-wider text-wood font-semibold">${product.subtitle}</span>
                  <h3 class="font-serif text-2xl font-medium text-charcoal mt-0.5">${product.name}</h3>
                </div>
                <button onclick="closeProductModal()" class="p-1.5 rounded-full hover:bg-stone-100 text-stone-400">
                  <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
                  </svg>
                </button>
              </div>

              <p class="text-sm text-stone-600 mt-3 leading-relaxed">${product.fullDesc}</p>

              <!-- Tabela de Especificações -->
              <div class="mt-5 space-y-2 text-xs border-t border-stone-100 pt-4">
                <div class="flex justify-between py-1 border-b border-stone-100">
                  <span class="text-stone-400">Altura Total</span>
                  <span class="font-semibold text-charcoal">${product.heightCm} cm</span>
                </div>
                <div class="flex justify-between py-1 border-b border-stone-100">
                  <span class="text-stone-400">Diâmetro do Assento</span>
                  <span class="font-semibold text-charcoal">${product.diameterCm} cm</span>
                </div>
                <div class="flex justify-between py-1 border-b border-stone-100">
                  <span class="text-stone-400">Capacidade de Peso</span>
                  <span class="font-semibold text-charcoal">Suporta até 150 kg</span>
                </div>
                <div class="flex justify-between py-1 border-b border-stone-100">
                  <span class="text-stone-400">Material & Montagem</span>
                  <span class="font-semibold text-charcoal">Madeira Maciça (Pronto p/ uso)</span>
                </div>
                <div class="py-1">
                  <span class="text-stone-400 block">Indicação de Uso</span>
                  <span class="font-medium text-charcoal mt-0.5 block">${product.idealFor}</span>
                </div>
              </div>
            </div>

            <div class="pt-4 border-t border-stone-100 flex items-center justify-between gap-4">
              <div>
                <span class="text-2xl font-bold text-charcoal block">${formatBRL(product.price)}</span>
                <span class="text-xs ${product.freeShipping ? 'text-freeGreen font-semibold' : 'text-stone-400'}">
                  ${product.freeShipping ? 'Frete Grátis incluso' : '+ frete calculado no CEP'}
                </span>
              </div>
              <button onclick="addToCart('${product.id}', 1); closeProductModal();" class="px-6 py-3 rounded-full bg-wood hover:bg-woodHover text-white text-sm font-medium transition-colors">
                Adicionar à Sacola
              </button>
            </div>
          </div>
        </div>
      `;

      modal.classList.remove('hidden');
      modal.classList.add('flex');
    }

    function closeProductModal() {
      const modal = document.getElementById('product-modal');
      modal.classList.add('hidden');
      modal.classList.remove('flex');
    }

    // Funções do Carrinho
    function addToCart(productId, quantity = 1) {
      const product = PRODUCTS.find(p => p.id === productId);
      if (!product) return;

      const existing = cart.find(item => item.id === productId);
      if (existing) {
        existing.qty += quantity;
      } else {
        cart.push({ ...product, qty: quantity });
      }

      updateCartUI();
      showToast(`${quantity}x ${product.name} (${product.heightCm} cm) adicionado!`);
      toggleCart(true);
    }

    function updateCartItemQty(productId, delta) {
      const idx = cart.findIndex(item => item.id === productId);
      if (idx === -1) return;

      cart[idx].qty += delta;
      if (cart[idx].qty <= 0) {
        cart.splice(idx, 1);
      }
      updateCartUI();
    }

    function removeCartItem(productId) {
      cart = cart.filter(item => item.id !== productId);
      updateCartUI();
    }

    // Cálculo de subtotal, regra de frete grátis e total
    function getCartTotals() {
      const subtotal = cart.reduce((acc, item) => acc + item.price * item.qty, 0);
      const totalItems = cart.reduce((acc, item) => acc + item.qty, 0);

      // Frete grátis se subtotal >= R$ 150,00 ou se contém a banqueta de 70cm (que já custa R$ 150,00)
      const hasTallStool = cart.some(item => item.id === 'banqueta-alta-70');
      const qualifiesFreeShipping = subtotal >= FREE_SHIPPING_THRESHOLD || hasTallStool;

      let shippingCost = 0;
      if (subtotal === 0) {
        shippingCost = 0;
      } else if (qualifiesFreeShipping) {
        shippingCost = 0;
      } else if (simulatedShippingRate !== null) {
        shippingCost = simulatedShippingRate;
      } else {
        shippingCost = null; // Aguardando CEP
      }

      const total = subtotal + (shippingCost || 0);
      return { subtotal, totalItems, qualifiesFreeShipping, shippingCost, total };
    }

    function updateCartUI() {
      const { subtotal, totalItems, qualifiesFreeShipping, shippingCost, total } = getCartTotals();

      // Badge do topo
      document.getElementById('cart-badge').textContent = totalItems;
      document.getElementById('drawer-subtitle').textContent =
        totalItems === 1 ? '1 item selecionado' : `${totalItems} itens selecionados`;

      // Barra de progresso Frete Grátis
      const pct = Math.min(100, Math.round((subtotal / FREE_SHIPPING_THRESHOLD) * 100));
      const progressEl = document.getElementById('free-shipping-progress');
      const msgEl = document.getElementById('free-shipping-msg');
      const pctEl = document.getElementById('free-shipping-pct');

      progressEl.style.width = `${pct}%`;
      pctEl.textContent = `${pct}%`;

      if (subtotal === 0) {
        msgEl.textContent = 'Frete Grátis em compras a partir de R$ 150,00';
        msgEl.className = 'text-charcoal';
        progressEl.className = 'h-full bg-wood rounded-full transition-all duration-300';
      } else if (qualifiesFreeShipping) {
        msgEl.textContent = 'Parabéns! Você ganhou FRETE GRÁTIS';
        msgEl.className = 'text-freeGreen font-semibold';
        progressEl.className = 'h-full bg-freeGreen rounded-full transition-all duration-300';
      } else {
        const remaining = FREE_SHIPPING_THRESHOLD - subtotal;
        msgEl.textContent = `Faltam ${formatBRL(remaining)} para ganhar Frete Grátis!`;
        msgEl.className = 'text-charcoal';
        progressEl.className = 'h-full bg-wood rounded-full transition-all duration-300';
      }

      // Renderizar itens no drawer
      const container = document.getElementById('cart-items-container');
      const btnCheckout = document.getElementById('btn-checkout');

      if (cart.length === 0) {
        btnCheckout.disabled = true;
        container.innerHTML = `
          <div class="h-full flex flex-col items-center justify-center text-center py-12 px-4">
            <div class="w-14 h-14 rounded-full bg-sand flex items-center justify-center text-stone-400 mb-3">
              <svg class="w-6 h-6" fill="none" stroke="currentColor" stroke-width="1.8" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" d="M16 11V7a4 4 0 00-8 0v4M5 9h14l1 12H4L5 9z" />
              </svg>
            </div>
            <p class="font-medium text-charcoal">Sua sacola está vazia</p>
            <p class="text-xs text-stone-400 mt-1 max-w-xs">Escolha um de nossos bancos artesanais de madeira maciça para começar.</p>
            <button onclick="toggleCart(false)" class="mt-5 px-5 py-2.5 rounded-full bg-wood text-white text-xs font-medium hover:bg-woodHover transition-colors">
              Explorar Bancos
            </button>
          </div>
        `;
      } else {
        btnCheckout.disabled = false;
        container.innerHTML = cart.map(item => `
          <div class="flex items-center gap-3.5 p-3.5 rounded-2xl bg-sand/60 border border-stone-200/70">
            <div class="w-16 h-16 rounded-xl bg-white border border-stone-100 flex items-center justify-center shrink-0 p-1">
              ${getStoolSvg(item.svgScale, 'cart-' + item.id)}
            </div>
            <div class="flex-1 min-w-0">
              <div class="flex items-start justify-between gap-2">
                <div>
                  <h4 class="text-sm font-semibold text-charcoal truncate">${item.name}</h4>
                  <p class="text-xs text-stone-500">${item.heightCm} cm &times; Ø ${item.diameterCm} cm</p>
                </div>
                <button onclick="removeCartItem('${item.id}')" aria-label="Remover item" class="text-stone-400 hover:text-red-600 transition-colors p-1">
                  <svg class="w-4 h-4" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M19 7l-.867 12.142A2 2 0 0116.138 21H7.862a2 2 0 01-1.995-1.858L5 7m5 4v6m4-6v6m1-10V4a1 1 0 00-1-1h-4a1 1 0 00-1 1v3M4 7h16" />
                  </svg>
                </button>
              </div>

              <div class="flex items-center justify-between mt-2.5">
                <div class="inline-flex items-center bg-white border border-stone-200 rounded-full px-1 py-0.5">
                  <button onclick="updateCartItemQty('${item.id}', -1)" class="w-6 h-6 rounded-full hover:bg-stone-100 text-xs font-semibold">&minus;</button>
                  <span class="w-6 text-center text-xs font-semibold">${item.qty}</span>
                  <button onclick="updateCartItemQty('${item.id}', 1)" class="w-6 h-6 rounded-full hover:bg-stone-100 text-xs font-semibold">+</button>
                </div>
                <span class="text-sm font-semibold text-charcoal">${formatBRL(item.price * item.qty)}</span>
              </div>
            </div>
          </div>
        `).join('');
      }

      // Atualizar valores no rodapé
      document.getElementById('cart-subtotal').textContent = formatBRL(subtotal);

      const shippingEl = document.getElementById('cart-shipping');
      if (subtotal === 0) {
        shippingEl.textContent = '—';
        shippingEl.className = 'text-stone-400';
      } else if (qualifiesFreeShipping) {
        shippingEl.textContent = 'GRÁTIS';
        shippingEl.className = 'px-2 py-0.5 rounded-full bg-freeGreenBg text-freeGreen text-xs font-bold';
      } else if (shippingCost !== null) {
        shippingEl.textContent = formatBRL(shippingCost);
        shippingEl.className = 'font-medium text-charcoal';
      } else {
        shippingEl.textContent = 'Calcule o CEP acima';
        shippingEl.className = 'text-xs text-wood font-medium';
      }

      document.getElementById('cart-total').textContent = formatBRL(total);
    }

    // Máscara de CEP
    function maskCep(input) {
      let v = input.value.replace(/\D/g, '');
      if (v.length > 5) {
        v = v.slice(0, 5) + '-' + v.slice(5, 8);
      }
      input.value = v;
    }

    // Simula cálculo de frete realista conforme prefixo do CEP brasileiro
    function simulateShippingByCep(cepStr) {
      const digits = cepStr.replace(/\D/g, '');
      if (digits.length !== 8) return null;

      const firstDigit = parseInt(digits[0], 10);
      // Valores simulados entre R$ 18,90 e R$ 29,90 conforme região
      if (firstDigit <= 3) {
        return { cost: 18.90, days: '2 a 4 dias úteis', region: 'Sudeste' };
      } else if (firstDigit === 8 || firstDigit === 9) {
        return { cost: 22.90, days: '3 a 6 dias úteis', region: 'Sul' };
      } else if (firstDigit === 7) {
        return { cost: 24.90, days: '4 a 7 dias úteis', region: 'Centro-Oeste' };
      } else {
        return { cost: 29.90, days: '5 a 9 dias úteis', region: 'Norte / Nordeste' };
      }
    }

    // Calculadora de CEP na página principal
    function handlePageCepSubmit(e) {
      e.preventDefault();
      const input = document.getElementById('page-cep-input');
      const resultEl = document.getElementById('page-cep-result');
      const info = simulateShippingByCep(input.value);

      if (!info) {
        resultEl.classList.remove('hidden');
        resultEl.innerHTML = `<span class="text-red-600 text-xs font-medium">Por favor, digite um CEP válido com 8 dígitos.</span>`;
        return;
      }

      currentCep = input.value;
      simulatedShippingRate = info.cost;
      document.getElementById('drawer-cep-input').value = currentCep;
      document.getElementById('drawer-cep-status').textContent = `Entrega estimada em ${info.days} (${info.region}).`;

      resultEl.classList.remove('hidden');
      resultEl.innerHTML = `
        <div class="p-3.5 rounded-2xl bg-sand border border-stone-200/80 space-y-1.5 text-xs">
          <div class="flex justify-between">
            <span class="text-stone-600">Bancos 30 cm ou 50 cm (unitário):</span>
            <span class="font-semibold text-charcoal">${formatBRL(info.cost)} (${info.days})</span>
          </div>
          <div class="flex justify-between">
            <span class="text-stone-600">Banqueta 70 cm ou pedidos &ge; R$ 150:</span>
            <span class="font-bold text-freeGreen">FRETE GRÁTIS (${info.days})</span>
          </div>
        </div>
      `;
      updateCartUI();
    }

    // Calculadora de CEP dentro do Drawer do Carrinho
    function calculateDrawerCep() {
      const input = document.getElementById('drawer-cep-input');
      const statusEl = document.getElementById('drawer-cep-status');
      const info = simulateShippingByCep(input.value);

      if (!info) {
        statusEl.textContent = 'Digite um CEP válido (8 números).';
        statusEl.className = 'text-xs text-red-600 mt-1.5';
        return;
      }

      currentCep = input.value;
      simulatedShippingRate = info.cost;
      document.getElementById('page-cep-input').value = currentCep;

      const { qualifiesFreeShipping } = getCartTotals();
      statusEl.textContent = qualifiesFreeShipping
        ? `CEP ${currentCep}: Frete Grátis aplicado (${info.days}).`
        : `CEP ${currentCep}: ${formatBRL(info.cost)} • Prazo: ${info.days}.`;
      statusEl.className = 'text-xs text-freeGreen font-medium mt-1.5';

      updateCartUI();
    }

    // Abrir / Fechar Drawer
    function toggleCart(open) {
      const overlay = document.getElementById('cart-overlay');
      const drawer = document.getElementById('cart-drawer');

      if (open) {
        overlay.classList.remove('hidden');
        drawer.classList.remove('translate-x-full');
      } else {
        overlay.classList.add('hidden');
        drawer.classList.add('translate-x-full');
      }
    }

    // Checkout Modal
    function openCheckoutModal() {
      if (cart.length === 0) return;

      // Se o cliente não digitou CEP ainda e o pedido não tem frete grátis, atribui um frete padrão estimado ou preenche o CEP já informado
      const { qualifiesFreeShipping } = getCartTotals();
      if (!qualifiesFreeShipping && simulatedShippingRate === null) {
        simulatedShippingRate = 21.90;
      }

      if (currentCep) {
        document.getElementById('chk-cep').value = currentCep;
      }

      document.getElementById('checkout-form-view').classList.remove('hidden');
      document.getElementById('checkout-success-view').classList.add('hidden');
      updateCheckoutSummary();

      toggleCart(false);
      const modal = document.getElementById('checkout-modal');
      modal.classList.remove('hidden');
      modal.classList.add('flex');
    }

    function closeCheckoutModal() {
      const modal = document.getElementById('checkout-modal');
      modal.classList.add('hidden');
      modal.classList.remove('flex');
    }

    function syncCheckoutCep(val) {
      const info = simulateShippingByCep(val);
      if (info) {
        currentCep = val;
        simulatedShippingRate = info.cost;
        updateCheckoutSummary();
      }
    }

    function updateCheckoutSummary() {
      const { subtotal, qualifiesFreeShipping, shippingCost } = getCartTotals();
      const paymentMethod = document.querySelector('input[name="paymentMethod"]:checked')?.value || 'pix';

      const finalShipping = qualifiesFreeShipping ? 0 : (shippingCost || 21.90);
      const pixDiscount = paymentMethod === 'pix' ? subtotal * 0.05 : 0;
      const finalTotal = subtotal + finalShipping - pixDiscount;

      document.getElementById('chk-subtotal').textContent = formatBRL(subtotal);
      document.getElementById('chk-shipping').textContent = finalShipping === 0 ? 'GRÁTIS' : formatBRL(finalShipping);
      document.getElementById('chk-shipping').className = finalShipping === 0 ? 'text-freeGreen font-semibold' : 'text-charcoal';

      const discountRow = document.getElementById('chk-discount-row');
      if (pixDiscount > 0) {
        discountRow.classList.remove('hidden');
        document.getElementById('chk-discount').textContent = `- ${formatBRL(pixDiscount)}`;
      } else {
        discountRow.classList.add('hidden');
      }

      document.getElementById('chk-total').textContent = formatBRL(finalTotal);
    }

    function submitOrder(e) {
      e.preventDefault();
      const name = document.getElementById('chk-name').value.trim();
      const address = document.getElementById('chk-address').value.trim();
      const randomCode = '#AM-' + Math.floor(1000 + Math.random() * 9000);

      document.getElementById('order-code').textContent = randomCode;
      document.getElementById('order-confirmation-text').textContent =
        `Obrigado, ${name}! Seus bancos artesanais de madeira maciça serão preparados e enviados montados para: ${address}.`;

      document.getElementById('checkout-form-view').classList.add('hidden');
      document.getElementById('checkout-success-view').classList.remove('hidden');
    }

    function resetAfterOrder() {
      cart = [];
      updateCartUI();
      closeCheckoutModal();
    }

    // Toast Notification
    let toastTimeout;
    function showToast(msg) {
      const toast = document.getElementById('toast');
      document.getElementById('toast-message').textContent = msg;
      toast.classList.remove('opacity-0', 'translate-y-2');
      clearTimeout(toastTimeout);
      toastTimeout = setTimeout(() => {
        toast.classList.add('opacity-0', 'translate-y-2');
      }, 2800);
    }

    // Inicialização
    window.addEventListener('DOMContentLoaded', () => {
      renderProducts();
      updateCartUI();
    });
  </script>
</body>
</html>
