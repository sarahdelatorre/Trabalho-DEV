# Guia 2 de 6 · Página inicial (home)

Passo a passo para sair do estado inicial de `index.html` e chegar à v3 (tema azul-marinho). Responsável sugerido pela página: **Luiz**. Faça um marco por vez e dê commit ao fim de cada um.

> Os IDs (T001...) são os mesmos da planilha `Controle_de_Tarefas_Grupo_1C.xlsx`. Marque o status por lá. Responsáveis e prazos marcados como "sugerido" ou "A definir" podem ser ajustados pelo grupo.

**47 tarefas** nesta frente.

## Marcos desta frente

| Marco | Nome | Tarefas | O que está pronto |
|---|---|---|---|
| M1 | V1 no repositório | 3 | O HTML original está no GitHub, cada integrante tem o repositório no computador e cada página tem uma branch. |
| M2 | Bootstrap e CSS ligados | 9 | Cada página carrega Bootstrap, estilo.css e o tema de cor. Visual ainda simples, mas a base está pronta. |
| M3 | Casca padronizada | 9 | Navbar, faixa de abertura (hero) com botões e rodapé iguais nas 5 páginas. |
| M4 | Seções em grade | 10 | O conteúdo está organizado em seções com container, row e col (Bootstrap) e em cartões. |
| M5 | Estilo final | 8 | Cores do tema, cartões com borda arredondada e sombra, efeito hover/foco e barra colorida nos títulos. |
| M6 | Revisão e entrega v3 | 8 | HTML validado, nada perdido, testado em celular/tablet/PC, Pull Request aprovado e versão v3 marcada. |

## Como estudar

- "PDF" é o material *O Cardápio do Navegador: CSS do Seletor ao Bootstrap* (capítulos indicados em cada tarefa).
- "Fora do PDF" são páginas oficiais; abra só a parte do assunto da tarefa, não precisa ler o site inteiro.

## M1 · V1 no repositório

*O HTML original está no GitHub, cada integrante tem o repositório no computador e cada página tem uma branch.*

#### T060 · Criar a branch pagina-home
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T002

- **O que fazer:** No terminal, dentro da pasta do repositório: "git switch -c pagina-home". A branch é uma cópia de trabalho só sua; a main fica protegida.
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2); [GitHub Docs: Hello World](https://docs.github.com/en/get-started/start-your-journey/hello-world)
- **Pronto quando:** "git branch" mostra pagina-home com um asterisco.

#### T061 · Abrir index.html no navegador e listar o que aparece
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T060

- **O que fazer:** Abra o arquivo e escreva uma lista curta: título, textos, fotos, listas e links que você vê. Isso vira seu mapa para não perder nada.
- **Estudar no PDF:** Cap. 1.1 (HTML descreve o conteúdo)
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Lista escrita (pode ser no bloco de notas).

#### T062 · Contar as imagens e os links de index.html
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T061

- **O que fazer:** Abra o arquivo no editor, use Ctrl+F e procure "<img" e "<a ". Anote os números. No original: 4 imagens e 5 links. No fim, a V3 tem de ter os mesmos.
- **Pronto quando:** Anotado: 4 imagens e 5 links.

## M2 · Bootstrap e CSS ligados

*Cada página carrega Bootstrap, estilo.css e o tema de cor. Visual ainda simples, mas a base está pronta.*

#### T063 · Conferir lang="pt-br" e meta charset UTF-8
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T062

- **O que fazer:** Confirme que a primeira linha tem <html lang="pt-br"> e o <head> tem <meta charset="UTF-8">. O charset garante que acentos apareçam certos.
- **Estudar no PDF:** Cap. 8.1
- **Pronto quando:** As duas linhas estão presentes.

#### T064 · Conferir a meta viewport
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T063

- **O que fazer:** Confirme a linha <meta name="viewport" content="width=device-width, initial-scale=1.0"> no <head>. Ela faz o celular usar a largura real da tela.
- **Estudar no PDF:** Cap. 7.1
- **Pronto quando:** A linha existe no <head>.

#### T065 · Ligar o Bootstrap 5.3.9 no <head> de index.html
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T064

- **O que fazer:** Copie do modelo/head.html (ou do site oficial) a linha <link ... bootstrap.min.css>. Sem internet o Bootstrap não carrega.
- **Estudar no PDF:** Cap. 8.1 (instalar pelo CDN)
- **Estudar fora do PDF:** [Bootstrap 5.3: Get started](https://getbootstrap.com/docs/5.3/getting-started/introduction/)
- **Pronto quando:** Ao recarregar, a fonte e os espaços do texto mudam um pouco.

#### T066 · Ligar css/estilo.css depois do Bootstrap
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T065

- **O que fazer:** Acrescente <link rel="stylesheet" href="css/estilo.css"> logo abaixo da linha do Bootstrap. A ordem importa: quem vem por último vence em caso de empate.
- **Estudar no PDF:** Cap. 1.2 (CSS externo) e 1.4 (cascata)
- **Pronto quando:** Fonte do body mudou para Segoe UI/Arial.

#### T067 · Ligar css/tema-home.css depois do estilo.css
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T066

- **O que fazer:** Acrescente <link rel="stylesheet" href="css/tema-home.css"> como terceira linha de CSS.
- **Estudar no PDF:** Cap. 1.2 e 1.4
- **Pronto quando:** Linha adicionada.

#### T068 · Colocar class="tema-home" na tag <body>
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T067

- **O que fazer:** Troque <body> por <body class="tema-home">. O CSS do tema só age em páginas que tenham essa classe.
- **Estudar no PDF:** Cap. 1.3 (seletor de classe)
- **Pronto quando:** Fundo da página na cor do tema (azul-marinho).

#### T069 · Testar: recarregar e ver se o fundo e a fonte mudaram
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T068

- **O que fazer:** Abra com F5. Se nada mudou, abra o DevTools (F12), aba Console/Network, e veja qual arquivo deu erro 404 (caminho errado).
- **Estudar fora do PDF:** [Chrome DevTools: device mode](https://developer.chrome.com/docs/devtools/device-mode)
- **Pronto quando:** Fundo e fonte corretos, sem erro 404.

#### T070 · Commit do marco M2
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T069

- **O que fazer:** git add index.html e git commit -m "M2 Home: Bootstrap e CSS ligados". Um commit por marco facilita desfazer se algo der errado.
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Commit criado.

#### T071 · Adicionar a tag <body> que está faltando
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T070

- **O que fazer:** O original abre o conteúdo direto depois do </head>, sem <body>. Escreva <body> logo depois do </head> e </body> antes do </html>. Os navegadores corrigem sozinhos, mas o certo é escrever.
- **Estudar no PDF:** Cap. 8.1 (estrutura <head> e <body>)
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements); [Validador de HTML do W3C](https://validator.w3.org/)
- **Pronto quando:** <body> aberto e fechado.

## M3 · Casca padronizada

*Navbar, faixa de abertura (hero) com botões e rodapé iguais nas 5 páginas.*

#### T072 · Colar a navbar no início do <body> de index.html
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T071

- **O que fazer:** Copie o bloco de modelo/navbar.html e cole logo depois de <body>. A navbar é a mesma em todas as páginas.
- **Estudar no PDF:** Cap. 4.2
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Barra de navegação aparece no topo.

#### T073 · Marcar o link da própria página como ativo
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T072

- **O que fazer:** No bloco da navbar, no link desta página, escreva class="ativo" aria-current="page". A aba ativa fica branca e mostra onde você está.
- **Estudar no PDF:** Cap. 6.1 (estado visual)
- **Pronto quando:** Só um link está destacado.

#### T074 · Testar os 5 links da navbar
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T073

- **O que fazer:** Clique em cada link. Todos devem abrir a página certa, na mesma aba.
- **Pronto quando:** 5 links funcionando.

#### T075 · Criar o hero com o título "Bem-vindo à página inicial"
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T074

- **O que fazer:** Depois da navbar, crie <section class="hero"><div class="container"><h1>…</h1></div></section> e mova para lá o título atual da página.
- **Estudar no PDF:** Cap. 8.2 (container) e 1.3
- **Estudar fora do PDF:** [Bootstrap 5.3: Grid system](https://getbootstrap.com/docs/5.3/layout/grid/)
- **Pronto quando:** Faixa colorida com o título dentro.

#### T076 · Acrescentar o subtítulo "Grupo pertencente ao 1ºC" no hero
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T075

- **O que fazer:** Mova o h2 "Grupo pertencente ao 1ºC" para dentro do hero, logo abaixo do h1.
- **Estudar no PDF:** Cap. 1.3
- **Pronto quando:** Subtítulo na faixa colorida.

#### T077 · Montar o rótulo "TÓPICOS DA PÁGINA" e os botões de atalho
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~25 min · **Depois de:** T076

- **O que fazer:** Dentro do hero: <h2 class="rotulo">TÓPICOS DA PÁGINA</h2> e uma <ul class="atalhos"> com um <li><a class="btn btn-primary" href="..."> por botão: os 4 nomes completos dos integrantes (cada botão leva à página da pessoa). Os links internos usam #id da seção.
- **Estudar no PDF:** Cap. 8.3 (btn btn-primary)
- **Estudar fora do PDF:** [Bootstrap 5.3: Get started](https://getbootstrap.com/docs/5.3/getting-started/introduction/)
- **Pronto quando:** Fileira de botões brancos abaixo do título.

#### T078 · Colar o rodapé antes de </body>
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T077

- **O que fazer:** Copie modelo/rodape.html e cole logo antes de </body>, depois de </main> (que será criado no M4).
- **Estudar no PDF:** Cap. 8.2
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Rodapé aparece no fim da página.

#### T079 · Testar o link "Volte ao topo da página!"
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T078

- **O que fazer:** Clique no link do rodapé: a página deve subir até a navbar (o id="topo" está no <header>).
- **Pronto quando:** Página sobe até o topo.

#### T080 · Commit do marco M3
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T079

- **O que fazer:** git add index.html e git commit -m "M3 Home: navbar, hero e rodapé".
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Commit criado.

## M4 · Seções em grade

*O conteúdo está organizado em seções com container, row e col (Bootstrap) e em cartões.*

#### T081 · Envolver todo o conteúdo entre o hero e o rodapé com <main>
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T080

- **O que fazer:** <main> marca o conteúdo principal da página. Ele fica entre </header> e <footer>.
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** <main> abre depois do hero e fecha antes do rodapé.

#### T082 · Criar a seção "Clique nas imagens ou nos nomes…" com h2
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T081

- **O que fazer:** Dentro de <main>: <section class="secao" id="integrantes"><div class="container"><h2>…</h2> e passe para dentro o h2 "Clique nas imagens ou nos nomes para ler as apresentações individuais de cada um".
- **Estudar no PDF:** Cap. 8.2
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Seção com o h2 certo.

#### T083 · Criar <div class="row g-3"> para a fileira de cartões
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T082

- **O que fazer:** A "row" é a linha da grade Bootstrap e "g-3" dá espaço entre as colunas. Ela é filha do container.
- **Estudar no PDF:** Cap. 8.2 e 8.3 (g-3)
- **Estudar fora do PDF:** [Bootstrap 5.3: Grid system](https://getbootstrap.com/docs/5.3/layout/grid/)
- **Pronto quando:** Linha criada.

#### T084 · Fazer uma coluna por integrante com col-12 col-sm-6 col-lg-3
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T083

- **O que fazer:** col-12: 1 por linha no celular; col-sm-6: 2 por linha a partir de 576 px; col-lg-3: 4 por linha a partir de 992 px. Some as partes: 12 dividido por 3 dá 4 colunas.
- **Estudar no PDF:** Cap. 8.2 (grade de 12 partes e o exemplo resolvido)
- **Estudar fora do PDF:** [Bootstrap 5.3: Grid system](https://getbootstrap.com/docs/5.3/layout/grid/)
- **Pronto quando:** No DevTools: 1, 2 e 4 colunas conforme a largura.

#### T085 · Colocar cada imagem de integrante dentro de um cartão com link
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T084

- **O que fazer:** Dentro de cada coluna: <div class="cartao"> com <a href="pessoa.html"><img …></a>. O link é a própria imagem.
- **Estudar no PDF:** Cap. 3.1
- **Pronto quando:** 4 cartões com imagem clicável.

#### T086 · Corrigir os 3 links vazios (href="") para sarah/lais/luiz.html
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T085

- **O que fazer:** No original, só o Joel tem link na lista de nomes; os outros 3 estão vazios. Preencha com o arquivo de cada página.
- **Pronto quando:** Todos os links levam a uma página.

#### T087 · Corrigir o texto alternativo (alt) das 4 imagens
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T086

- **O que fazer:** No original todas têm alt="sarah Bazoni Macedo". Troque cada alt pelo nome da pessoa da imagem. O alt é lido por leitor de tela e aparece se a imagem falhar.
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** 4 alt diferentes e corretos.

#### T088 · Trocar a lista <h3><ol> por uma legenda numerada em cada cartão
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T087

- **O que fazer:** No original a lista numerada de nomes está dentro de um <h3> (HTML errado). Em cada cartão, depois da imagem, escreva <ol start="1"><li><a>Nome</a></li></ol>, mudando o start para 2, 3 e 4. Assim a numeração continua.
- **Estudar no PDF:** Cap. 1.3 (seletor de classe para a legenda)
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Legendas "1." a "4." com o nome em link.

#### T089 · Centralizar o texto dos cartões com text-center
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T088

- **O que fazer:** Acrescente text-center na classe de cada coluna.
- **Estudar no PDF:** Cap. 8.3 (text-center)
- **Pronto quando:** Imagens e nomes centralizados.

#### T090 · Atualizar o cartão da sarah para o da Sarah
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T003

- **O que fazer:** Depois da troca, mude o nome, o link e o ícone do cartão 1 (sarah.html e icons/Sarah_favicon.png), inclusive no hero e na navbar.
- **Pronto quando:** Nenhuma menção à sarah na home.

## M5 · Estilo final

*Cores do tema, cartões com borda arredondada e sombra, efeito hover/foco e barra colorida nos títulos.*

#### T091 · Trocar width e height das imagens por CSS
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T090

- **O que fazer:** Apague os atributos width="…" e height="…" das <img>. Quem controla o tamanho agora é o CSS (img { max-width: 100%; height: auto; }) e as colunas.
- **Estudar no PDF:** Cap. 7.3
- **Estudar fora do PDF:** [PDF F17: Responsive web design basics (web.dev)](https://web.dev/articles/responsive-web-design-basics)
- **Pronto quando:** Nenhuma <img> com width/height.

#### T092 · Aplicar class="titulo" em todos os h2 das seções
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T091

- **O que fazer:** Acrescente class="titulo" nos h2. A barra colorida antes do título vem do CSS (::before).
- **Estudar no PDF:** Cap. 6.3
- **Pronto quando:** Barra colorida antes de cada título.

#### T093 · Aplicar class="cartao" nas caixas de conteúdo
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T092

- **O que fazer:** Coloque <div class="cartao"> em volta de cada item que virou cartão (curiosidades, lugares, integrantes).
- **Estudar no PDF:** Cap. 3.4
- **Pronto quando:** Cartões com canto redondo e sombra.

#### T094 · Aplicar class="foto" nas imagens das galerias
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T093

- **O que fazer:** Use <figure class="foto"><img …></figure> para foto sem link e <a class="foto" href="…"><img …></a> para foto com link.
- **Estudar no PDF:** Cap. 3.4 e 6.1
- **Pronto quando:** Fotos arredondadas, com sombra e hover.

#### T095 · Alternar o fundo das seções com class="secao secao-alt"
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T094

- **O que fazer:** Use <section class="secao"> e, de duas em duas seções, <section class="secao secao-alt"> para alternar o fundo.
- **Estudar no PDF:** Cap. 1.4 (várias classes no mesmo elemento)
- **Pronto quando:** Fundos alternando.

#### T096 · Testar hover e foco pelo teclado
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T095

- **O que fazer:** Passe o mouse nos cartões e fotos e depois aperte Tab várias vezes. Todo link deve mostrar um destaque ao receber foco.
- **Estudar no PDF:** Cap. 6.1
- **Estudar fora do PDF:** [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/)
- **Pronto quando:** Hover e foco visíveis.

#### T097 · Conferir as cores do tema na página inteira
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T096

- **O que fazer:** Olhe navbar, hero, títulos, links e rodapé: tudo na cor azul-marinho e legível.
- **Estudar no PDF:** Cap. 2.1
- **Estudar fora do PDF:** [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/)
- **Pronto quando:** Visual coerente com o tema.

#### T098 · Commit do marco M5
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T097

- **O que fazer:** git add . e git commit -m "M5 Home: estilo final".
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Commit criado.

## M6 · Revisão e entrega v3

*HTML validado, nada perdido, testado em celular/tablet/PC, Pull Request aprovado e versão v3 marcada.*

#### T099 · Validar index.html no validador HTML do W3C
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~30 min · **Depois de:** T098

- **O que fazer:** Abra o validador, escolha "Validate by File Upload" ou "Direct Input" e envie o arquivo. Corrija cada erro listado (tag aberta sem fechar, atributo errado).
- **Estudar fora do PDF:** [Validador de HTML do W3C](https://validator.w3.org/); [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Sem erros (avisos podem ficar).

#### T100 · Comparar a contagem de imagens e links com a do M1
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T099

- **O que fazer:** Repita o Ctrl+F do M1. Tem de dar 4 imagens e os 5 links do original (a navbar e o rodapé acrescentam links novos: confira só os do conteúdo).
- **Pronto quando:** Números batem.

#### T101 · Ler texto novo x texto original lado a lado
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T100

- **O que fazer:** Abra o HTML do M1 (git show) e a página nova e confira se todos os textos continuam lá, com as mesmas palavras.
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Nenhum texto perdido ou alterado.

#### T102 · Testar em 360, 768 e 1200 px no DevTools
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T101

- **O que fazer:** No Chrome aperte F12 e clique no ícone de celular/tablet. Teste as 3 larguras. Nenhuma rolagem horizontal pode aparecer.
- **Estudar no PDF:** Cap. 7.2 e 8.2 (breakpoints md = 768 px)
- **Estudar fora do PDF:** [Chrome DevTools: device mode](https://developer.chrome.com/docs/devtools/device-mode); [Bootstrap 5.3: Grid system](https://getbootstrap.com/docs/5.3/layout/grid/)
- **Pronto quando:** 3 larguras sem rolagem horizontal e com layout certo.

#### T103 · Clicar em todos os links externos da página
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T102

- **O que fazer:** Abra cada link externo numa nova aba e anote os que não abrem. Entregue a lista para a tarefa "Consolidar os links externos".
- **Pronto quando:** Lista de links quebrados (pode ser vazia).

#### T104 · Abrir o Pull Request da branch
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T103

- **O que fazer:** git push -u origin pagina-home; no GitHub clique em "Compare & pull request", descreva o que mudou e peça revisão de outra pessoa.
- **Estudar fora do PDF:** [GitHub Docs: Creating a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request); [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Pull Request aberto com revisor.

#### T105 · Revisar o Pull Request de outra pessoa (checklist)
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T104

- **O que fazer:** Quem revisa abre a aba "Files changed", segue o checklist e comenta ou aprova. Só depois o autor faz o merge.
- **Estudar fora do PDF:** [GitHub Docs: Creating a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)
- **Pronto quando:** PR aprovado por alguém que não é o autor.

#### T106 · Fazer o merge na main e atualizar o status no Excel
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T105

- **O que fazer:** Com o PR aprovado, clique em "Merge pull request". Depois marque as tarefas da página como Concluída nesta planilha.
- **Estudar fora do PDF:** [GitHub Docs: Creating a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)
- **Pronto quando:** Página na main e status atualizado.

## Fontes desta frente

- [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2) (aberta em 17/11/2026)
- [GitHub Docs: Hello World](https://docs.github.com/en/get-started/start-your-journey/hello-world) (aberta em 17/11/2026)
- [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements) (aberta em 17/11/2026)
- [Bootstrap 5.3: Get started](https://getbootstrap.com/docs/5.3/getting-started/introduction/) (aberta em 17/11/2026)
- [Chrome DevTools: device mode](https://developer.chrome.com/docs/devtools/device-mode) (aberta em 17/11/2026)
- [Validador de HTML do W3C](https://validator.w3.org/) (aberta em 17/11/2026)
- [Bootstrap 5.3: Grid system](https://getbootstrap.com/docs/5.3/layout/grid/) (aberta em 17/11/2026)
- PDF F17: [Responsive web design basics (web.dev)](https://web.dev/articles/responsive-web-design-basics) (citada na lista de fontes do PDF; não reaberta nesta sessão)
- [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/) (aberta em 17/11/2026)
- [GitHub Docs: Creating a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) (aberta em 17/11/2026)
