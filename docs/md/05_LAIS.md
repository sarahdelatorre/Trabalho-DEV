# Guia 5 de 6 · Página da Laís

Passo a passo para sair do estado inicial de `lais.html` e chegar à v3 (tema rosa). Responsável sugerido pela página: **Laís**. Faça um marco por vez e dê commit ao fim de cada um.

> Os IDs (T001...) são os mesmos da planilha `Controle_de_Tarefas_Grupo_1C.xlsx`. Marque o status por lá. Responsáveis e prazos marcados como "sugerido" ou "A definir" podem ser ajustados pelo grupo.

**47 tarefas** nesta frente.

## Marcos desta frente

| Marco | Nome | Tarefas | O que está pronto |
|---|---|---|---|
| M1 | V1 no repositório | 3 | O HTML original está no GitHub, cada integrante tem o repositório no computador e cada página tem uma branch. |
| M2 | Bootstrap e CSS ligados | 8 | Cada página carrega Bootstrap, estilo.css e o tema de cor. Visual ainda simples, mas a base está pronta. |
| M3 | Casca padronizada | 8 | Navbar, faixa de abertura (hero) com botões e rodapé iguais nas 5 páginas. |
| M4 | Seções em grade | 12 | O conteúdo está organizado em seções com container, row e col (Bootstrap) e em cartões. |
| M5 | Estilo final | 8 | Cores do tema, cartões com borda arredondada e sombra, efeito hover/foco e barra colorida nos títulos. |
| M6 | Revisão e entrega v3 | 8 | HTML validado, nada perdido, testado em celular/tablet/PC, Pull Request aprovado e versão v3 marcada. |

## Como estudar

- "PDF" é o material *O Cardápio do Navegador: CSS do Seletor ao Bootstrap* (capítulos indicados em cada tarefa).
- "Fora do PDF" são páginas oficiais; abra só a parte do assunto da tarefa, não precisa ler o site inteiro.

## M1 · V1 no repositório

*O HTML original está no GitHub, cada integrante tem o repositório no computador e cada página tem uma branch.*

#### T217 · Criar a branch pagina-lais
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T002

- **O que fazer:** No terminal, dentro da pasta do repositório: "git switch -c pagina-lais". A branch é uma cópia de trabalho só sua; a main fica protegida.
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2); [GitHub Docs: Hello World](https://docs.github.com/en/get-started/start-your-journey/hello-world)
- **Pronto quando:** "git branch" mostra pagina-lais com um asterisco.

#### T218 · Abrir lais.html no navegador e listar o que aparece
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T217

- **O que fazer:** Abra o arquivo e escreva uma lista curta: título, textos, fotos, listas e links que você vê. Isso vira seu mapa para não perder nada.
- **Estudar no PDF:** Cap. 1.1 (HTML descreve o conteúdo)
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Lista escrita (pode ser no bloco de notas).

#### T219 · Contar as imagens e os links de lais.html
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T218

- **O que fazer:** Abra o arquivo no editor, use Ctrl+F e procure "<img" e "<a ". Anote os números. No original: 15 imagens e 8 links. No fim, a V3 tem de ter os mesmos.
- **Pronto quando:** Anotado: 15 imagens e 8 links.

## M2 · Bootstrap e CSS ligados

*Cada página carrega Bootstrap, estilo.css e o tema de cor. Visual ainda simples, mas a base está pronta.*

#### T220 · Conferir lang="pt-br" e meta charset UTF-8
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T219

- **O que fazer:** Confirme que a primeira linha tem <html lang="pt-br"> e o <head> tem <meta charset="UTF-8">. O charset garante que acentos apareçam certos.
- **Estudar no PDF:** Cap. 8.1
- **Pronto quando:** As duas linhas estão presentes.

#### T221 · Conferir a meta viewport
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T220

- **O que fazer:** Confirme a linha <meta name="viewport" content="width=device-width, initial-scale=1.0"> no <head>. Ela faz o celular usar a largura real da tela.
- **Estudar no PDF:** Cap. 7.1
- **Pronto quando:** A linha existe no <head>.

#### T222 · Ligar o Bootstrap 5.3.9 no <head> de lais.html
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T221

- **O que fazer:** Copie do modelo/head.html (ou do site oficial) a linha <link ... bootstrap.min.css>. Sem internet o Bootstrap não carrega.
- **Estudar no PDF:** Cap. 8.1 (instalar pelo CDN)
- **Estudar fora do PDF:** [Bootstrap 5.3: Get started](https://getbootstrap.com/docs/5.3/getting-started/introduction/)
- **Pronto quando:** Ao recarregar, a fonte e os espaços do texto mudam um pouco.

#### T223 · Ligar css/estilo.css depois do Bootstrap
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T222

- **O que fazer:** Acrescente <link rel="stylesheet" href="css/estilo.css"> logo abaixo da linha do Bootstrap. A ordem importa: quem vem por último vence em caso de empate.
- **Estudar no PDF:** Cap. 1.2 (CSS externo) e 1.4 (cascata)
- **Pronto quando:** Fonte do body mudou para Segoe UI/Arial.

#### T224 · Ligar css/tema-lais.css depois do estilo.css
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T223

- **O que fazer:** Acrescente <link rel="stylesheet" href="css/tema-lais.css"> como terceira linha de CSS.
- **Estudar no PDF:** Cap. 1.2 e 1.4
- **Pronto quando:** Linha adicionada.

#### T225 · Colocar class="tema-lais" na tag <body>
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T224

- **O que fazer:** Troque <body> por <body class="tema-lais">. O CSS do tema só age em páginas que tenham essa classe.
- **Estudar no PDF:** Cap. 1.3 (seletor de classe)
- **Pronto quando:** Fundo da página na cor do tema (rosa).

#### T226 · Testar: recarregar e ver se o fundo e a fonte mudaram
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T225

- **O que fazer:** Abra com F5. Se nada mudou, abra o DevTools (F12), aba Console/Network, e veja qual arquivo deu erro 404 (caminho errado).
- **Estudar fora do PDF:** [Chrome DevTools: device mode](https://developer.chrome.com/docs/devtools/device-mode)
- **Pronto quando:** Fundo e fonte corretos, sem erro 404.

#### T227 · Commit do marco M2
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T226

- **O que fazer:** git add lais.html e git commit -m "M2 Laís: Bootstrap e CSS ligados". Um commit por marco facilita desfazer se algo der errado.
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Commit criado.

## M3 · Casca padronizada

*Navbar, faixa de abertura (hero) com botões e rodapé iguais nas 5 páginas.*

#### T228 · Colar a navbar no início do <body> de lais.html
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T227

- **O que fazer:** Copie o bloco de modelo/navbar.html e cole logo depois de <body>. A navbar é a mesma em todas as páginas.
- **Estudar no PDF:** Cap. 4.2
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Barra de navegação aparece no topo.

#### T229 · Marcar o link da própria página como ativo
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T228

- **O que fazer:** No bloco da navbar, no link desta página, escreva class="ativo" aria-current="page". A aba ativa fica branca e mostra onde você está.
- **Estudar no PDF:** Cap. 6.1 (estado visual)
- **Pronto quando:** Só um link está destacado.

#### T230 · Testar os 5 links da navbar
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T229

- **O que fazer:** Clique em cada link. Todos devem abrir a página certa, na mesma aba.
- **Pronto quando:** 5 links funcionando.

#### T231 · Criar o hero com o título "Laís Casteluci Almeida"
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T230

- **O que fazer:** Depois da navbar, crie <section class="hero"><div class="container"><h1>…</h1></div></section> e mova para lá o título atual da página.
- **Estudar no PDF:** Cap. 8.2 (container) e 1.3
- **Estudar fora do PDF:** [Bootstrap 5.3: Grid system](https://getbootstrap.com/docs/5.3/layout/grid/)
- **Pronto quando:** Faixa colorida com o título dentro.

#### T232 · Montar o rótulo "TÓPICOS DA PÁGINA" e os botões de atalho
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~25 min · **Depois de:** T231

- **O que fazer:** Dentro do hero: <h2 class="rotulo">TÓPICOS DA PÁGINA</h2> e uma <ul class="atalhos"> com um <li><a class="btn btn-primary" href="..."> por botão: Voltar para a página inicial, Sobre mim, Curiosidades, Lugares que já visitei e Lugares que quero visitar. Os links internos usam #id da seção.
- **Estudar no PDF:** Cap. 8.3 (btn btn-primary)
- **Estudar fora do PDF:** [Bootstrap 5.3: Get started](https://getbootstrap.com/docs/5.3/getting-started/introduction/)
- **Pronto quando:** Fileira de botões brancos abaixo do título.

#### T233 · Colar o rodapé antes de </body>
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T232

- **O que fazer:** Copie modelo/rodape.html e cole logo antes de </body>, depois de </main> (que será criado no M4).
- **Estudar no PDF:** Cap. 8.2
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Rodapé aparece no fim da página.

#### T234 · Testar o link "Volte ao topo da página!"
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T233

- **O que fazer:** Clique no link do rodapé: a página deve subir até a navbar (o id="topo" está no <header>).
- **Pronto quando:** Página sobe até o topo.

#### T235 · Commit do marco M3
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T234

- **O que fazer:** git add lais.html e git commit -m "M3 Laís: navbar, hero e rodapé".
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Commit criado.

## M4 · Seções em grade

*O conteúdo está organizado em seções com container, row e col (Bootstrap) e em cartões.*

#### T236 · Envolver todo o conteúdo entre o hero e o rodapé com <main>
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T235

- **O que fazer:** <main> marca o conteúdo principal da página. Ele fica entre </header> e <footer>.
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** <main> abre depois do hero e fecha antes do rodapé.

#### T237 · Remover as <hr> (linhas horizontais) do conteúdo
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T236

- **O que fazer:** As linhas separavam as partes no HTML antigo. Com seções coloridas elas não são mais necessárias; apague as tags <hr>.
- **Estudar no PDF:** Cap. 3.1
- **Pronto quando:** Nenhuma <hr> no arquivo.

#### T238 · Criar <section id="sobremim"> e mover o h2 "Sobre mim:" e os 2 parágrafos
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T237

- **O que fazer:** Seção com container e h2. O texto "Meu nome é Laís Casteluci Almeida…" e "Gosto muito de passar tempo…" vão para uma coluna col-12 col-lg-7.
- **Estudar no PDF:** Cap. 8.2
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Texto na coluna esquerda.

#### T239 · Montar a coluna de fotos (retrato col-6, tênis col-6, grupo col-12)
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T238

- **O que fazer:** Coluna col-12 col-lg-5 com <div class="row g-3">: retrato (WhatsApp … 16.51.09) e foto do tênis em col-6; foto com os amigos em col-12.
- **Estudar no PDF:** Cap. 8.2
- **Estudar fora do PDF:** [Bootstrap 5.3: Grid system](https://getbootstrap.com/docs/5.3/layout/grid/)
- **Pronto quando:** 3 fotos organizadas ao lado do texto.

#### T240 · Apagar os "." usados como espaçador entre as imagens
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T239

- **O que fazer:** No original há um ponto solto entre as duas imagens de várias linhas. Era um truque para afastar as fotos; com a grade não precisa mais.
- **Estudar no PDF:** Cap. 8.3 (g-3 dá o espaço)
- **Pronto quando:** Nenhum "." solto entre <img>.

#### T241 · Criar <section id="curiosidades"> e fazer 5 cartões (col-12 col-md-6 col-lg-4)
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~25 min · **Depois de:** T240

- **O que fazer:** Cada <li> da lista "Curiosidades" vira um cartão numa row g-3. As bolinhas somem (list-style: none).
- **Estudar no PDF:** Cap. 8.2
- **Pronto quando:** 5 cartões.

#### T242 · Criar <section id="visitei"> com a row g-3 dos 4 lugares
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T241

- **O que fazer:** h2 "Lugares que já visitei" e <div class="row g-3">.
- **Estudar no PDF:** Cap. 8.2
- **Pronto quando:** Seção criada.

#### T243 · Cartão do Balneário Camburiú (h3, foto e link)
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T242

- **O que fazer:** <div class="col-12 col-lg-6"><div class="cartao"> com o h3 "Balneário Camburiú, Santa Catarina", a foto (col-12) e o parágrafo com o link para a página de turismo.
- **Estudar no PDF:** Cap. 8.2
- **Pronto quando:** Cartão pronto.

#### T244 · Cartões do Beto Carrero Word, Maceio e Curitiba
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~30 min · **Depois de:** T243

- **O que fazer:** Mesma estrutura. Nos que têm 2 fotos, use <div class="row g-3"> com 2 colunas col-6; no de 1 foto (Curitiba) use col-12. Mantenha cada link "Clique aqui…" em <p class="saiba">.
- **Estudar no PDF:** Cap. 8.2
- **Estudar fora do PDF:** [Bootstrap 5.3: Grid system](https://getbootstrap.com/docs/5.3/layout/grid/)
- **Pronto quando:** 4 cartões de lugares na seção.

#### T245 · Criar <section id="visitar"> com Paris, Suíça e Itália
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~25 min · **Depois de:** T244

- **O que fazer:** Mesma estrutura de cartões, com id="visitar" e o h2 "Lugares que quero visitar".
- **Estudar no PDF:** Cap. 8.2
- **Pronto quando:** 3 cartões.

#### T246 · Conferir o alt das imagens (substituir os que estão com erro de digitação)
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T245

- **O que fazer:** Alguns alt têm erros ("imgem louvre", "Imagme coliseu"). Reescreva com poucas palavras corretas.
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Alt sem erros.

#### T247 · Limpar os parâmetros de rastreamento (gclid, utm) dos links (opcional)
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T246 · *opcional*

- **O que fazer:** Links do Beto Carrero e de Alagoas carregam códigos de anúncio depois do "?". Teste o link sem eles; se abrir igual, deixe o endereço mais curto.
- **Pronto quando:** Links curtos funcionando.

## M5 · Estilo final

*Cores do tema, cartões com borda arredondada e sombra, efeito hover/foco e barra colorida nos títulos.*

#### T248 · Trocar width e height das imagens por CSS
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T247

- **O que fazer:** Apague os atributos width="…" e height="…" das <img>. Quem controla o tamanho agora é o CSS (img { max-width: 100%; height: auto; }) e as colunas.
- **Estudar no PDF:** Cap. 7.3
- **Estudar fora do PDF:** [PDF F17: Responsive web design basics (web.dev)](https://web.dev/articles/responsive-web-design-basics)
- **Pronto quando:** Nenhuma <img> com width/height.

#### T249 · Aplicar class="titulo" em todos os h2 das seções
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T248

- **O que fazer:** Acrescente class="titulo" nos h2. A barra colorida antes do título vem do CSS (::before).
- **Estudar no PDF:** Cap. 6.3
- **Pronto quando:** Barra colorida antes de cada título.

#### T250 · Aplicar class="cartao" nas caixas de conteúdo
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T249

- **O que fazer:** Coloque <div class="cartao"> em volta de cada item que virou cartão (curiosidades, lugares, integrantes).
- **Estudar no PDF:** Cap. 3.4
- **Pronto quando:** Cartões com canto redondo e sombra.

#### T251 · Aplicar class="foto" nas imagens das galerias
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T250

- **O que fazer:** Use <figure class="foto"><img …></figure> para foto sem link e <a class="foto" href="…"><img …></a> para foto com link.
- **Estudar no PDF:** Cap. 3.4 e 6.1
- **Pronto quando:** Fotos arredondadas, com sombra e hover.

#### T252 · Alternar o fundo das seções com class="secao secao-alt"
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T251

- **O que fazer:** Use <section class="secao"> e, de duas em duas seções, <section class="secao secao-alt"> para alternar o fundo.
- **Estudar no PDF:** Cap. 1.4 (várias classes no mesmo elemento)
- **Pronto quando:** Fundos alternando.

#### T253 · Testar hover e foco pelo teclado
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T252

- **O que fazer:** Passe o mouse nos cartões e fotos e depois aperte Tab várias vezes. Todo link deve mostrar um destaque ao receber foco.
- **Estudar no PDF:** Cap. 6.1
- **Estudar fora do PDF:** [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/)
- **Pronto quando:** Hover e foco visíveis.

#### T254 · Conferir as cores do tema na página inteira
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T253

- **O que fazer:** Olhe navbar, hero, títulos, links e rodapé: tudo na cor rosa e legível.
- **Estudar no PDF:** Cap. 2.1
- **Estudar fora do PDF:** [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/)
- **Pronto quando:** Visual coerente com o tema.

#### T255 · Commit do marco M5
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T254

- **O que fazer:** git add . e git commit -m "M5 Laís: estilo final".
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Commit criado.

## M6 · Revisão e entrega v3

*HTML validado, nada perdido, testado em celular/tablet/PC, Pull Request aprovado e versão v3 marcada.*

#### T256 · Validar lais.html no validador HTML do W3C
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~30 min · **Depois de:** T255

- **O que fazer:** Abra o validador, escolha "Validate by File Upload" ou "Direct Input" e envie o arquivo. Corrija cada erro listado (tag aberta sem fechar, atributo errado).
- **Estudar fora do PDF:** [Validador de HTML do W3C](https://validator.w3.org/); [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Sem erros (avisos podem ficar).

#### T257 · Comparar a contagem de imagens e links com a do M1
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T256

- **O que fazer:** Repita o Ctrl+F do M1. Tem de dar 15 imagens e os 8 links do original (a navbar e o rodapé acrescentam links novos: confira só os do conteúdo).
- **Pronto quando:** Números batem.

#### T258 · Ler texto novo x texto original lado a lado
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T257

- **O que fazer:** Abra o HTML do M1 (git show) e a página nova e confira se todos os textos continuam lá, com as mesmas palavras.
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Nenhum texto perdido ou alterado.

#### T259 · Testar em 360, 768 e 1200 px no DevTools
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T258

- **O que fazer:** No Chrome aperte F12 e clique no ícone de celular/tablet. Teste as 3 larguras. Nenhuma rolagem horizontal pode aparecer.
- **Estudar no PDF:** Cap. 7.2 e 8.2 (breakpoints md = 768 px)
- **Estudar fora do PDF:** [Chrome DevTools: device mode](https://developer.chrome.com/docs/devtools/device-mode); [Bootstrap 5.3: Grid system](https://getbootstrap.com/docs/5.3/layout/grid/)
- **Pronto quando:** 3 larguras sem rolagem horizontal e com layout certo.

#### T260 · Clicar em todos os links externos da página
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T259

- **O que fazer:** Abra cada link externo numa nova aba e anote os que não abrem. Entregue a lista para a tarefa "Consolidar os links externos".
- **Pronto quando:** Lista de links quebrados (pode ser vazia).

#### T261 · Abrir o Pull Request da branch
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T260

- **O que fazer:** git push -u origin pagina-lais; no GitHub clique em "Compare & pull request", descreva o que mudou e peça revisão de outra pessoa.
- **Estudar fora do PDF:** [GitHub Docs: Creating a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request); [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Pull Request aberto com revisor.

#### T262 · Revisar o Pull Request de outra pessoa (checklist)
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T261

- **O que fazer:** Quem revisa abre a aba "Files changed", segue o checklist e comenta ou aprova. Só depois o autor faz o merge.
- **Estudar fora do PDF:** [GitHub Docs: Creating a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)
- **Pronto quando:** PR aprovado por alguém que não é o autor.

#### T263 · Fazer o merge na main e atualizar o status no Excel
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T262

- **O que fazer:** Com o PR aprovado, clique em "Merge pull request". Depois marque as tarefas da página como Concluída nesta planilha.
- **Estudar fora do PDF:** [GitHub Docs: Creating a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)
- **Pronto quando:** Página na main e status atualizado.

## Fontes desta frente

- [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2) (aberta em 17/11/2026)
- [GitHub Docs: Hello World](https://docs.github.com/en/get-started/start-your-journey/hello-world) (aberta em 17/11/2026)
- [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements) (aberta em 17/11/2026)
- [Bootstrap 5.3: Get started](https://getbootstrap.com/docs/5.3/getting-started/introduction/) (aberta em 17/11/2026)
- [Chrome DevTools: device mode](https://developer.chrome.com/docs/devtools/device-mode) (aberta em 17/11/2026)
- [Bootstrap 5.3: Grid system](https://getbootstrap.com/docs/5.3/layout/grid/) (aberta em 17/11/2026)
- PDF F17: [Responsive web design basics (web.dev)](https://web.dev/articles/responsive-web-design-basics) (citada na lista de fontes do PDF; não reaberta nesta sessão)
- [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/) (aberta em 17/11/2026)
- [Validador de HTML do W3C](https://validator.w3.org/) (aberta em 17/11/2026)
- [GitHub Docs: Creating a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) (aberta em 17/11/2026)
