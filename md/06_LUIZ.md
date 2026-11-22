# Guia 6 de 6 · Página do Luiz

Passo a passo para sair do estado inicial de `luiz.html` e chegar à v3 (tema vermelho). Responsável sugerido pela página: **Luiz**. Faça um marco por vez e dê commit ao fim de cada um.

> Os IDs (T001...) são os mesmos da planilha `Controle_de_Tarefas_Grupo_1C.xlsx`. Marque o status por lá. Responsáveis e prazos marcados como "sugerido" ou "A definir" podem ser ajustados pelo grupo.

**48 tarefas** nesta frente.

## Marcos desta frente

| Marco | Nome | Tarefas | O que está pronto |
|---|---|---|---|
| M1 | V1 no repositório | 3 | O HTML original está no GitHub, cada integrante tem o repositório no computador e cada página tem uma branch. |
| M2 | Bootstrap e CSS ligados | 8 | Cada página carrega Bootstrap, estilo.css e o tema de cor. Visual ainda simples, mas a base está pronta. |
| M3 | Casca padronizada | 8 | Navbar, faixa de abertura (hero) com botões e rodapé iguais nas 5 páginas. |
| M4 | Seções em grade | 13 | O conteúdo está organizado em seções com container, row e col (Bootstrap) e em cartões. |
| M5 | Estilo final | 8 | Cores do tema, cartões com borda arredondada e sombra, efeito hover/foco e barra colorida nos títulos. |
| M6 | Revisão e entrega v3 | 8 | HTML validado, nada perdido, testado em celular/tablet/PC, Pull Request aprovado e versão v3 marcada. |

## Como estudar

- "PDF" é o material *O Cardápio do Navegador: CSS do Seletor ao Bootstrap* (capítulos indicados em cada tarefa).
- "Fora do PDF" são páginas oficiais; abra só a parte do assunto da tarefa, não precisa ler o site inteiro.

## M1 · V1 no repositório

*O HTML original está no GitHub, cada integrante tem o repositório no computador e cada página tem uma branch.*

#### T264 · Criar a branch pagina-luiz
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T002

- **O que fazer:** No terminal, dentro da pasta do repositório: "git switch -c pagina-luiz". A branch é uma cópia de trabalho só sua; a main fica protegida.
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2); [GitHub Docs: Hello World](https://docs.github.com/en/get-started/start-your-journey/hello-world)
- **Pronto quando:** "git branch" mostra pagina-luiz com um asterisco.

#### T265 · Abrir luiz.html no navegador e listar o que aparece
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T264

- **O que fazer:** Abra o arquivo e escreva uma lista curta: título, textos, fotos, listas e links que você vê. Isso vira seu mapa para não perder nada.
- **Estudar no PDF:** Cap. 1.1 (HTML descreve o conteúdo)
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Lista escrita (pode ser no bloco de notas).

#### T266 · Contar as imagens e os links de luiz.html
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T265

- **O que fazer:** Abra o arquivo no editor, use Ctrl+F e procure "<img" e "<a ". Anote os números. No original: 19 imagens e 7 links. No fim, a V3 tem de ter os mesmos.
- **Pronto quando:** Anotado: 19 imagens e 7 links.

## M2 · Bootstrap e CSS ligados

*Cada página carrega Bootstrap, estilo.css e o tema de cor. Visual ainda simples, mas a base está pronta.*

#### T267 · Conferir lang="pt-br" e meta charset UTF-8
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T266

- **O que fazer:** Confirme que a primeira linha tem <html lang="pt-br"> e o <head> tem <meta charset="UTF-8">. O charset garante que acentos apareçam certos.
- **Estudar no PDF:** Cap. 8.1
- **Pronto quando:** As duas linhas estão presentes.

#### T268 · Adicionar a meta viewport (o original não tem)
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T267

- **O que fazer:** No <head> acrescente <meta name="viewport" content="width=device-width, initial-scale=1.0">. Sem ela o celular mostra o site de computador encolhido.
- **Estudar no PDF:** Cap. 7.1 (meta viewport)
- **Estudar fora do PDF:** [PDF F17: Responsive web design basics (web.dev)](https://web.dev/articles/responsive-web-design-basics); [Chrome DevTools: device mode](https://developer.chrome.com/docs/devtools/device-mode)
- **Pronto quando:** A linha existe no <head>.

#### T269 · Ligar o Bootstrap 5.3.9 no <head> de luiz.html
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T268

- **O que fazer:** Copie do modelo/head.html (ou do site oficial) a linha <link ... bootstrap.min.css>. Sem internet o Bootstrap não carrega.
- **Estudar no PDF:** Cap. 8.1 (instalar pelo CDN)
- **Estudar fora do PDF:** [Bootstrap 5.3: Get started](https://getbootstrap.com/docs/5.3/getting-started/introduction/)
- **Pronto quando:** Ao recarregar, a fonte e os espaços do texto mudam um pouco.

#### T270 · Ligar ../css/estilo.css depois do Bootstrap
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T269

- **O que fazer:** Acrescente <link rel="stylesheet" href="../css/estilo.css"> logo abaixo da linha do Bootstrap. A ordem importa: quem vem por último vence em caso de empate.
- **Estudar no PDF:** Cap. 1.2 (CSS externo) e 1.4 (cascata)
- **Pronto quando:** Fonte do body mudou para Segoe UI/Arial.

#### T271 · Ligar ../css/tema-luiz.css depois do estilo.css
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T270

- **O que fazer:** Acrescente <link rel="stylesheet" href="../css/tema-luiz.css"> como terceira linha de CSS.
- **Estudar no PDF:** Cap. 1.2 e 1.4
- **Pronto quando:** Linha adicionada.

#### T272 · Colocar class="tema-luiz" na tag <body>
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T271

- **O que fazer:** Troque <body> por <body class="tema-luiz">. O CSS do tema só age em páginas que tenham essa classe.
- **Estudar no PDF:** Cap. 1.3 (seletor de classe)
- **Pronto quando:** Fundo da página na cor do tema (vermelho).

#### T273 · Testar: recarregar e ver se o fundo e a fonte mudaram
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T272

- **O que fazer:** Abra com F5. Se nada mudou, abra o DevTools (F12), aba Console/Network, e veja qual arquivo deu erro 404 (caminho errado).
- **Estudar fora do PDF:** [Chrome DevTools: device mode](https://developer.chrome.com/docs/devtools/device-mode)
- **Pronto quando:** Fundo e fonte corretos, sem erro 404.

#### T274 · Commit do marco M2
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T273

- **O que fazer:** git add luiz.html e git commit -m "M2 Luiz: Bootstrap e CSS ligados". Um commit por marco facilita desfazer se algo der errado.
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Commit criado.

## M3 · Casca padronizada

*Navbar, faixa de abertura (hero) com botões e rodapé iguais nas 5 páginas.*

#### T275 · Colar a navbar no início do <body> de luiz.html
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T274

- **O que fazer:** Copie o bloco de modelo/navbar.html e cole logo depois de <body>. A navbar é a mesma em todas as páginas.
- **Estudar no PDF:** Cap. 4.2
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Barra de navegação aparece no topo.

#### T276 · Marcar o link da própria página como ativo
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T275

- **O que fazer:** No bloco da navbar, no link desta página, escreva class="ativo" aria-current="page". A aba ativa fica branca e mostra onde você está.
- **Estudar no PDF:** Cap. 6.1 (estado visual)
- **Pronto quando:** Só um link está destacado.

#### T277 · Testar os 5 links da navbar
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T276

- **O que fazer:** Clique em cada link. Todos devem abrir a página certa, na mesma aba.
- **Pronto quando:** 5 links funcionando.

#### T278 · Criar o hero com o título "Luiz Miguel Félix Ferreira"
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T277

- **O que fazer:** Depois da navbar, crie <section class="hero"><div class="container"><h1>…</h1></div></section> e mova para lá o título atual da página.
- **Estudar no PDF:** Cap. 8.2 (container) e 1.3
- **Estudar fora do PDF:** [Bootstrap 5.3: Grid system](https://getbootstrap.com/docs/5.3/layout/grid/)
- **Pronto quando:** Faixa colorida com o título dentro.

#### T279 · Montar o rótulo "TÓPICOS DA PÁGINA" e os botões de atalho
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~25 min · **Depois de:** T278

- **O que fazer:** Dentro do hero: <h2 class="rotulo">TÓPICOS DA PÁGINA</h2> e uma <ul class="atalhos"> com um <li><a class="btn btn-primary" href="..."> por botão: Voltar para a Página inicial, Algumas Curiosidades sobre Mim, Viagens e Fotos !. Os links internos usam #id da seção.
- **Estudar no PDF:** Cap. 8.3 (btn btn-primary)
- **Estudar fora do PDF:** [Bootstrap 5.3: Get started](https://getbootstrap.com/docs/5.3/getting-started/introduction/)
- **Pronto quando:** Fileira de botões brancos abaixo do título.

#### T280 · Colar o rodapé antes de </body>
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T279

- **O que fazer:** Copie modelo/rodape.html e cole logo antes de </body>, depois de </main> (que será criado no M4).
- **Estudar no PDF:** Cap. 8.2
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Rodapé aparece no fim da página.

#### T281 · Testar o link "Volte ao topo da página!"
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T280

- **O que fazer:** Clique no link do rodapé: a página deve subir até a navbar (o id="topo" está no <header>).
- **Pronto quando:** Página sobe até o topo.

#### T282 · Commit do marco M3
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T281

- **O que fazer:** git add luiz.html e git commit -m "M3 Luiz: navbar, hero e rodapé".
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Commit criado.

## M4 · Seções em grade

*O conteúdo está organizado em seções com container, row e col (Bootstrap) e em cartões.*

#### T283 · Envolver todo o conteúdo entre o hero e o rodapé com <main>
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T282

- **O que fazer:** <main> marca o conteúdo principal da página. Ele fica entre </header> e <footer>.
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** <main> abre depois do hero e fecha antes do rodapé.

#### T284 · Remover as <hr> (linhas horizontais) do conteúdo
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T283

- **O que fazer:** As linhas separavam as partes no HTML antigo. Com seções coloridas elas não são mais necessárias; apague as tags <hr>.
- **Estudar no PDF:** Cap. 3.1
- **Pronto quando:** Nenhuma <hr> no arquivo.

#### T285 · Criar <section id="sobremim"> sem título, com a lista de dados e as fotos
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T284

- **O que fazer:** O original não tem "Sobre mim". Crie a seção sem h2: coluna col-12 col-lg-7 com a lista (1 Ano C - TEC, 15 anos, Osasco - SP) e col-12 col-lg-5 com as fotos.
- **Estudar no PDF:** Cap. 8.2
- **Estudar fora do PDF:** [Bootstrap 5.3: Grid system](https://getbootstrap.com/docs/5.3/layout/grid/)
- **Pronto quando:** Dados e fotos lado a lado.

#### T286 · Foto principal (aa.jpg) em col-12 e o emoji em col-6
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T285

- **O que fazer:** Dentro da coluna das fotos: <div class="row g-3"> com aa.jpg em <div class="col-12"> e o emoji (Luiz_favicon.png) em <div class="col-6">.
- **Estudar no PDF:** Cap. 8.2
- **Pronto quando:** Foto grande e emoji menor.

#### T287 · Criar <section id="curiosidades"> com o h2 "Algumas Curiosidades sobre Mim"
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T286

- **O que fazer:** Seção com container e h2. É o destino do botão do hero.
- **Estudar no PDF:** Cap. 8.2
- **Pronto quando:** Seção criada.

#### T288 · Remover os <br> soltos entre os itens da lista
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T287

- **O que fazer:** No original há <br> entre os <li> (HTML inválido). Apague: o espaço agora vem da grade (g-3).
- **Estudar fora do PDF:** [Validador de HTML do W3C](https://validator.w3.org/)
- **Pronto quando:** Nenhum <br> direto dentro de <ul>.

#### T289 · Transformar os 3 itens em cartões com a imagem pequena
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~25 min · **Depois de:** T288

- **O que fazer:** Cada <li> vira <li class="col-12 col-md-6 col-lg-4"><div class="cartao"><p>texto</p><div class="midias"><img class="mini" …></div></div></li>. Textos: esportes, música/videogame e teclado.
- **Estudar no PDF:** Cap. 8.2 e 3.3 (largura em %)
- **Pronto quando:** 3 cartões com a imagem abaixo do texto.

#### T290 · Criar <section id="visitei"> com o h2 "Viagens" e os dois h3
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T289

- **O que fazer:** Dentro: h3 "Lugares que eu já visitei" + row g-3; depois h3 "Lugares que eu quero conhecer" + row g-3. São as duas colunas da tabela do original, agora uma abaixo da outra.
- **Estudar no PDF:** Cap. 8.2
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Seção com dois blocos e seus títulos.

#### T291 · Substituir a tabela por cartões (Porto Seguro, Águas de Lindóia, Teresina)
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~25 min · **Depois de:** T290

- **O que fazer:** Cada <li> (link do nome + foto) vira um cartão col-12 col-md-6 col-lg-4 com <h3><a>nome</a></h3> e a foto.
- **Estudar no PDF:** Cap. 8.2
- **Estudar fora do PDF:** [Bootstrap 5.3: Grid system](https://getbootstrap.com/docs/5.3/layout/grid/)
- **Pronto quando:** 3 cartões de lugares visitados.

#### T292 · Repetir para Jericoacoara, Santiago (Chile) e Buenos Aires
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T291

- **O que fazer:** Mesma estrutura para "Lugares que eu quero conhecer".
- **Estudar no PDF:** Cap. 8.2
- **Pronto quando:** 3 cartões.

#### T293 · Apagar as tags <table>, <tr>, <th>, <td> e os atributos border/cellpadding/valign
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T292

- **O que fazer:** Depois que todo o conteúdo estiver nos cartões, remova a tabela. Esses atributos são antigos; o visual agora vem do CSS e da grade.
- **Estudar no PDF:** Cap. 3.1 (borda e padding no CSS)
- **Pronto quando:** Sem <table> no arquivo.

#### T294 · Criar <section id="fotos"> com o h2 "Fotos !" e 8 fotos em col-6 col-md-4 col-lg-3
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~25 min · **Depois de:** T293

- **O que fazer:** Cada imagem em <div class="col-6 col-md-4 col-lg-3"><figure class="foto"><img …></figure></div>.
- **Estudar no PDF:** Cap. 8.2
- **Estudar fora do PDF:** [Bootstrap 5.3: Grid system](https://getbootstrap.com/docs/5.3/layout/grid/)
- **Pronto quando:** Galeria com 8 fotos.

#### T295 · Trocar o alt "ft" por textos descritivos (Foto 1 a Foto 8)
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T294

- **O que fazer:** O alt "ft" não diz nada ao leitor de tela. Use "Foto 1", "Foto 2"… ou, melhor, descreva a foto.
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** 8 alt diferentes.

## M5 · Estilo final

*Cores do tema, cartões com borda arredondada e sombra, efeito hover/foco e barra colorida nos títulos.*

#### T296 · Trocar width e height das imagens por CSS
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T295

- **O que fazer:** Apague os atributos width="…" e height="…" das <img>. Quem controla o tamanho agora é o CSS (img { max-width: 100%; height: auto; }) e as colunas.
- **Estudar no PDF:** Cap. 7.3
- **Estudar fora do PDF:** [PDF F17: Responsive web design basics (web.dev)](https://web.dev/articles/responsive-web-design-basics)
- **Pronto quando:** Nenhuma <img> com width/height.

#### T297 · Aplicar class="titulo" em todos os h2 das seções
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T296

- **O que fazer:** Acrescente class="titulo" nos h2. A barra colorida antes do título vem do CSS (::before).
- **Estudar no PDF:** Cap. 6.3
- **Pronto quando:** Barra colorida antes de cada título.

#### T298 · Aplicar class="cartao" nas caixas de conteúdo
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T297

- **O que fazer:** Coloque <div class="cartao"> em volta de cada item que virou cartão (curiosidades, lugares, integrantes).
- **Estudar no PDF:** Cap. 3.4
- **Pronto quando:** Cartões com canto redondo e sombra.

#### T299 · Aplicar class="foto" nas imagens das galerias
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T298

- **O que fazer:** Use <figure class="foto"><img …></figure> para foto sem link e <a class="foto" href="…"><img …></a> para foto com link.
- **Estudar no PDF:** Cap. 3.4 e 6.1
- **Pronto quando:** Fotos arredondadas, com sombra e hover.

#### T300 · Alternar o fundo das seções com class="secao secao-alt"
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T299

- **O que fazer:** Use <section class="secao"> e, de duas em duas seções, <section class="secao secao-alt"> para alternar o fundo.
- **Estudar no PDF:** Cap. 1.4 (várias classes no mesmo elemento)
- **Pronto quando:** Fundos alternando.

#### T301 · Testar hover e foco pelo teclado
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T300

- **O que fazer:** Passe o mouse nos cartões e fotos e depois aperte Tab várias vezes. Todo link deve mostrar um destaque ao receber foco.
- **Estudar no PDF:** Cap. 6.1
- **Estudar fora do PDF:** [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/)
- **Pronto quando:** Hover e foco visíveis.

#### T302 · Conferir as cores do tema na página inteira
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T301

- **O que fazer:** Olhe navbar, hero, títulos, links e rodapé: tudo na cor vermelho e legível.
- **Estudar no PDF:** Cap. 2.1
- **Estudar fora do PDF:** [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/)
- **Pronto quando:** Visual coerente com o tema.

#### T303 · Commit do marco M5
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T302

- **O que fazer:** git add . e git commit -m "M5 Luiz: estilo final".
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Commit criado.

## M6 · Revisão e entrega v3

*HTML validado, nada perdido, testado em celular/tablet/PC, Pull Request aprovado e versão v3 marcada.*

#### T304 · Validar luiz.html no validador HTML do W3C
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~30 min · **Depois de:** T303

- **O que fazer:** Abra o validador, escolha "Validate by File Upload" ou "Direct Input" e envie o arquivo. Corrija cada erro listado (tag aberta sem fechar, atributo errado).
- **Estudar fora do PDF:** [Validador de HTML do W3C](https://validator.w3.org/); [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Sem erros (avisos podem ficar).

#### T305 · Comparar a contagem de imagens e links com a do M1
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T304

- **O que fazer:** Repita o Ctrl+F do M1. Tem de dar 19 imagens e os 7 links do original (a navbar e o rodapé acrescentam links novos: confira só os do conteúdo).
- **Pronto quando:** Números batem.

#### T306 · Ler texto novo x texto original lado a lado
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T305

- **O que fazer:** Abra o HTML do M1 (git show) e a página nova e confira se todos os textos continuam lá, com as mesmas palavras.
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Nenhum texto perdido ou alterado.

#### T307 · Testar em 360, 768 e 1200 px no DevTools
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T306

- **O que fazer:** No Chrome aperte F12 e clique no ícone de celular/tablet. Teste as 3 larguras. Nenhuma rolagem horizontal pode aparecer.
- **Estudar no PDF:** Cap. 7.2 e 8.2 (breakpoints md = 768 px)
- **Estudar fora do PDF:** [Chrome DevTools: device mode](https://developer.chrome.com/docs/devtools/device-mode); [Bootstrap 5.3: Grid system](https://getbootstrap.com/docs/5.3/layout/grid/)
- **Pronto quando:** 3 larguras sem rolagem horizontal e com layout certo.

#### T308 · Clicar em todos os links externos da página
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T307

- **O que fazer:** Abra cada link externo numa nova aba e anote os que não abrem. Entregue a lista para a tarefa "Consolidar os links externos".
- **Pronto quando:** Lista de links quebrados (pode ser vazia).

#### T309 · Abrir o Pull Request da branch
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T308

- **O que fazer:** git push -u origin pagina-luiz; no GitHub clique em "Compare & pull request", descreva o que mudou e peça revisão de outra pessoa.
- **Estudar fora do PDF:** [GitHub Docs: Creating a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request); [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Pull Request aberto com revisor.

#### T310 · Revisar o Pull Request de outra pessoa (checklist)
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T309

- **O que fazer:** Quem revisa abre a aba "Files changed", segue o checklist e comenta ou aprova. Só depois o autor faz o merge.
- **Estudar fora do PDF:** [GitHub Docs: Creating a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)
- **Pronto quando:** PR aprovado por alguém que não é o autor.

#### T311 · Fazer o merge na main e atualizar o status no Excel
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T310

- **O que fazer:** Com o PR aprovado, clique em "Merge pull request". Depois marque as tarefas da página como Concluída nesta planilha.
- **Estudar fora do PDF:** [GitHub Docs: Creating a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)
- **Pronto quando:** Página na main e status atualizado.

## Fontes desta frente

- [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2) (aberta em 17/11/2026)
- [GitHub Docs: Hello World](https://docs.github.com/en/get-started/start-your-journey/hello-world) (aberta em 17/11/2026)
- [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements) (aberta em 17/11/2026)
- PDF F17: [Responsive web design basics (web.dev)](https://web.dev/articles/responsive-web-design-basics) (citada na lista de fontes do PDF; não reaberta nesta sessão)
- [Chrome DevTools: device mode](https://developer.chrome.com/docs/devtools/device-mode) (aberta em 17/11/2026)
- [Bootstrap 5.3: Get started](https://getbootstrap.com/docs/5.3/getting-started/introduction/) (aberta em 17/11/2026)
- [Bootstrap 5.3: Grid system](https://getbootstrap.com/docs/5.3/layout/grid/) (aberta em 17/11/2026)
- [Validador de HTML do W3C](https://validator.w3.org/) (aberta em 17/11/2026)
- [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/) (aberta em 17/11/2026)
- [GitHub Docs: Creating a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) (aberta em 17/11/2026)
