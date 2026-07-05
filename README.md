<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Grandes Autores de Maceió</title>
  <link rel="stylesheet" href="style.css">
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,700;0,900;1,400&family=Lato:wght@300;400;700&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
</head>
<body>

  <!-- PRELOADER -->
  <div id="preloader" class="preloader">
    <div class="preloader__box">
      <div class="preloader__pen">✒</div>
      <div class="preloader__barra"><div class="preloader__fill"></div></div>
      <p class="preloader__texto">Carregando...</p>
    </div>
  </div>

  <!-- BARRA DE PROGRESSO -->
  <div class="prog-wrap"><div id="progressBar" class="prog-bar"></div></div>

  <!-- HEADER -->
  <header id="header" class="header">
    <div class="header-inner">
      <a href="#inicio" class="logo">✒ Grandes Autores de Maceió</a>
      <span class="header-escola">Escola Prof. Guiomar de Almeida Peixoto</span>
      <button id="menuBtn" class="menu-btn" aria-label="Abrir menu" aria-expanded="false">
        <span></span><span></span><span></span>
      </button>
      <nav id="mainNav" class="nav">
        <a href="#inicio"   class="nav-link" data-sec="inicio">Início</a>
        <a href="#autores"  class="nav-link" data-sec="autores">Autores</a>
        <a href="#obras"    class="nav-link" data-sec="obras">Obras</a>
        <a href="#historia" class="nav-link" data-sec="historia">História</a>
        <a href="#contato"  class="nav-link" data-sec="contato">Contato</a>
      </nav>
    </div>
  </header>

  <main>

    <!-- HERO -->
    <section id="inicio" class="hero">
      <canvas id="heroCanvas" class="hero-canvas"></canvas>
      <div class="hero-content">
        <p class="hero-eyebrow">Literatura · Cultura · Identidade</p>
        <h1 class="hero-title">Os Grandes Autores da<br><em>Literatura Maceioense</em></h1>
        <p class="hero-sub">Maceió é berço de vozes que moldaram a alma brasileira. Da prosa nordestina aos versos que ecoam o Atlântico, a literatura maceioense transcende fronteiras e revela a profundidade de um povo marcado pelo sol, pelo mar e pela resistência.</p>
        <div class="hero-btns">
          <a href="#autores" class="btn btn-gold">Conhecer os Autores</a>
          <a href="#historia" class="btn btn-outline">Nossa História</a>
        </div>
      </div>
      <div class="hero-stats">
        <div class="stat"><strong class="counter" data-target="6">0</strong><span>Autores consagrados</span></div>
        <div class="stat"><strong class="counter" data-target="150" data-suffix="+">0</strong><span>Anos de tradição</span></div>
        <div class="stat"><strong class="counter" data-target="50" data-suffix="+">0</strong><span>Obras de referência</span></div>
      </div>
    </section>

    <!-- AUTORES -->
    <section id="autores" class="secao bg-off">
      <div class="container">
        <div class="secao-header">
          <p class="eyebrow">Vozes que definiram uma era</p>
          <h2 class="secao-titulo">Os Autores</h2>
          <div class="divisor"></div>
        </div>

        <!-- Busca -->
        <div class="busca-wrap">
          <div class="busca-box">
            <i class="fa fa-search"></i>
            <input id="busca" type="text" placeholder="Buscar autor..." aria-label="Buscar autor">
            <button id="btnLimpar" class="btn-limpar" hidden aria-label="Limpar busca"><i class="fa fa-times"></i></button>
          </div>
          <p id="buscaCount" class="busca-count"></p>
        </div>
        <p id="buscaVazio" class="busca-vazio" hidden>Nenhum autor encontrado para "<span id="buscaTermo"></span>"</p>

        <div id="autoresGrid" class="autores-grid">

          <!-- GRACILIANO RAMOS -->
          <article class="autor-card"
            data-name="Graciliano Ramos"
            data-dates="1892 – 1953"
            data-bio="Maior prosador do Nordeste brasileiro, nasceu em Quebrangulo, Alagoas. Prefeito de Palmeira dos Índios e preso político durante o Estado Novo, sua escrita austera e psicológica o consagrou entre os gigantes da língua portuguesa."
            data-obras='["Vidas Secas (1938)","São Bernardo (1934)","Angústia (1936)","Memórias do Cárcere (1953)"]'
            data-curiosidade="Graciliano escrevia com lápis e revisava cada frase dezenas de vezes. Sua prosa seca e precisa era resultado de uma disciplina quase monástica — chegou a destruir manuscritos inteiros por não estarem à altura do que imaginava."
            data-wiki="Graciliano_Ramos"
            data-cor1="#1a2a4a" data-cor2="#2c4a7a" data-fgcor="#F4B400">
            <div class="card-img-wrap">
              <img class="card-img" src="" alt="Graciliano Ramos">
              <span class="card-badge">1892 – 1953</span>
              <button class="card-expand btn-saiba" aria-label="Saiba mais"><i class="fa fa-expand"></i></button>
            </div>
            <div class="card-body">
              <h3 class="card-nome">Graciliano Ramos</h3>
              <p class="card-bio">Maior prosador do Nordeste, sua escrita austera e psicológica retrata a seca, a miséria e a condição humana com precisão cirúrgica.</p>
              <ul class="card-obras">
                <li><i class="fa fa-book-open"></i> Vidas Secas (1938)</li>
                <li><i class="fa fa-book-open"></i> São Bernardo (1934)</li>
                <li><i class="fa fa-book-open"></i> Angústia (1936)</li>
              </ul>
              <button class="btn-saiba btn-ver-mais">Saiba mais <i class="fa fa-arrow-right"></i></button>
            </div>
          </article>

          <!-- JORGE DE LIMA -->
          <article class="autor-card"
            data-name="Jorge de Lima"
            data-dates="1893 – 1953"
            data-bio="Poeta, romancista, médico e pintor nascido em União dos Palmares, AL. Transitou do parnasianismo ao modernismo com maestria única. Seu poema Essa Negra Fulô é um dos mais emblemáticos do Nordeste."
            data-obras='["Invenção de Orfeu (1952)","Essa Negra Fulô (1928)","Calunga (1935)","A Túnica Inconsútil (1938)"]'
            data-curiosidade="Jorge de Lima era um verdadeiro gênio múltiplo: além de poeta e romancista, era médico renomado e pintor surrealista. Sua pintura Invenção de Orfeu inspirou o poema épico de mesmo nome, considerado sua obra-prima."
            data-wiki="Jorge_de_Lima"
            data-cor1="#1D4A2A" data-cor2="#2E7D44" data-fgcor="#F9FAFB">
            <div class="card-img-wrap">
              <img class="card-img" src="" alt="Jorge de Lima">
              <span class="card-badge">1893 – 1953</span>
              <button class="card-expand btn-saiba" aria-label="Saiba mais"><i class="fa fa-expand"></i></button>
            </div>
            <div class="card-body">
              <h3 class="card-nome">Jorge de Lima</h3>
              <p class="card-bio">Poeta, médico e pintor, criou a maior epopeia poética brasileira do século XX com visões místicas e surrealistas do Brasil.</p>
              <ul class="card-obras">
                <li><i class="fa fa-book-open"></i> Invenção de Orfeu (1952)</li>
                <li><i class="fa fa-book-open"></i> Essa Negra Fulô (1928)</li>
                <li><i class="fa fa-book-open"></i> Calunga (1935)</li>
              </ul>
              <button class="btn-saiba btn-ver-mais">Saiba mais <i class="fa fa-arrow-right"></i></button>
            </div>
          </article>

          <!-- AURELIO BUARQUE -->
          <article class="autor-card"
            data-name="Aurélio Buarque de Holanda"
            data-dates="1910 – 1989"
            data-bio="Nascido em Piaçabuçu, AL, foi o maior lexicógrafo da língua portuguesa no Brasil. Seu dicionário tornou-se sinônimo de dicionário no imaginário brasileiro. Também foi crítico literário, tradutor e professor."
            data-obras='["Novo Dicionário da Língua Portuguesa (1975)","Pequeno Dicionário Brasileiro (1938)","Antologia dos Poetas Brasileiros (1956)"]'
            data-curiosidade="O Dicionário Aurélio levou mais de 30 anos para ser concluído. Com mais de 220.000 verbetes e colaboração de centenas de especialistas, tornou-se a obra lexicográfica mais completa da língua portuguesa produzida no Brasil."
            data-wiki="Aur%C3%A9lio_Buarque_de_Holanda"
            data-cor1="#0A3D62" data-cor2="#1a5a8a" data-fgcor="#F4B400">
            <div class="card-img-wrap">
              <img class="card-img" src="" alt="Aurélio Buarque de Holanda">
              <span class="card-badge">1910 – 1989</span>
              <button class="card-expand btn-saiba" aria-label="Saiba mais"><i class="fa fa-expand"></i></button>
            </div>
            <div class="card-body">
              <h3 class="card-nome">Aurélio Buarque de Holanda</h3>
              <p class="card-bio">Maior lexicógrafo brasileiro, criou o dicionário que se tornou sinônimo de língua portuguesa no Brasil inteiro.</p>
              <ul class="card-obras">
                <li><i class="fa fa-book-open"></i> Novo Dicionário (1975)</li>
                <li><i class="fa fa-book-open"></i> Pequeno Dicionário (1938)</li>
              </ul>
              <button class="btn-saiba btn-ver-mais">Saiba mais <i class="fa fa-arrow-right"></i></button>
            </div>
          </article>

          <!-- LEDO IVO -->
          <article class="autor-card"
            data-name="Lêdo Ivo"
            data-dates="1924 – 2012"
            data-bio="Poeta, cronista e romancista nascido em Maceió. Membro da Academia Brasileira de Letras, sua obra poética é marcada pelo lirismo tropical e a tensão entre o cotidiano e o universal."
            data-obras='["Ninho de Cobras (1973)","As Imaginações (1944)","Confissões de um Poeta (1979)","O Ajudante de Mentiroso (1982)"]'
            data-curiosidade="Lêdo Ivo publicou seu primeiro livro de poemas aos 20 anos e foi imediatamente reconhecido pela crítica nacional. Era famoso por suas crônicas sobre Maceió, que misturavam nostalgia, ironia e um amor incondicional pela cidade."
            data-wiki="L%C3%AAdo_Ivo"
            data-cor1="#3A1050" data-cor2="#6A1E8A" data-fgcor="#F9FAFB">
            <div class="card-img-wrap">
              <img class="card-img" src="" alt="Lêdo Ivo">
              <span class="card-badge">1924 – 2012</span>
              <button class="card-expand btn-saiba" aria-label="Saiba mais"><i class="fa fa-expand"></i></button>
            </div>
            <div class="card-body">
              <h3 class="card-nome">Lêdo Ivo</h3>
              <p class="card-bio">Poeta maceioense de lirismo tropical profundo, membro da Academia Brasileira de Letras e um dos maiores poetas do século XX.</p>
              <ul class="card-obras">
                <li><i class="fa fa-book-open"></i> Ninho de Cobras (1973)</li>
                <li><i class="fa fa-book-open"></i> As Imaginações (1944)</li>
              </ul>
              <button class="btn-saiba btn-ver-mais">Saiba mais <i class="fa fa-arrow-right"></i></button>
            </div>
          </article>

          <!-- CLARICE LISPECTOR -->
          <article class="autor-card"
            data-name="Clarice Lispector"
            data-dates="1920 – 1977"
            data-bio="Nascida na Ucrânia, cresceu em Maceió e Recife, sendo profundamente moldada pelo Nordeste. Considerada a maior escritora brasileira do século XX, sua prosa introspectiva e filosófica revolucionou a literatura nacional."
            data-obras='["A Paixão Segundo G.H. (1964)","A Hora da Estrela (1977)","Perto do Coração Selvagem (1943)","Laços de Família (1960)"]'
            data-curiosidade="Clarice escreveu seu primeiro romance, Perto do Coração Selvagem, aos 19 anos. A obra foi comparada a Virginia Woolf pela crítica. Ela guardava memórias vívidas das ruas de Maceió, que aparecem veladas em sua prosa mais introspectiva."
            data-wiki="Clarice_Lispector"
            data-cor1="#4A1060" data-cor2="#8B1A9A" data-fgcor="#F4D03F">
            <div class="card-img-wrap">
              <img class="card-img" src="" alt="Clarice Lispector">
              <span class="card-badge">1920 – 1977</span>
              <button class="card-expand btn-saiba" aria-label="Saiba mais"><i class="fa fa-expand"></i></button>
            </div>
            <div class="card-body">
              <h3 class="card-nome">Clarice Lispector</h3>
              <p class="card-bio">Maior escritora brasileira do século XX, cresceu em Maceió e revolucionou a literatura com sua prosa filosófica e introspectiva.</p>
              <ul class="card-obras">
                <li><i class="fa fa-book-open"></i> A Hora da Estrela (1977)</li>
                <li><i class="fa fa-book-open"></i> Laços de Família (1960)</li>
              </ul>
              <button class="btn-saiba btn-ver-mais">Saiba mais <i class="fa fa-arrow-right"></i></button>
            </div>
          </article>

          <!-- ALTAVINO FLORES -->
          <article class="autor-card"
            data-name="Altavino Flores"
            data-dates="1907 – 1992"
            data-bio="Poeta e jornalista maceioense, figura central na vida cultural de Maceió por décadas. Sua poesia lírica e engajada retratou o cotidiano alagoano e as contradições sociais do Nordeste com sensibilidade única."
            data-obras='["Poemas do Mar (1940)","Canções da Lagoa (1955)","Maceió de Todos os Ventos (1968)"]'
            data-curiosidade="Altavino Flores foi o primeiro presidente da União Brasileira de Escritores em Alagoas. Fundou revistas literárias fundamentais para a formação de uma geração de escritores locais e é considerado o guardião poético da Lagoa Mundaú."
            data-wiki=""
            data-cor1="#7A4A00" data-cor2="#C8930A" data-fgcor="#0A3D62">
            <div class="card-img-wrap">
              <img class="card-img" src="" alt="Altavino Flores">
              <span class="card-badge">1907 – 1992</span>
              <button class="card-expand btn-saiba" aria-label="Saiba mais"><i class="fa fa-expand"></i></button>
            </div>
            <div class="card-body">
              <h3 class="card-nome">Altavino Flores</h3>
              <p class="card-bio">Poeta e jornalista maceioense que celebrou a Lagoa Mundaú e a alma alagoana com lirismo e engajamento social profundos.</p>
              <ul class="card-obras">
                <li><i class="fa fa-book-open"></i> Canções da Lagoa (1955)</li>
                <li><i class="fa fa-book-open"></i> Poemas do Mar (1940)</li>
              </ul>
              <button class="btn-saiba btn-ver-mais">Saiba mais <i class="fa fa-arrow-right"></i></button>
            </div>
          </article>

        </div>
      </div>
    </section>

    <!-- OBRAS -->
    <section id="obras" class="secao bg-white">
      <div class="container">
        <div class="secao-header">
          <p class="eyebrow">Páginas que atravessaram gerações</p>
          <h2 class="secao-titulo">Obras em Destaque</h2>
          <div class="divisor"></div>
        </div>

        <!-- Filtros -->
        <div class="filtros">
          <button class="filtro-btn active" data-filtro="todos">Todos</button>
          <button class="filtro-btn" data-filtro="Graciliano Ramos">Graciliano</button>
          <button class="filtro-btn" data-filtro="Clarice Lispector">Clarice</button>
          <button class="filtro-btn" data-filtro="Jorge de Lima">Jorge de Lima</button>
          <button class="filtro-btn" data-filtro="Lêdo Ivo">Lêdo Ivo</button>
          <button class="filtro-btn" data-filtro="Aurélio Buarque de Holanda">Aurélio</button>
          <button class="filtro-btn" data-filtro="Altavino Flores">Altavino</button>
        </div>

        <div id="obrasGrid" class="obras-grid">

          <div class="obra-card" data-autor="Graciliano Ramos" data-titulo="Vidas Secas" data-icone="☀️" data-cor1="#7B1A1A" data-cor2="#C0392B" data-resumo="A família de Fabiano foge da seca nordestina em busca de sobrevivência. Narrado com austeridade brutal, retrata a miséria e a resistência silenciosa de seres no limite da existência.">
            <div class="obra-capa"></div>
            <div class="obra-info">
              <h3 class="obra-nome">Vidas Secas</h3>
              <p class="obra-autor">Graciliano Ramos · <span class="obra-ano">1938</span></p>
              <p class="obra-resumo"></p>
            </div>
          </div>

          <div class="obra-card" data-autor="Jorge de Lima" data-titulo="Invenção de Orfeu" data-icone="🌊" data-cor1="#0A1F3D" data-cor2="#1A6899" data-resumo="Épica poética em dez cantos que mistura mitologia grega, espiritualidade cristã e surrealismo. Considerada a maior epopeia da língua portuguesa do século XX.">
            <div class="obra-capa"></div>
            <div class="obra-info">
              <h3 class="obra-nome">Invenção de Orfeu</h3>
              <p class="obra-autor">Jorge de Lima · <span class="obra-ano">1952</span></p>
              <p class="obra-resumo"></p>
            </div>
          </div>

          <div class="obra-card" data-autor="Graciliano Ramos" data-titulo="São Bernardo" data-icone="🌿" data-cor1="#1A4A2A" data-cor2="#27AE60" data-resumo="Paulo Honório narra sua própria história, incluindo o amor obsessivo por Madalena que o leva à tragédia. Um estudo magistral da psicologia do poder e da culpa.">
            <div class="obra-capa"></div>
            <div class="obra-info">
              <h3 class="obra-nome">São Bernardo</h3>
              <p class="obra-autor">Graciliano Ramos · <span class="obra-ano">1934</span></p>
              <p class="obra-resumo"></p>
            </div>
          </div>

          <div class="obra-card" data-autor="Clarice Lispector" data-titulo="A Hora da Estrela" data-icone="⭐" data-cor1="#7A5A00" data-cor2="#D4A017" data-resumo="Macabéa, nordestina pobre no Rio de Janeiro, tem sua história contada por um narrador que questiona a própria criação. Um livro sobre invisibilidade e existência.">
            <div class="obra-capa"></div>
            <div class="obra-info">
              <h3 class="obra-nome">A Hora da Estrela</h3>
              <p class="obra-autor">Clarice Lispector · <span class="obra-ano">1977</span></p>
              <p class="obra-resumo"></p>
            </div>
          </div>

          <div class="obra-card" data-autor="Lêdo Ivo" data-titulo="Ninho de Cobras" data-icone="🌙" data-cor1="#3A0D4A" data-cor2="#7D3C98" data-resumo="Romance em Maceió dos anos 1940 onde adolescentes da elite mergulham em ritos noturnos de iniciação e violência. Lêdo Ivo retrata o despertar da sexualidade numa sociedade provinciana.">
            <div class="obra-capa"></div>
            <div class="obra-info">
              <h3 class="obra-nome">Ninho de Cobras</h3>
              <p class="obra-autor">Lêdo Ivo · <span class="obra-ano">1973</span></p>
              <p class="obra-resumo"></p>
            </div>
          </div>

          <div class="obra-card" data-autor="Clarice Lispector" data-titulo="Perto do Coração Selvagem" data-icone="💙" data-cor1="#0D3347" data-cor2="#2471A3" data-resumo="Romance de estreia de Clarice, escrito aos 19 anos. Narra a formação interior de Joana, mulher que recusa convenções sociais em busca de si mesma. Inaugurou o fluxo de consciência no Brasil.">
            <div class="obra-capa"></div>
            <div class="obra-info">
              <h3 class="obra-nome">Perto do Coração Selvagem</h3>
              <p class="obra-autor">Clarice Lispector · <span class="obra-ano">1943</span></p>
              <p class="obra-resumo"></p>
            </div>
          </div>

          <div class="obra-card" data-autor="Graciliano Ramos" data-titulo="Angústia" data-icone="🔥" data-cor1="#3D2010" data-cor2="#884A2A" data-resumo="Luís da Silva narra em delírio sua obsessão e o assassinato do rival Julião Tavares. O livro mais perturbador de Graciliano, com monólogo interior caótico que explode o realismo.">
            <div class="obra-capa"></div>
            <div class="obra-info">
              <h3 class="obra-nome">Angústia</h3>
              <p class="obra-autor">Graciliano Ramos · <span class="obra-ano">1936</span></p>
              <p class="obra-resumo"></p>
            </div>
          </div>

          <div class="obra-card" data-autor="Graciliano Ramos" data-titulo="Memórias do Cárcere" data-icone="✒️" data-cor1="#0D3330" data-cor2="#148F77" data-resumo="Relato autobiográfico da prisão de Graciliano durante o Estado Novo. Com lucidez e amargura, descreve as condições desumanas das cadeias e os companheiros de cativeiro.">
            <div class="obra-capa"></div>
            <div class="obra-info">
              <h3 class="obra-nome">Memórias do Cárcere</h3>
              <p class="obra-autor">Graciliano Ramos · <span class="obra-ano">1953</span></p>
              <p class="obra-resumo"></p>
            </div>
          </div>

          <div class="obra-card" data-autor="Aurélio Buarque de Holanda" data-titulo="Novo Dicionário" data-icone="📚" data-cor1="#1A0A3D" data-cor2="#6C3483" data-resumo="O maior dicionário da língua portuguesa produzido no Brasil, com mais de 220.000 verbetes e 30 anos de pesquisa. O Aurélio tornou-se sinônimo de dicionário no Brasil.">
            <div class="obra-capa"></div>
            <div class="obra-info">
              <h3 class="obra-nome">Novo Dicionário</h3>
              <p class="obra-autor">Aurélio Buarque · <span class="obra-ano">1975</span></p>
              <p class="obra-resumo"></p>
            </div>
          </div>

          <div class="obra-card" data-autor="Altavino Flores" data-titulo="Canções da Lagoa" data-icone="🌅" data-cor1="#7A4A00" data-cor2="#C8930A" data-resumo="Coletânea de poemas que celebra a Lagoa Mundaú com lirismo delicado. Altavino transforma a lagoa em símbolo da alma alagoana, dando voz poética a suas cores, barcos e pescadores.">
            <div class="obra-capa"></div>
            <div class="obra-info">
              <h3 class="obra-nome">Canções da Lagoa</h3>
              <p class="obra-autor">Altavino Flores · <span class="obra-ano">1955</span></p>
              <p class="obra-resumo"></p>
            </div>
          </div>

        </div>
      </div>
    </section>

    <!-- HISTORIA -->
    <section id="historia" class="secao bg-off">
      <div class="container">
        <div class="secao-header">
          <p class="eyebrow">Raízes e identidade</p>
          <h2 class="secao-titulo">A História da Literatura Maceioense</h2>
          <div class="divisor"></div>
        </div>
        <div class="historia-layout">
          <div class="historia-texto">
            <p class="historia-lead">Maceió, a capital alagoana banhada pelo Atlântico e pela Lagoa Mundaú, sempre foi mais do que uma cidade — foi um estado de espírito que transbordou em palavras.</p>
            <p>As raízes da literatura maceioense mergulham no século XIX, quando intelectuais e abolicionistas fundaram os primeiros jornais literários da cidade. Era um Maceió ainda colonial, mas que já pulsava com a inquietação de quem tem histórias urgentes para contar.</p>
            <p>Com o Modernismo brasileiro nos anos 1920, escritores alagoanos protagonizaram a renovação da literatura nacional. Graciliano Ramos levou o sertão para o mundo. Jorge de Lima misturou espiritualidade, surrealismo e negritude numa poesia sem precedentes.</p>
            <p>A infância de Clarice Lispector nas ruas de Maceió deixou marcas indeléveis em sua escrita. A cidade aparece como sombra nas memórias que alimentaram sua prosa revolucionária — o calor, o mar, a pobreza vista pelos olhos de uma criança imigrante.</p>
            <p>Hoje, a literatura maceioense vive um renascimento. Novos autores exploram identidade racial, memória afroindígena e urbanidade periférica. Festivais literários e saraus nas praias mantêm viva a chama acesa por Graciliano e seus contemporâneos.</p>
          </div>
          <aside class="timeline-wrap">
            <h3 class="timeline-titulo">Linha do Tempo</h3>
            <ol class="timeline">
              <li class="tl-item"><span class="tl-ano">1819</span><div class="tl-info"><strong>Maceió torna-se capital</strong><p>Início da vida intelectual organizada na cidade.</p></div></li>
              <li class="tl-item"><span class="tl-ano">1881</span><div class="tl-info"><strong>Primeira Revista Literária</strong><p>Surgem os primeiros periódicos dedicados à literatura local.</p></div></li>
              <li class="tl-item"><span class="tl-ano">1919</span><div class="tl-info"><strong>Academia Alagoana de Letras</strong><p>Fundação do principal órgão de promoção literária em Alagoas.</p></div></li>
              <li class="tl-item"><span class="tl-ano">1934</span><div class="tl-info"><strong>São Bernardo</strong><p>Graciliano define o romance nordestino moderno.</p></div></li>
              <li class="tl-item"><span class="tl-ano">1938</span><div class="tl-info"><strong>Vidas Secas</strong><p>Obra máxima do realismo nordestino, traduzida para dezenas de idiomas.</p></div></li>
              <li class="tl-item"><span class="tl-ano">1952</span><div class="tl-info"><strong>Invenção de Orfeu</strong><p>Jorge de Lima publica sua epopeia, obra-prima da poesia brasileira.</p></div></li>
              <li class="tl-item"><span class="tl-ano">Hoje</span><div class="tl-info"><strong>Novos Saraus</strong><p>Nova geração redefine a literatura alagoana em festivais e praias.</p></div></li>
            </ol>
          </aside>
        </div>
      </div>
    </section>

    <!-- CITACAO -->
    <section class="citacao-secao">
      <div class="container">
        <div id="carouselWrap" class="carousel-wrap">
          <button id="carPrev" class="car-btn" aria-label="Anterior"><i class="fa fa-chevron-left"></i></button>
          <div class="carousel-view">
            <div id="carTrack" class="car-track">
              <div class="car-slide">
                <blockquote>
                  <p>"Escrever é uma maneira de existir. E existir, em Alagoas, é carregar o peso do sol, a leveza das lagoas e a dor que o silêncio do sertão nunca conseguiu esconder."</p>
                  <footer>— Inspirado em Graciliano Ramos</footer>
                </blockquote>
              </div>
              <div class="car-slide">
                <blockquote>
                  <p>"A poesia não é ornamento da vida. É a própria vida se reconhecendo no espelho da linguagem, entre o mar e a lagoa de Maceió."</p>
                  <footer>— Inspirado em Lêdo Ivo</footer>
                </blockquote>
              </div>
              <div class="car-slide">
                <blockquote>
                  <p>"Escrever é uma maldição que salva. A frase já estava em mim — eu é que precisava de coragem para deixá-la sair."</p>
                  <footer>— Inspirado em Clarice Lispector</footer>
                </blockquote>
              </div>
            </div>
          </div>
          <button id="carNext" class="car-btn" aria-label="Próximo"><i class="fa fa-chevron-right"></i></button>
        </div>
        <div id="carDots" class="car-dots"></div>
      </div>
    </section>

  </main>

  <!-- MODAL -->
  <div id="modal" class="modal" hidden>
    <div id="modalOverlay" class="modal-overlay"></div>
    <div class="modal-box">
      <button id="modalFechar" class="modal-fechar" aria-label="Fechar"><i class="fa fa-times"></i></button>
      <div class="modal-layout">
        <div class="modal-col-img">
          <img id="modalImg" src="" alt="">
          <p id="modalDatas" class="modal-datas"></p>
        </div>
        <div class="modal-col-info">
          <h2 id="modalNome" class="modal-nome"></h2>
          <p id="modalBio" class="modal-bio"></p>
          <div class="modal-curiosidade">
            <h4><i class="fa fa-lightbulb"></i> Curiosidade</h4>
            <p id="modalCuriosidade"></p>
          </div>
          <h4 class="modal-obras-titulo">Principais Obras</h4>
          <ul id="modalObras" class="modal-obras"></ul>
        </div>
      </div>
    </div>
  </div>


    <!-- SECAO ESCOLA E ALUNOS -->
    <section class="escola-secao">
      <div class="container">
        <div class="escola-grid">
          <div class="escola-info">
            <p class="eyebrow">Projeto Escolar</p>
            <h2 class="escola-titulo">Escola Estadual Prof.<br>Guiomar de Almeida Peixoto</h2>
            <p class="escola-turma"><i class="fa fa-users"></i> Turma: <strong>3° ADM</strong></p>
            <a href="mailto:ee.guiomaralmeida@educ.al.gov.br" class="escola-email">
              <i class="fa fa-envelope"></i> ee.guiomaralmeida@educ.al.gov.br
            </a>
            <a href="https://www.instagram.com/escolaestadualgap?igsh=aXBlcG9hd3FhNDNk" target="_blank" rel="noopener" class="escola-insta">
              <i class="fa-brands fa-instagram"></i> @escolaestadualgap
            </a>
          </div>
          <div class="alunos-wrap">
            <h3 class="alunos-titulo"><i class="fa fa-star"></i> Alunos Participantes</h3>
            <ul class="alunos-lista">
              <li><span class="aluno-num">01</span>Tharlysson Renato</li>
              <li><span class="aluno-num">02</span>Endrel Rafael</li>
              <li><span class="aluno-num">03</span>Yasmin</li>
              <li><span class="aluno-num">04</span>Diogo</li>
              <li><span class="aluno-num">05</span>Iuri</li>
              <li><span class="aluno-num">06</span>Olivia</li>
            </ul>
          </div>
        </div>
      </div>
    </section>

  <!-- RODAPE -->
  <footer id="contato" class="rodape">
    <div class="container">
      <div class="rodape-grid">
        <div class="rodape-col">
          <p class="rodape-logo">✒ Grandes Autores de Maceió</p>
          <p class="rodape-sobre">Projeto escolar da <strong>Escola Estadual Prof. Guiomar de Almeida Peixoto</strong> — Turma <strong>3° ADM</strong>. Um tributo à riqueza literária de Maceió e Alagoas.</p>
          <div class="rodape-social">
            <a href="https://www.instagram.com/escolaestadualgap?igsh=aXBlcG9hd3FhNDNk" target="_blank" rel="noopener" aria-label="Instagram"><i class="fa-brands fa-instagram"></i></a>
            <a href="#" aria-label="Facebook"><i class="fa-brands fa-facebook-f"></i></a>
            <a href="#" aria-label="Twitter"><i class="fa-brands fa-x-twitter"></i></a>
            <a href="#" aria-label="YouTube"><i class="fa-brands fa-youtube"></i></a>
          </div>
        </div>
        <div class="rodape-col">
          <h4>Navegação</h4>
          <ul>
            <li><a href="#inicio">Início</a></li>
            <li><a href="#autores">Autores</a></li>
            <li><a href="#obras">Obras</a></li>
            <li><a href="#historia">História</a></li>
          </ul>
        </div>
        <div class="rodape-col">
          <h4>Contato</h4>
          <address>
            <p><i class="fa fa-envelope"></i> <a href="mailto:ee.guiomaralmeida@educ.al.gov.br">ee.guiomaralmeida@educ.al.gov.br</a></p>
            <p><i class="fa fa-location-dot"></i> Maceió, Alagoas — Brasil</p>
            <p><i class="fa fa-graduation-cap"></i> Escola Est. Prof. Guiomar de Almeida Peixoto</p>
          </address>
        </div>
      </div>
    </div>
    <div class="rodape-bottom">
      <p>© <span id="anoAtual"></span> Grandes Autores de Maceió · Escola Est. Prof. Guiomar de Almeida Peixoto · Turma 3° ADM · Todos os direitos reservados.</p>
    </div>
  </footer>

  <!-- BOTAO TOPO -->
  <button id="btnTopo" class="btn-topo" hidden aria-label="Voltar ao topo"><i class="fa fa-chevron-up"></i></button>

  <!-- TOAST -->
  <div id="toast" class="toast"></div>

  <script src="script.js"></script>
</body>
</html>
