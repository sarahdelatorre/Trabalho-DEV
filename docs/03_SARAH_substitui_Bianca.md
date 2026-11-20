# Guia 3 de 6 · Página da Sarah (substitui a da sarah)

Passo a passo para sair do estado inicial de `sarah.html` e chegar à v3 (tema a definir (azul, como o modelo da sarah, ou rosa)). Responsável sugerido pela página: **Sarah**. Faça um marco por vez e dê commit ao fim de cada um. **Esta frente começa pela substituição da página da sarah (T003 e seus passos pequenos, marco M1)** e só depois segue para a v3.

> Os IDs (T001...) são os mesmos da planilha `Controle_de_Tarefas_Grupo_1C.xlsx`. Marque o status por lá. Responsáveis e prazos marcados como "sugerido" ou "A definir" podem ser ajustados pelo grupo.

**57 tarefas** nesta frente.

## Marcos desta frente

| Marco | Nome | Tarefas | O que está pronto |
|---|---|---|---|
| M1 | V1 no repositório | 13 | O HTML original está no GitHub, cada integrante tem o repositório no computador e cada página tem uma branch. |
| M2 | Bootstrap e CSS ligados | 9 | Cada página carrega Bootstrap, estilo.css e o tema de cor. Visual ainda simples, mas a base está pronta. |
| M3 | Casca padronizada | 8 | Navbar, faixa de abertura (hero) com botões e rodapé iguais nas 5 páginas. |
| M4 | Seções em grade | 11 | O conteúdo está organizado em seções com container, row e col (Bootstrap) e em cartões. |
| M5 | Estilo final | 8 | Cores do tema, cartões com borda arredondada e sombra, efeito hover/foco e barra colorida nos títulos. |
| M6 | Revisão e entrega v3 | 8 | HTML validado, nada perdido, testado em celular/tablet/PC, Pull Request aprovado e versão v3 marcada. |

## Como estudar

- "PDF" é o material *O Cardápio do Navegador: CSS do Seletor ao Bootstrap* (capítulos indicados em cada tarefa).
- "Fora do PDF" são páginas oficiais; abra só a parte do assunto da tarefa, não precisa ler o site inteiro.

## M1 · V1 no repositório

*O HTML original está no GitHub, cada integrante tem o repositório no computador e cada página tem uma branch.*

#### T107 · Criar a branch pagina-sarah
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T002

- **O que fazer:** No terminal, dentro da pasta do repositório: "git switch -c pagina-sarah". A branch é uma cópia de trabalho só sua; a main fica protegida.
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2); [GitHub Docs: Hello World](https://docs.github.com/en/get-started/start-your-journey/hello-world)
- **Pronto quando:** "git branch" mostra pagina-sarah com um asterisco.

#### T108 · Receber o conteúdo da Sarah (texto e fotos) e guardar numa pasta de apoio
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T107 · *passo de T003*

- **O que fazer:** Peça para a Sarah mandar o texto e as fotos. Guarde tudo numa pasta fora do repositório até conferir.
- **Pronto quando:** Todo o material está na sua pasta.

#### T109 · Criar images/sarah/ e copiar as fotos para lá
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T108 · *passo de T003*

- **O que fazer:** Dentro de images/ crie a pasta sarah e coloque as fotos. Use nomes sem espaço nem acento (ex.: foto1.jpg): evita erro de caminho.
- **Estudar no PDF:** Cap. 1.2 (caminhos de arquivos)
- **Pronto quando:** Fotos em images/sarah/.

#### T110 · Criar sarah.html a partir do texto da Sarah
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~30 min · **Depois de:** T109 · *passo de T003*

- **O que fazer:** Copie o sarah.html como molde de estrutura (h1, parágrafos, listas, imagens) e troque o conteúdo pelo da Sarah. Salve como sarah.html em files/.
- **Pronto quando:** sarah.html criado.

#### T111 · Ajustar os caminhos das imagens para ../images/sarah/…
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T110 · *passo de T003*

- **O que fazer:** Cada <img src="…"> precisa apontar para ../images/sarah/nome-da-foto. Abra no navegador e confira se todas aparecem.
- **Estudar no PDF:** Cap. 1.2 (caminhos de arquivos)
- **Pronto quando:** Nenhuma imagem quebrada.

#### T112 · Trocar o ícone da aba (favicon) e o <title>
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T111 · *passo de T003*

- **O que fazer:** No <head>, ajuste <link rel="icon" href="../icons/Sarah_favicon.png"> (coloque o arquivo em icons/) e o <title> com o nome da Sarah.
- **Pronto quando:** Aba do navegador mostra o nome e o ícone certos.

#### T113 · Trocar sarah.html por sarah.html na home e nas outras páginas
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T112 · *passo de T003*

- **O que fazer:** Procure "sarah.html" em todos os arquivos (Ctrl+Shift+F no editor) e troque por "sarah.html".
- **Pronto quando:** Busca por "sarah.html" não retorna nada.

#### T114 · Trocar o nome "sarah" por "Sarah" na navbar e no rodapé
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T113 · *passo de T003*

- **O que fazer:** Nos blocos modelo/navbar.html e modelo/rodape.html (e nas páginas que já os usam) troque o rótulo do link.
- **Pronto quando:** Navbar e rodapé mostram "Sarah".

#### T115 · Mover sarah.html e images/sarah/ para fora do projeto
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T114 · *passo de T003*

- **O que fazer:** Use "git rm" (ou "git mv" para uma pasta arquivo/). O histórico do Git guarda os arquivos antigos, então nada se perde.
- **Estudar no PDF:** Cap. 1.2 (caminhos de arquivos)
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Pasta e arquivo da sarah fora de files/ e images/.

#### T116 · Testar: nenhuma página aponta mais para a sarah
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T115 · *passo de T003*

- **O que fazer:** Procure "sarah" no projeto inteiro e abra as 5 páginas clicando nos links.
- **Pronto quando:** Zero ocorrências e nenhum link quebrado.

#### T117 · Commit e Pull Request "Substituir página da sarah pela página da Sarah"
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T116 · *passo de T003*

- **O que fazer:** git add . e git commit -m "Substitui página da sarah pela da Sarah"; depois abra o Pull Request pedindo revisão.
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Pull Request aberto.

#### T118 · Abrir sarah.html no navegador e listar o que aparece
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T117

- **O que fazer:** Abra o arquivo e escreva uma lista curta: título, textos, fotos, listas e links que você vê. Isso vira seu mapa para não perder nada.
- **Estudar no PDF:** Cap. 1.1 (HTML descreve o conteúdo)
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Lista escrita (pode ser no bloco de notas).

#### T119 · Contar as imagens e os links de sarah.html
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T118

- **O que fazer:** Abra o arquivo no editor, use Ctrl+F e procure "<img" e "<a ". Anote os dois números. No fim, a V3 tem de ter os mesmos.
- **Pronto quando:** Números anotados.

## M2 · Bootstrap e CSS ligados

*Cada página carrega Bootstrap, estilo.css e o tema de cor. Visual ainda simples, mas a base está pronta.*

#### T120 · Conferir lang="pt-br" e meta charset UTF-8
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T119

- **O que fazer:** Confirme que a primeira linha tem <html lang="pt-br"> e o <head> tem <meta charset="UTF-8">. O charset garante que acentos apareçam certos.
- **Estudar no PDF:** Cap. 8.1
- **Pronto quando:** As duas linhas estão presentes.

#### T121 · Conferir a meta viewport
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T120

- **O que fazer:** Confirme a linha <meta name="viewport" content="width=device-width, initial-scale=1.0"> no <head>. Ela faz o celular usar a largura real da tela.
- **Estudar no PDF:** Cap. 7.1
- **Pronto quando:** A linha existe no <head>.

#### T122 · Ligar o Bootstrap 5.3.9 no <head> de sarah.html
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T121

- **O que fazer:** Copie do modelo/head.html (ou do site oficial) a linha <link ... bootstrap.min.css>. Sem internet o Bootstrap não carrega.
- **Estudar no PDF:** Cap. 8.1 (instalar pelo CDN)
- **Estudar fora do PDF:** [Bootstrap 5.3: Get started](https://getbootstrap.com/docs/5.3/getting-started/introduction/)
- **Pronto quando:** Ao recarregar, a fonte e os espaços do texto mudam um pouco.

#### T123 · Ligar ../css/estilo.css depois do Bootstrap
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T122

- **O que fazer:** Acrescente <link rel="stylesheet" href="../css/estilo.css"> logo abaixo da linha do Bootstrap. A ordem importa: quem vem por último vence em caso de empate.
- **Estudar no PDF:** Cap. 1.2 (CSS externo) e 1.4 (cascata)
- **Pronto quando:** Fonte do body mudou para Segoe UI/Arial.

#### T124 · Ligar ../css/tema-sarah.css depois do estilo.css
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T123

- **O que fazer:** Acrescente <link rel="stylesheet" href="../css/tema-sarah.css"> como terceira linha de CSS.
- **Estudar no PDF:** Cap. 1.2 e 1.4
- **Pronto quando:** Linha adicionada.

#### T125 · Colocar class="tema-sarah" na tag <body>
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T124

- **O que fazer:** Troque <body> por <body class="tema-sarah">. O CSS do tema só age em páginas que tenham essa classe.
- **Estudar no PDF:** Cap. 1.3 (seletor de classe)
- **Pronto quando:** Fundo da página na cor do tema (a definir (azul, como o modelo da sarah, ou rosa)).

#### T126 · Testar: recarregar e ver se o fundo e a fonte mudaram
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T125

- **O que fazer:** Abra com F5. Se nada mudou, abra o DevTools (F12), aba Console/Network, e veja qual arquivo deu erro 404 (caminho errado).
- **Estudar fora do PDF:** [Chrome DevTools: device mode](https://developer.chrome.com/docs/devtools/device-mode)
- **Pronto quando:** Fundo e fonte corretos, sem erro 404.

#### T127 · Commit do marco M2
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T126

- **O que fazer:** git add sarah.html e git commit -m "M2 Sarah: Bootstrap e CSS ligados". Um commit por marco facilita desfazer se algo der errado.
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Commit criado.

#### T128 · Decidir a cor da Sarah (azul do modelo ou rosa)
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T127

- **O que fazer:** Converse com o grupo: a sarah era azul (#1F5FBF) e a cor rosa foi pedida para a Sarah. Escolha uma, anote no README e copie a paleta correspondente para tema-sarah.css.
- **Estudar no PDF:** Cap. 2.1
- **Estudar fora do PDF:** [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/)
- **Pronto quando:** Cor decidida e registrada.

## M3 · Casca padronizada

*Navbar, faixa de abertura (hero) com botões e rodapé iguais nas 5 páginas.*

#### T129 · Colar a navbar no início do <body> de sarah.html
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T128

- **O que fazer:** Copie o bloco de modelo/navbar.html e cole logo depois de <body>. A navbar é a mesma em todas as páginas.
- **Estudar no PDF:** Cap. 4.2
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Barra de navegação aparece no topo.

#### T130 · Marcar o link da própria página como ativo
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T129

- **O que fazer:** No bloco da navbar, no link desta página, escreva class="ativo" aria-current="page". A aba ativa fica branca e mostra onde você está.
- **Estudar no PDF:** Cap. 6.1 (estado visual)
- **Pronto quando:** Só um link está destacado.

#### T131 · Testar os 5 links da navbar
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T130

- **O que fazer:** Clique em cada link. Todos devem abrir a página certa, na mesma aba.
- **Pronto quando:** 5 links funcionando.

#### T132 · Criar o hero com o título "título da página (como no <title>)"
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T131

- **O que fazer:** Depois da navbar, crie <section class="hero"><div class="container"><h1>…</h1></div></section> e mova para lá o título atual da página.
- **Estudar no PDF:** Cap. 8.2 (container) e 1.3
- **Estudar fora do PDF:** [Bootstrap 5.3: Grid system](https://getbootstrap.com/docs/5.3/layout/grid/)
- **Pronto quando:** Faixa colorida com o título dentro.

#### T133 · Montar o rótulo "TÓPICOS DA PÁGINA" e os botões de atalho
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~25 min · **Depois de:** T132

- **O que fazer:** Dentro do hero: <h2 class="rotulo">TÓPICOS DA PÁGINA</h2> e uma <ul class="atalhos"> com um <li><a class="btn btn-primary" href="..."> por botão: Voltar à página inicial, Sobre mim, Curiosidades, Lugares que já visitei e Lugares que quero visitar (ajuste aos títulos reais). Os links internos usam #id da seção.
- **Estudar no PDF:** Cap. 8.3 (btn btn-primary)
- **Estudar fora do PDF:** [Bootstrap 5.3: Get started](https://getbootstrap.com/docs/5.3/getting-started/introduction/)
- **Pronto quando:** Fileira de botões brancos abaixo do título.

#### T134 · Colar o rodapé antes de </body>
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T133

- **O que fazer:** Copie modelo/rodape.html e cole logo antes de </body>, depois de </main> (que será criado no M4).
- **Estudar no PDF:** Cap. 8.2
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Rodapé aparece no fim da página.

#### T135 · Testar o link "Volte ao topo da página!"
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T134

- **O que fazer:** Clique no link do rodapé: a página deve subir até a navbar (o id="topo" está no <header>).
- **Pronto quando:** Página sobe até o topo.

#### T136 · Commit do marco M3
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T135

- **O que fazer:** git add sarah.html e git commit -m "M3 Sarah: navbar, hero e rodapé".
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Commit criado.

## M4 · Seções em grade

*O conteúdo está organizado em seções com container, row e col (Bootstrap) e em cartões.*

#### T137 · Envolver todo o conteúdo entre o hero e o rodapé com <main>
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T136

- **O que fazer:** <main> marca o conteúdo principal da página. Ele fica entre </header> e <footer>.
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** <main> abre depois do hero e fecha antes do rodapé.

#### T138 · Remover as <hr> (linhas horizontais) do conteúdo
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T137

- **O que fazer:** As linhas separavam as partes no HTML antigo. Com seções coloridas elas não são mais necessárias; apague as tags <hr>.
- **Estudar no PDF:** Cap. 3.1
- **Pronto quando:** Nenhuma <hr> no arquivo.

#### T139 · Mapear as seções da página da Sarah nas 4 seções padrão
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T138

- **O que fazer:** Leia o conteúdo e decida onde cada parte entra: Sobre mim, Curiosidades, Lugares que já visitei, Lugares que quero visitar. Partes que não cabem podem virar uma seção extra (como "Fotos").
- **Estudar no PDF:** Cap. 8.2
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Tabela "parte do texto → seção" escrita.

#### T140 · Colocar "Lugares que já visitei" antes de "Lugares que quero visitar"
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T139

- **O que fazer:** A ordem padrão das 5 páginas é: visitei primeiro, quero visitar depois. Reordene os blocos no HTML (recorte e cole a <section> inteira).
- **Pronto quando:** Ordem igual à das outras páginas.

#### T141 · Transformar o índice de tópicos (se existir) nos botões do hero
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T140

- **O que fazer:** No modelo da sarah o índice "TÓPICOS DA PÁGINA" era uma lista de âncoras. Cada item vira um botão do hero e cada âncora precisa de um id na seção correspondente (id="sobremim", "curiosidades", "visitei", "visitar").
- **Estudar no PDF:** Cap. 8.3
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Cada botão leva à seção certa.

#### T142 · Seção "Sobre mim": texto em col-12 col-lg-7 e fotos em col-12 col-lg-5
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~25 min · **Depois de:** T141

- **O que fazer:** Dentro de <section id="sobremim">: <div class="row g-3"> com a coluna do texto (7 partes) e a coluna das fotos (5 partes). A partir de 992 px ficam lado a lado.
- **Estudar no PDF:** Cap. 8.2 (colunas somam 12)
- **Estudar fora do PDF:** [Bootstrap 5.3: Grid system](https://getbootstrap.com/docs/5.3/layout/grid/)
- **Pronto quando:** Texto à esquerda e fotos à direita no PC; empilhados no celular.

#### T143 · Fotos do "Sobre mim" em linhas de duas colunas (col-6)
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T142

- **O que fazer:** Dentro da coluna das fotos faça outra <div class="row g-3"> e coloque cada foto em <div class="col-6">.
- **Estudar no PDF:** Cap. 8.2
- **Pronto quando:** Fotos em 2 por linha.

#### T144 · Legenda entre grupos de fotos em linha própria (col-12)
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T143

- **O que fazer:** Se houver uma frase entre dois grupos de fotos (no modelo era "Essa sou eu atualmente."), coloque-a em <div class="col-12"><p class="legenda">…</p></div>.
- **Estudar no PDF:** Cap. 8.2
- **Pronto quando:** Frase ocupa a linha inteira entre os grupos.

#### T145 · Curiosidades: um cartão por item da lista
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~25 min · **Depois de:** T144

- **O que fazer:** Troque a lista por <ul class="lista-cartoes row g-3"> e cada <li> por <li class="col-12 col-md-6"><div class="cartao">…</div></li>. Listas dentro de itens (artistas, músicas) ficam dentro do cartão.
- **Estudar no PDF:** Cap. 8.2 e 3.1
- **Pronto quando:** Itens em cartões, 2 por linha no tablet.

#### T146 · Galerias de lugares: foto com link em col-6 col-md-4 col-lg-3
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~25 min · **Depois de:** T145

- **O que fazer:** Cada foto que leva a uma página (ex.: Wikipédia) vira <div class="col-6 col-md-4 col-lg-3"><a class="foto" href="…"><img …></a></div>. Mantenha o texto de introdução acima da galeria.
- **Estudar no PDF:** Cap. 8.2
- **Estudar fora do PDF:** [Bootstrap 5.3: Grid system](https://getbootstrap.com/docs/5.3/layout/grid/)
- **Pronto quando:** Galeria em 2, 3 e 4 colunas conforme a tela.

#### T147 · Escrever um texto alternativo (alt) descritivo em cada foto
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T146

- **O que fazer:** Descreva em poucas palavras o que a foto mostra ("Praia Grande", "Foto de Sarah 1"). Evite deixar o caminho do arquivo como alt.
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Nenhum alt vazio ou igual ao nome do arquivo.

## M5 · Estilo final

*Cores do tema, cartões com borda arredondada e sombra, efeito hover/foco e barra colorida nos títulos.*

#### T148 · Trocar width e height das imagens por CSS
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T147

- **O que fazer:** Apague os atributos width="…" e height="…" das <img>. Quem controla o tamanho agora é o CSS (img { max-width: 100%; height: auto; }) e as colunas.
- **Estudar no PDF:** Cap. 7.3
- **Estudar fora do PDF:** [PDF F17: Responsive web design basics (web.dev)](https://web.dev/articles/responsive-web-design-basics)
- **Pronto quando:** Nenhuma <img> com width/height.

#### T149 · Aplicar class="titulo" em todos os h2 das seções
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T148

- **O que fazer:** Acrescente class="titulo" nos h2. A barra colorida antes do título vem do CSS (::before).
- **Estudar no PDF:** Cap. 6.3
- **Pronto quando:** Barra colorida antes de cada título.

#### T150 · Aplicar class="cartao" nas caixas de conteúdo
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T149

- **O que fazer:** Coloque <div class="cartao"> em volta de cada item que virou cartão (curiosidades, lugares, integrantes).
- **Estudar no PDF:** Cap. 3.4
- **Pronto quando:** Cartões com canto redondo e sombra.

#### T151 · Aplicar class="foto" nas imagens das galerias
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T150

- **O que fazer:** Use <figure class="foto"><img …></figure> para foto sem link e <a class="foto" href="…"><img …></a> para foto com link.
- **Estudar no PDF:** Cap. 3.4 e 6.1
- **Pronto quando:** Fotos arredondadas, com sombra e hover.

#### T152 · Alternar o fundo das seções com class="secao secao-alt"
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T151

- **O que fazer:** Use <section class="secao"> e, de duas em duas seções, <section class="secao secao-alt"> para alternar o fundo.
- **Estudar no PDF:** Cap. 1.4 (várias classes no mesmo elemento)
- **Pronto quando:** Fundos alternando.

#### T153 · Testar hover e foco pelo teclado
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T152

- **O que fazer:** Passe o mouse nos cartões e fotos e depois aperte Tab várias vezes. Todo link deve mostrar um destaque ao receber foco.
- **Estudar no PDF:** Cap. 6.1
- **Estudar fora do PDF:** [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/)
- **Pronto quando:** Hover e foco visíveis.

#### T154 · Conferir as cores do tema na página inteira
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T153

- **O que fazer:** Olhe navbar, hero, títulos, links e rodapé: tudo na cor a definir (azul, como o modelo da sarah, ou rosa) e legível.
- **Estudar no PDF:** Cap. 2.1
- **Estudar fora do PDF:** [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/)
- **Pronto quando:** Visual coerente com o tema.

#### T155 · Commit do marco M5
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T154

- **O que fazer:** git add . e git commit -m "M5 Sarah: estilo final".
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Commit criado.

## M6 · Revisão e entrega v3

*HTML validado, nada perdido, testado em celular/tablet/PC, Pull Request aprovado e versão v3 marcada.*

#### T156 · Validar sarah.html no validador HTML do W3C
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~30 min · **Depois de:** T155

- **O que fazer:** Abra o validador, escolha "Validate by File Upload" ou "Direct Input" e envie o arquivo. Corrija cada erro listado (tag aberta sem fechar, atributo errado).
- **Estudar fora do PDF:** [Validador de HTML do W3C](https://validator.w3.org/); [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Sem erros (avisos podem ficar).

#### T157 · Comparar a contagem de imagens e links com a do M1
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T156

- **O que fazer:** Repita o Ctrl+F do M1. Os números do conteúdo precisam bater (navbar e rodapé acrescentam links novos: confira só os do conteúdo).
- **Pronto quando:** Números batem.

#### T158 · Ler texto novo x texto original lado a lado
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T157

- **O que fazer:** Abra o HTML do M1 (git show) e a página nova e confira se todos os textos continuam lá, com as mesmas palavras.
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Nenhum texto perdido ou alterado.

#### T159 · Testar em 360, 768 e 1200 px no DevTools
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T158

- **O que fazer:** No Chrome aperte F12 e clique no ícone de celular/tablet. Teste as 3 larguras. Nenhuma rolagem horizontal pode aparecer.
- **Estudar no PDF:** Cap. 7.2 e 8.2 (breakpoints md = 768 px)
- **Estudar fora do PDF:** [Chrome DevTools: device mode](https://developer.chrome.com/docs/devtools/device-mode); [Bootstrap 5.3: Grid system](https://getbootstrap.com/docs/5.3/layout/grid/)
- **Pronto quando:** 3 larguras sem rolagem horizontal e com layout certo.

#### T160 · Clicar em todos os links externos da página
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T159

- **O que fazer:** Abra cada link externo numa nova aba e anote os que não abrem. Entregue a lista para a tarefa "Consolidar os links externos".
- **Pronto quando:** Lista de links quebrados (pode ser vazia).

#### T161 · Abrir o Pull Request da branch
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T160

- **O que fazer:** git push -u origin pagina-sarah; no GitHub clique em "Compare & pull request", descreva o que mudou e peça revisão de outra pessoa.
- **Estudar fora do PDF:** [GitHub Docs: Creating a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request); [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Pull Request aberto com revisor.

#### T162 · Revisar o Pull Request de outra pessoa (checklist)
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T161

- **O que fazer:** Quem revisa abre a aba "Files changed", segue o checklist e comenta ou aprova. Só depois o autor faz o merge.
- **Estudar fora do PDF:** [GitHub Docs: Creating a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)
- **Pronto quando:** PR aprovado por alguém que não é o autor.

#### T163 · Fazer o merge na main e atualizar o status no Excel
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T162

- **O que fazer:** Com o PR aprovado, clique em "Merge pull request". Depois marque as tarefas da página como Concluída nesta planilha.
- **Estudar fora do PDF:** [GitHub Docs: Creating a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)
- **Pronto quando:** Página na main e status atualizado.

## Fontes desta frente

- [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2) (aberta em 17/11/2026)
- [GitHub Docs: Hello World](https://docs.github.com/en/get-started/start-your-journey/hello-world) (aberta em 17/11/2026)
- [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements) (aberta em 17/11/2026)
- [Bootstrap 5.3: Get started](https://getbootstrap.com/docs/5.3/getting-started/introduction/) (aberta em 17/11/2026)
- [Chrome DevTools: device mode](https://developer.chrome.com/docs/devtools/device-mode) (aberta em 17/11/2026)
- [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/) (aberta em 17/11/2026)
- [Bootstrap 5.3: Grid system](https://getbootstrap.com/docs/5.3/layout/grid/) (aberta em 17/11/2026)
- PDF F17: [Responsive web design basics (web.dev)](https://web.dev/articles/responsive-web-design-basics) (citada na lista de fontes do PDF; não reaberta nesta sessão)
- [Validador de HTML do W3C](https://validator.w3.org/) (aberta em 17/11/2026)
- [GitHub Docs: Creating a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) (aberta em 17/11/2026)
