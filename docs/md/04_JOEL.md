# Guia 4 de 6 · Página do Joel

Passo a passo para sair do estado inicial de `joel.html` e chegar à v3 (tema verde). Responsável sugerido pela página: **Joel**. Faça um marco por vez e dê commit ao fim de cada um.

> Os IDs (T001...) são os mesmos da planilha `Controle_de_Tarefas_Grupo_1C.xlsx`. Marque o status por lá. Responsáveis e prazos marcados como "sugerido" ou "A definir" podem ser ajustados pelo grupo.

**53 tarefas** nesta frente.

## Marcos desta frente

| Marco | Nome | Tarefas | O que está pronto |
|---|---|---|---|
| M1 | V1 no repositório | 3 | O HTML original está no GitHub, cada integrante tem o repositório no computador e cada página tem uma branch. |
| M2 | Bootstrap e CSS ligados | 8 | Cada página carrega Bootstrap, estilo.css e o tema de cor. Visual ainda simples, mas a base está pronta. |
| M3 | Casca padronizada | 8 | Navbar, faixa de abertura (hero) com botões e rodapé iguais nas 5 páginas. |
| M4 | Seções em grade | 18 | O conteúdo está organizado em seções com container, row e col (Bootstrap) e em cartões. |
| M5 | Estilo final | 8 | Cores do tema, cartões com borda arredondada e sombra, efeito hover/foco e barra colorida nos títulos. |
| M6 | Revisão e entrega v3 | 8 | HTML validado, nada perdido, testado em celular/tablet/PC, Pull Request aprovado e versão v3 marcada. |

## Como estudar

- "PDF" é o material *O Cardápio do Navegador: CSS do Seletor ao Bootstrap* (capítulos indicados em cada tarefa).
- "Fora do PDF" são páginas oficiais; abra só a parte do assunto da tarefa, não precisa ler o site inteiro.

## M1 · V1 no repositório

*O HTML original está no GitHub, cada integrante tem o repositório no computador e cada página tem uma branch.*

#### T164 · Criar a branch pagina-joel
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T002

- **O que fazer:** No terminal, dentro da pasta do repositório: "git switch -c pagina-joel". A branch é uma cópia de trabalho só sua; a main fica protegida.
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2); [GitHub Docs: Hello World](https://docs.github.com/en/get-started/start-your-journey/hello-world)
- **Pronto quando:** "git branch" mostra pagina-joel com um asterisco.

#### T165 · Abrir joel.html no navegador e listar o que aparece
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T164

- **O que fazer:** Abra o arquivo e escreva uma lista curta: título, textos, fotos, listas e links que você vê. Isso vira seu mapa para não perder nada.
- **Estudar no PDF:** Cap. 1.1 (HTML descreve o conteúdo)
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Lista escrita (pode ser no bloco de notas).

#### T166 · Contar as imagens e os links de joel.html
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T165

- **O que fazer:** Abra o arquivo no editor, use Ctrl+F e procure "<img" e "<a ". Anote os números. No original: 15 imagens e 13 links. No fim, a V3 tem de ter os mesmos.
- **Pronto quando:** Anotado: 15 imagens e 13 links.

## M2 · Bootstrap e CSS ligados

*Cada página carrega Bootstrap, estilo.css e o tema de cor. Visual ainda simples, mas a base está pronta.*

#### T167 · Corrigir lang="bt-br" para lang="pt-br" na tag <html>
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T166

- **O que fazer:** No original está escrito "bt-br" (erro de digitação). O "pt-br" diz ao navegador e ao leitor de tela que o texto é português do Brasil.
- **Estudar no PDF:** Cap. 8.1 (exemplo de <html lang="pt-br">)
- **Pronto quando:** <html lang="pt-br">.

#### T168 · Conferir a meta viewport
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T167

- **O que fazer:** Confirme a linha <meta name="viewport" content="width=device-width, initial-scale=1.0"> no <head>. Ela faz o celular usar a largura real da tela.
- **Estudar no PDF:** Cap. 7.1
- **Pronto quando:** A linha existe no <head>.

#### T169 · Ligar o Bootstrap 5.3.9 no <head> de joel.html
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T168

- **O que fazer:** Copie do modelo/head.html (ou do site oficial) a linha <link ... bootstrap.min.css>. Sem internet o Bootstrap não carrega.
- **Estudar no PDF:** Cap. 8.1 (instalar pelo CDN)
- **Estudar fora do PDF:** [Bootstrap 5.3: Get started](https://getbootstrap.com/docs/5.3/getting-started/introduction/)
- **Pronto quando:** Ao recarregar, a fonte e os espaços do texto mudam um pouco.

#### T170 · Ligar css/estilo.css depois do Bootstrap
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T169

- **O que fazer:** Acrescente <link rel="stylesheet" href="css/estilo.css"> logo abaixo da linha do Bootstrap. A ordem importa: quem vem por último vence em caso de empate.
- **Estudar no PDF:** Cap. 1.2 (CSS externo) e 1.4 (cascata)
- **Pronto quando:** Fonte do body mudou para Segoe UI/Arial.

#### T171 · Ligar css/tema-joel.css depois do estilo.css
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T170

- **O que fazer:** Acrescente <link rel="stylesheet" href="css/tema-joel.css"> como terceira linha de CSS.
- **Estudar no PDF:** Cap. 1.2 e 1.4
- **Pronto quando:** Linha adicionada.

#### T172 · Colocar class="tema-joel" na tag <body>
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T171

- **O que fazer:** Troque <body> por <body class="tema-joel">. O CSS do tema só age em páginas que tenham essa classe.
- **Estudar no PDF:** Cap. 1.3 (seletor de classe)
- **Pronto quando:** Fundo da página na cor do tema (verde).

#### T173 · Testar: recarregar e ver se o fundo e a fonte mudaram
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T172

- **O que fazer:** Abra com F5. Se nada mudou, abra o DevTools (F12), aba Console/Network, e veja qual arquivo deu erro 404 (caminho errado).
- **Estudar fora do PDF:** [Chrome DevTools: device mode](https://developer.chrome.com/docs/devtools/device-mode)
- **Pronto quando:** Fundo e fonte corretos, sem erro 404.

#### T174 · Commit do marco M2
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T173

- **O que fazer:** git add joel.html e git commit -m "M2 Joel: Bootstrap e CSS ligados". Um commit por marco facilita desfazer se algo der errado.
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Commit criado.

## M3 · Casca padronizada

*Navbar, faixa de abertura (hero) com botões e rodapé iguais nas 5 páginas.*

#### T175 · Colar a navbar no início do <body> de joel.html
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T174

- **O que fazer:** Copie o bloco de modelo/navbar.html e cole logo depois de <body>. A navbar é a mesma em todas as páginas.
- **Estudar no PDF:** Cap. 4.2
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Barra de navegação aparece no topo.

#### T176 · Marcar o link da própria página como ativo
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T175

- **O que fazer:** No bloco da navbar, no link desta página, escreva class="ativo" aria-current="page". A aba ativa fica branca e mostra onde você está.
- **Estudar no PDF:** Cap. 6.1 (estado visual)
- **Pronto quando:** Só um link está destacado.

#### T177 · Testar os 5 links da navbar
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T176

- **O que fazer:** Clique em cada link. Todos devem abrir a página certa, na mesma aba.
- **Pronto quando:** 5 links funcionando.

#### T178 · Criar o hero com o título "Apresentação Pessoal - Joel Gracek"
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T177

- **O que fazer:** Depois da navbar, crie <section class="hero"><div class="container"><h1>…</h1></div></section> e mova para lá o título atual da página.
- **Estudar no PDF:** Cap. 8.2 (container) e 1.3
- **Estudar fora do PDF:** [Bootstrap 5.3: Grid system](https://getbootstrap.com/docs/5.3/layout/grid/)
- **Pronto quando:** Faixa colorida com o título dentro.

#### T179 · Montar o rótulo "TÓPICOS DA PÁGINA" e os botões de atalho
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~25 min · **Depois de:** T178

- **O que fazer:** Dentro do hero: <h2 class="rotulo">TÓPICOS DA PÁGINA</h2> e uma <ul class="atalhos"> com um <li><a class="btn btn-primary" href="..."> por botão: Voltar para a Página inicial, Sobre mim, Curiosidades sobre mim, Lugares que visitei e Lugares que quero visitar. Os links internos usam #id da seção.
- **Estudar no PDF:** Cap. 8.3 (btn btn-primary)
- **Estudar fora do PDF:** [Bootstrap 5.3: Get started](https://getbootstrap.com/docs/5.3/getting-started/introduction/)
- **Pronto quando:** Fileira de botões brancos abaixo do título.

#### T180 · Colar o rodapé antes de </body>
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T179

- **O que fazer:** Copie modelo/rodape.html e cole logo antes de </body>, depois de </main> (que será criado no M4).
- **Estudar no PDF:** Cap. 8.2
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Rodapé aparece no fim da página.

#### T181 · Testar o link "Volte ao topo da página!"
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T180

- **O que fazer:** Clique no link do rodapé: a página deve subir até a navbar (o id="topo" está no <header>).
- **Pronto quando:** Página sobe até o topo.

#### T182 · Commit do marco M3
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T181

- **O que fazer:** git add joel.html e git commit -m "M3 Joel: navbar, hero e rodapé".
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Commit criado.

## M4 · Seções em grade

*O conteúdo está organizado em seções com container, row e col (Bootstrap) e em cartões.*

#### T183 · Envolver todo o conteúdo entre o hero e o rodapé com <main>
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T182

- **O que fazer:** <main> marca o conteúdo principal da página. Ele fica entre </header> e <footer>.
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** <main> abre depois do hero e fecha antes do rodapé.

#### T184 · Remover as <hr> (linhas horizontais) do conteúdo
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T183

- **O que fazer:** As linhas separavam as partes no HTML antigo. Com seções coloridas elas não são mais necessárias; apague as tags <hr>.
- **Estudar no PDF:** Cap. 3.1
- **Pronto quando:** Nenhuma <hr> no arquivo.

#### T185 · Remover a <ul> do link "Voltar para a Página inicial"
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T184

- **O que fazer:** No original o link está numa lista de 1 item. Agora ele é o primeiro botão do hero: copie o link (mantendo o <strong>) para lá e apague a <ul>.
- **Estudar no PDF:** Cap. 8.3
- **Pronto quando:** Link só aparece no hero.

#### T186 · Criar <section id="sobremim"> com o h2 "Sobre mim"
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T185

- **O que fazer:** O id="sobremim" é o destino do botão "Sobre mim" do hero.
- **Estudar no PDF:** Cap. 8.2
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Seção criada com o h2.

#### T187 · Dividir "Sobre mim" em texto (col-12 col-lg-7) e fotos (col-12 col-lg-5)
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T186

- **O que fazer:** Dentro da seção crie <div class="row g-3"> e as duas colunas. Texto "Opa! Meu nome é Joel Gracek…" na primeira.
- **Estudar no PDF:** Cap. 8.2
- **Estudar fora do PDF:** [Bootstrap 5.3: Grid system](https://getbootstrap.com/docs/5.3/layout/grid/)
- **Pronto quando:** Texto e fotos lado a lado a partir de 992 px.

#### T188 · Colocar foto_joel_1 e vila_moraes em col-6 dentro da coluna das fotos
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T187

- **O que fazer:** Outra <div class="row g-3"> dentro da coluna das fotos com duas <div class="col-6">, cada uma com <figure class="foto"><img …></figure>.
- **Estudar no PDF:** Cap. 8.2
- **Pronto quando:** Duas fotos lado a lado.

#### T189 · Mover o parágrafo "Sou cristão…(dica: clique nas imagens :D)" para linha própria
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T188

- **O que fazer:** Abaixo das duas colunas, <div class="row g-3 mt-3"> e <div class="col-12">com o parágrafo.
- **Estudar no PDF:** Cap. 8.3 (mt-3)
- **Pronto quando:** Parágrafo ocupa a largura toda.

#### T190 · Colocar as 4 imagens com link (Crash, Marvel, O Velho e o Mar, Parque) em col-6 col-md-3
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T189

- **O que fazer:** Cada uma vira <div class="col-6 col-md-3"><a class="foto" href="…" target="_blank" rel="noopener"><img …></a></div>. Mantenha os mesmos links.
- **Estudar no PDF:** Cap. 8.2
- **Pronto quando:** 4 imagens clicáveis em 2 (celular) ou 4 (tablet em diante) por linha.

#### T191 · Criar <section id="curiosidades"> com o h2 "Curiosidades sobre mim"
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T190

- **O que fazer:** Seção nova com container e o h2. É o destino do botão "Curiosidades sobre mim".
- **Estudar no PDF:** Cap. 8.2
- **Pronto quando:** Seção criada.

#### T192 · Separar a lista numerada I e II em dois cartões (col-12 col-md-6)
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~25 min · **Depois de:** T191

- **O que fazer:** No original é uma só <ol type="I"> com 2 itens. Crie 2 cartões, cada um com <ol type="I" start="1"> e <ol type="I" start="2"> com 1 item. A numeração romana continua certa.
- **Estudar no PDF:** Cap. 8.2
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Dois cartões: "I." e "II.".

#### T193 · Tirar os <p> de dentro da <ol> e levar as fotos das calopsitas para o cartão I
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T192

- **O que fazer:** O original põe <p> entre os <li> (HTML inválido). Mova as imagens bella.jpeg e ovos_calopsitas.png para dentro do cartão I, depois do texto.
- **Estudar fora do PDF:** [Validador de HTML do W3C](https://validator.w3.org/)
- **Pronto quando:** Nenhum <p> dentro de <ol>.

#### T194 · Levar o banner do canal (link para o YouTube) para o cartão II
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T193

- **O que fazer:** Mova <a href="https://www.youtube.com/@JoelGG4610"><img banner_canal.jpg></a> para dentro do cartão II, abaixo do texto.
- **Pronto quando:** Banner clicável dentro do cartão II.

#### T195 · Criar <section id="visitei"> com o h2 "Lugares que visitei" e uma row g-3
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T194

- **O que fazer:** Seção com container, h2 e <div class="row g-3"> para os cartões.
- **Estudar no PDF:** Cap. 8.2
- **Pronto quando:** Seção criada.

#### T196 · Transformar cada <li> (Santos, Balneário Camboriú, Beto Carrero) em cartão col-12 col-md-6 col-lg-4
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~25 min · **Depois de:** T195

- **O que fazer:** Troque <ul type="circle"> por row e cada <li> por <div class="col-12 col-md-6 col-lg-4"><div class="cartao">…</div></div>. As bolinhas somem.
- **Estudar no PDF:** Cap. 8.2
- **Estudar fora do PDF:** [Bootstrap 5.3: Grid system](https://getbootstrap.com/docs/5.3/layout/grid/)
- **Pronto quando:** 3 cartões lado a lado no PC.

#### T197 · Dentro do cartão: título em <h3><a> e foto em <a class="foto">; remover os <br>
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T196

- **O que fazer:** O original tinha <a>texto<br><br><img><br><br></a>. Agora: <h3><a href="…">Santos - SP</a></h3> e <a class="foto" href="…"><img …></a>, os dois com o mesmo endereço. Sem <br>.
- **Estudar no PDF:** Cap. 3.1
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Cartão com título e foto, ambos clicáveis.

#### T198 · Repetir para "Lugares que quero visitar" (Foz do Iguaçu, Suíça, Coliseu) em <section id="visitar">
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T197

- **O que fazer:** Mesma estrutura da seção anterior, com id="visitar".
- **Estudar no PDF:** Cap. 8.2
- **Pronto quando:** 3 cartões na seção nova.

#### T199 · Garantir target="_blank" rel="noopener" nos links externos
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T198

- **O que fazer:** Os links que abrem em outra aba precisam de rel="noopener": evita que a página aberta controle a sua.
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Todos os links externos com os 2 atributos.

#### T200 · Decidir sobre o link do Coliseu (site de ingressos)
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T199 · *opcional*

- **O que fazer:** O link aponta para um site que parece revenda de ingressos. Combine com o grupo: manter ou trocar por uma página informativa (ex.: Wikipédia).
- **Pronto quando:** Decisão registrada.

## M5 · Estilo final

*Cores do tema, cartões com borda arredondada e sombra, efeito hover/foco e barra colorida nos títulos.*

#### T201 · Trocar width e height das imagens por CSS
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T200

- **O que fazer:** Apague os atributos width="…" e height="…" das <img>. Quem controla o tamanho agora é o CSS (img { max-width: 100%; height: auto; }) e as colunas.
- **Estudar no PDF:** Cap. 7.3
- **Estudar fora do PDF:** [PDF F17: Responsive web design basics (web.dev)](https://web.dev/articles/responsive-web-design-basics)
- **Pronto quando:** Nenhuma <img> com width/height.

#### T202 · Aplicar class="titulo" em todos os h2 das seções
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T201

- **O que fazer:** Acrescente class="titulo" nos h2. A barra colorida antes do título vem do CSS (::before).
- **Estudar no PDF:** Cap. 6.3
- **Pronto quando:** Barra colorida antes de cada título.

#### T203 · Aplicar class="cartao" nas caixas de conteúdo
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T202

- **O que fazer:** Coloque <div class="cartao"> em volta de cada item que virou cartão (curiosidades, lugares, integrantes).
- **Estudar no PDF:** Cap. 3.4
- **Pronto quando:** Cartões com canto redondo e sombra.

#### T204 · Aplicar class="foto" nas imagens das galerias
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T203

- **O que fazer:** Use <figure class="foto"><img …></figure> para foto sem link e <a class="foto" href="…"><img …></a> para foto com link.
- **Estudar no PDF:** Cap. 3.4 e 6.1
- **Pronto quando:** Fotos arredondadas, com sombra e hover.

#### T205 · Alternar o fundo das seções com class="secao secao-alt"
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T204

- **O que fazer:** Use <section class="secao"> e, de duas em duas seções, <section class="secao secao-alt"> para alternar o fundo.
- **Estudar no PDF:** Cap. 1.4 (várias classes no mesmo elemento)
- **Pronto quando:** Fundos alternando.

#### T206 · Testar hover e foco pelo teclado
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T205

- **O que fazer:** Passe o mouse nos cartões e fotos e depois aperte Tab várias vezes. Todo link deve mostrar um destaque ao receber foco.
- **Estudar no PDF:** Cap. 6.1
- **Estudar fora do PDF:** [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/)
- **Pronto quando:** Hover e foco visíveis.

#### T207 · Conferir as cores do tema na página inteira
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T206

- **O que fazer:** Olhe navbar, hero, títulos, links e rodapé: tudo na cor verde e legível.
- **Estudar no PDF:** Cap. 2.1
- **Estudar fora do PDF:** [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/)
- **Pronto quando:** Visual coerente com o tema.

#### T208 · Commit do marco M5
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T207

- **O que fazer:** git add . e git commit -m "M5 Joel: estilo final".
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Commit criado.

## M6 · Revisão e entrega v3

*HTML validado, nada perdido, testado em celular/tablet/PC, Pull Request aprovado e versão v3 marcada.*

#### T209 · Validar joel.html no validador HTML do W3C
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~30 min · **Depois de:** T208

- **O que fazer:** Abra o validador, escolha "Validate by File Upload" ou "Direct Input" e envie o arquivo. Corrija cada erro listado (tag aberta sem fechar, atributo errado).
- **Estudar fora do PDF:** [Validador de HTML do W3C](https://validator.w3.org/); [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Sem erros (avisos podem ficar).

#### T210 · Comparar a contagem de imagens e links com a do M1
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T209

- **O que fazer:** Repita o Ctrl+F do M1. Tem de dar 15 imagens e os 13 links do original (a navbar e o rodapé acrescentam links novos: confira só os do conteúdo).
- **Pronto quando:** Números batem.

#### T211 · Ler texto novo x texto original lado a lado
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T210

- **O que fazer:** Abra o HTML do M1 (git show) e a página nova e confira se todos os textos continuam lá, com as mesmas palavras.
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Nenhum texto perdido ou alterado.

#### T212 · Testar em 360, 768 e 1200 px no DevTools
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T211

- **O que fazer:** No Chrome aperte F12 e clique no ícone de celular/tablet. Teste as 3 larguras. Nenhuma rolagem horizontal pode aparecer.
- **Estudar no PDF:** Cap. 7.2 e 8.2 (breakpoints md = 768 px)
- **Estudar fora do PDF:** [Chrome DevTools: device mode](https://developer.chrome.com/docs/devtools/device-mode); [Bootstrap 5.3: Grid system](https://getbootstrap.com/docs/5.3/layout/grid/)
- **Pronto quando:** 3 larguras sem rolagem horizontal e com layout certo.

#### T213 · Clicar em todos os links externos da página
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T212

- **O que fazer:** Abra cada link externo numa nova aba e anote os que não abrem. Entregue a lista para a tarefa "Consolidar os links externos".
- **Pronto quando:** Lista de links quebrados (pode ser vazia).

#### T214 · Abrir o Pull Request da branch
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T213

- **O que fazer:** git push -u origin pagina-joel; no GitHub clique em "Compare & pull request", descreva o que mudou e peça revisão de outra pessoa.
- **Estudar fora do PDF:** [GitHub Docs: Creating a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request); [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Pull Request aberto com revisor.

#### T215 · Revisar o Pull Request de outra pessoa (checklist)
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T214

- **O que fazer:** Quem revisa abre a aba "Files changed", segue o checklist e comenta ou aprova. Só depois o autor faz o merge.
- **Estudar fora do PDF:** [GitHub Docs: Creating a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)
- **Pronto quando:** PR aprovado por alguém que não é o autor.

#### T216 · Fazer o merge na main e atualizar o status no Excel
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T215

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
- [Validador de HTML do W3C](https://validator.w3.org/) (aberta em 17/11/2026)
- PDF F17: [Responsive web design basics (web.dev)](https://web.dev/articles/responsive-web-design-basics) (citada na lista de fontes do PDF; não reaberta nesta sessão)
- [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/) (aberta em 17/11/2026)
- [GitHub Docs: Creating a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) (aberta em 17/11/2026)
