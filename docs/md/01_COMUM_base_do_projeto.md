# Guia 1 de 6 · Base comum do projeto

Tarefas que valem para o grupo todo: repositório, V1, base de CSS, navbar, hero, rodapé e classes compartilhadas. As três primeiras (T001 a T003) foram cadastradas por você; as demais são sugestões.

> Os IDs (T001...) são os mesmos da planilha `Controle_de_Tarefas_Grupo_1C.xlsx`. Marque o status por lá. Responsáveis e prazos marcados como "sugerido" ou "A definir" podem ser ajustados pelo grupo.

**59 tarefas** nesta frente.

## Marcos desta frente

| Marco | Nome | Tarefas | O que está pronto |
|---|---|---|---|
| M1 | V1 no repositório | 23 | O HTML original está no GitHub, cada integrante tem o repositório no computador e cada página tem uma branch. |
| M2 | Bootstrap e CSS ligados | 11 | Cada página carrega Bootstrap, estilo.css e o tema de cor. Visual ainda simples, mas a base está pronta. |
| M3 | Casca padronizada | 12 | Navbar, faixa de abertura (hero) com botões e rodapé iguais nas 5 páginas. |
| M4 | Seções em grade | 1 | O conteúdo está organizado em seções com container, row e col (Bootstrap) e em cartões. |
| M5 | Estilo final | 6 | Cores do tema, cartões com borda arredondada e sombra, efeito hover/foco e barra colorida nos títulos. |
| M6 | Revisão e entrega v3 | 6 | HTML validado, nada perdido, testado em celular/tablet/PC, Pull Request aprovado e versão v3 marcada. |

## Como estudar

- "PDF" é o material *O Cardápio do Navegador: CSS do Seletor ao Bootstrap* (capítulos indicados em cada tarefa).
- "Fora do PDF" são páginas oficiais; abra só a parte do assunto da tarefa, não precisa ler o site inteiro.

## M1 · V1 no repositório

*O HTML original está no GitHub, cada integrante tem o repositório no computador e cada página tem uma branch.*

#### T001 · Criar repositório Github
**Quem:** Sarah (informado) · **Prazo:** 17/11/2026 · **Status:** Concluída · **Esforço:** ~15 min

- **O que fazer:** Criar o repositório do grupo no GitHub (nome do projeto, visibilidade e README inicial).
- **Estudar fora do PDF:** [GitHub Docs: Hello World](https://docs.github.com/en/get-started/start-your-journey/hello-world)
- **Pronto quando:** O repositório existe e o grupo consegue abrir o endereço.

#### T002 · Adicionar V1 das páginas iniciais
**Quem:** Joel (informado) · **Prazo:** 17/11/2026 · **Status:** Não Iniciada · **Esforço:** ~30 min · **Depois de:** T001

- **O que fazer:** Colocar no repositório as páginas do jeito que estão hoje (estado inicial), sem mudar nada. É a "foto" do ponto de partida.
- **Estudar no PDF:** Cap. 1.1 (o que é HTML e o que é CSS)
- **Estudar fora do PDF:** [GitHub Docs: Hello World](https://docs.github.com/en/get-started/start-your-journey/hello-world); [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** As 5 páginas, images/ e icons/ aparecem no GitHub.

#### T003 · Substituir página da sarah pela página da Sarah
**Quem:** Sarah (informado) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~60 min · **Depois de:** T002

- **O que fazer:** A página da sarah sai e a da Sarah entra no lugar, com todos os links da navbar, da home e do rodapé atualizados. Os passos pequenos estão na frente "Sarah", marco M1.
- **Estudar no PDF:** Cap. 1.1 e 8.2 (ver o modelo que será mantido)
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Nenhuma página aponta para sarah.html e a página da Sarah abre sem imagem quebrada.

#### T004 · Convidar Joel, Luiz e Laís como colaboradores do repositório
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T001

- **O que fazer:** No repositório, abra Settings > Collaborators e convide os três pelo nome de usuário do GitHub. Cada um aceita o convite pelo e-mail.
- **Estudar fora do PDF:** [GitHub Docs: Hello World](https://docs.github.com/en/get-started/start-your-journey/hello-world)
- **Pronto quando:** Os 4 integrantes conseguem enviar alterações ao repositório.

#### T005 · Escrever o README.md do projeto
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T004

- **O que fazer:** Abra o README.md e escreva: nome do projeto, quem são os integrantes e como abrir o site (abrir files/index.html no navegador).
- **Estudar no PDF:** Cap. 1.1
- **Estudar fora do PDF:** [GitHub Docs: Hello World](https://docs.github.com/en/get-started/start-your-journey/hello-world)
- **Pronto quando:** O README aparece na página inicial do repositório.

#### T006 · Combinar a regra de trabalho em grupo
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T005

- **O que fazer:** Escrever no README: "1 branch por página; só entra na main com Pull Request revisado por outra pessoa". Evita sobrescrever o trabalho dos outros.
- **Estudar fora do PDF:** [GitHub Docs: Creating a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request); [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** A regra está no README e todos leram.

#### T007 · Criar o .gitignore
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T006 · *opcional*

- **O que fazer:** Criar um arquivo .gitignore com os arquivos que não devem subir (por exemplo .DS_Store e Thumbs.db). Evita sujeira no repositório.
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Arquivos de sistema não aparecem mais em "git status".

#### T008 · Clonar o repositório no computador (Sarah)
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T001

- **O que fazer:** Na página do repositório clique em Code, copie o endereço e rode "git clone <endereço>" numa pasta sua. Isso baixa uma cópia para trabalhar.
- **Estudar fora do PDF:** [GitHub Docs: Hello World](https://docs.github.com/en/get-started/start-your-journey/hello-world); [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** A pasta do projeto existe no computador.

#### T009 · Clonar o repositório no computador (Joel)
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T001

- **O que fazer:** Na página do repositório clique em Code, copie o endereço e rode "git clone <endereço>" numa pasta sua. Isso baixa uma cópia para trabalhar.
- **Estudar fora do PDF:** [GitHub Docs: Hello World](https://docs.github.com/en/get-started/start-your-journey/hello-world); [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** A pasta do projeto existe no computador.

#### T010 · Clonar o repositório no computador (Luiz)
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T001

- **O que fazer:** Na página do repositório clique em Code, copie o endereço e rode "git clone <endereço>" numa pasta sua. Isso baixa uma cópia para trabalhar.
- **Estudar fora do PDF:** [GitHub Docs: Hello World](https://docs.github.com/en/get-started/start-your-journey/hello-world); [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** A pasta do projeto existe no computador.

#### T011 · Clonar o repositório no computador (Laís)
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T001

- **O que fazer:** Na página do repositório clique em Code, copie o endereço e rode "git clone <endereço>" numa pasta sua. Isso baixa uma cópia para trabalhar.
- **Estudar fora do PDF:** [GitHub Docs: Hello World](https://docs.github.com/en/get-started/start-your-journey/hello-world); [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** A pasta do projeto existe no computador.

#### T012 · Configurar nome e e-mail do Git (Sarah)
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T011

- **O que fazer:** Rode "git config --global user.name" e "git config --global user.email" com seus dados. Assim cada commit mostra quem fez.
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** "git config --list" mostra seu nome e e-mail.

#### T013 · Configurar nome e e-mail do Git (Joel)
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T012

- **O que fazer:** Rode "git config --global user.name" e "git config --global user.email" com seus dados. Assim cada commit mostra quem fez.
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** "git config --list" mostra seu nome e e-mail.

#### T014 · Configurar nome e e-mail do Git (Luiz)
**Quem:** Luiz (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T013

- **O que fazer:** Rode "git config --global user.name" e "git config --global user.email" com seus dados. Assim cada commit mostra quem fez.
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** "git config --list" mostra seu nome e e-mail.

#### T015 · Configurar nome e e-mail do Git (Laís)
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T014

- **O que fazer:** Rode "git config --global user.name" e "git config --global user.email" com seus dados. Assim cada commit mostra quem fez.
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** "git config --list" mostra seu nome e e-mail.

#### T016 · Copiar a pasta Trabalhos (files, images, icons) para dentro do repositório clonado
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T015 · *passo de T002*

- **O que fazer:** Copie as pastas do estado inicial para dentro da pasta do repositório, mantendo os mesmos nomes (files, images, icons). Não renomeie nada.
- **Estudar no PDF:** Cap. 1.2 (por que os caminhos "images" precisam ser mantidos)
- **Pronto quando:** As 3 pastas estão no repositório com a mesma estrutura do zip original.

#### T017 · Abrir files/index.html a partir do repositório e conferir se as imagens aparecem
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T016 · *passo de T002*

- **O que fazer:** Dê duplo clique em index.html. Se alguma imagem não aparecer, o caminho foi quebrado ao copiar: confira os nomes das pastas.
- **Estudar no PDF:** Cap. 1.1
- **Pronto quando:** Home abre com as 4 imagens e as 4 outras páginas abrem sem imagem quebrada.

#### T018 · Anotar os problemas conhecidos do V1 no README
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T017 · *passo de T002*

- **O que fazer:** Anote o que está errado hoje (ex.: 3 links vazios na home, lang="bt-br" no Joel, falta da meta viewport no Luiz). Serve de lista do que a V3 corrige.
- **Estudar no PDF:** Cap. 7.1 (meta viewport)
- **Pronto quando:** Seção "Problemas do V1" no README.

#### T019 · Registrar a V1 (git add e git commit)
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T018 · *passo de T002*

- **O que fazer:** Rode "git add ." e "git commit -m \"V1: páginas iniciais sem CSS\"". O commit guarda esta versão para sempre; dá para voltar a ela.
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** git log mostra o commit "V1: páginas iniciais sem CSS".

#### T020 · Enviar a V1 para o GitHub (git push)
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T019 · *passo de T002*

- **O que fazer:** Rode "git push". Seu commit sobe para o repositório da nuvem.
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** O commit aparece no GitHub.

#### T021 · Conferir no site do GitHub se as pastas apareceram
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T020 · *passo de T002*

- **O que fazer:** Abra o repositório no navegador e entre em files/. Abra um HTML pelo botão Raw só para confirmar que é o original.
- **Pronto quando:** As 5 páginas estão listadas no GitHub.

#### T022 · Criar a tag v1 (opcional)
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T021 · *opcional* · *passo de T002*

- **O que fazer:** Rode "git tag v1" e "git push --tags". A tag é uma etiqueta que marca esta versão para achar depois.
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** A tag v1 aparece em Releases/Tags.

#### T023 · Avisar o grupo que a V1 está no repositório
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T022 · *passo de T002*

- **O que fazer:** Mande mensagem no grupo com o endereço do repositório e peça para cada um fazer o clone e o "git pull".
- **Pronto quando:** Todos confirmaram que têm a V1.

## M2 · Bootstrap e CSS ligados

*Cada página carrega Bootstrap, estilo.css e o tema de cor. Visual ainda simples, mas a base está pronta.*

#### T024 · Conferir a versão atual do Bootstrap no site oficial
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T023

- **O que fazer:** Abra a página "Get started" do Bootstrap 5.3 e veja a versão mostrada nos links do CDN. Em 17/11/2026 era 5.3.9 (o PDF cita 5.3.8, que ainda funciona).
- **Estudar no PDF:** Cap. 8.1
- **Estudar fora do PDF:** [Bootstrap 5.3: Get started](https://getbootstrap.com/docs/5.3/getting-started/introduction/)
- **Pronto quando:** Versão anotada no README.

#### T025 · Criar a pasta css/ ao lado de files/
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T024

- **O que fazer:** Crie a pasta "css" dentro de Trabalhos, no mesmo nível de files, images e icons. As páginas vão chamá-la com "css/".
- **Estudar no PDF:** Cap. 1.2 (CSS externo)
- **Pronto quando:** Pasta css/ criada.

#### T026 · Criar css/estilo.css com o comentário de cabeçalho
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T025

- **O que fazer:** Crie o arquivo estilo.css e escreva um comentário no topo explicando que é a base comum das páginas. Comentário no CSS fica entre /* e */.
- **Estudar no PDF:** Cap. 1.2 e 1.3 (comentário /* */)
- **Pronto quando:** Arquivo criado e salvo.

#### T027 · Escrever a regra * { box-sizing: border-box; }
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T026

- **O que fazer:** Com isso, padding e borda ficam dentro da largura que você definiu. Evita caixas maiores que o esperado.
- **Estudar no PDF:** Cap. 3.2 (box-sizing)
- **Pronto quando:** Regra escrita em estilo.css.

#### T028 · Escrever a regra do body (fonte, tamanho, altura de linha, margem)
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T027

- **O que fazer:** body { font-family: "Segoe UI", Arial, sans-serif; font-size: 16px; line-height: 1.6; margin: 0; }. Se a primeira fonte faltar, o navegador tenta a próxima.
- **Estudar no PDF:** Cap. 2.2 e 2.3
- **Pronto quando:** Regra escrita; texto das páginas muda de fonte.

#### T029 · Escrever a regra de imagens responsivas
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T028

- **O que fazer:** img { max-width: 100%; height: auto; } faz a foto nunca passar da largura da caixa e manter a proporção.
- **Estudar no PDF:** Cap. 7.3 (caixa final)
- **Estudar fora do PDF:** [Chrome DevTools: device mode](https://developer.chrome.com/docs/devtools/device-mode)
- **Pronto quando:** Regra escrita; fotos grandes não estouram a tela.

#### T030 · Escrever a regra dos títulos h1, h2 e h3
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T029

- **O que fazer:** Defina line-height: 1.25 e tamanhos em rem (h1 2rem, h2 1.6rem, h3 1.25rem). O rem acompanha o tamanho da fonte da página e escala junto.
- **Estudar no PDF:** Cap. 3.3 (rem)
- **Estudar fora do PDF:** [PDF F7: CSS values and units (MDN)](https://developer.mozilla.org/docs/Learn/CSS/Building_blocks/Values_and_units)
- **Pronto quando:** Títulos com tamanho padronizado.

#### T031 · Criar o bloco-modelo do <head> em modelo/head.html
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T030

- **O que fazer:** Guarde num arquivo de apoio as linhas que todas as páginas repetem: meta charset, meta viewport, link do Bootstrap, estilo.css e tema. Cada um copia e só troca o nome do tema.
- **Estudar no PDF:** Cap. 7.1 e 8.1
- **Estudar fora do PDF:** [Bootstrap 5.3: Get started](https://getbootstrap.com/docs/5.3/getting-started/introduction/)
- **Pronto quando:** modelo/head.html com 5 linhas prontas para copiar.

#### T032 · Definir as 5 cores de cada tema (principal, escura, clara, suave, texto)
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T031

- **O que fazer:** Para cada tema escolha 5 códigos HEX. Sugestão do projeto: Joel verde #1B6F36, Luiz vermelho #B92323, Laís rosa #C2185B, sarah/Sarah azul #1F5FBF, home azul-marinho #1F3A5F.
- **Estudar no PDF:** Cap. 2.1 (HEX)
- **Pronto quando:** Tabela de cores no README.

#### T033 · Conferir o contraste das cores no WebAIM
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T032

- **O que fazer:** Cole a cor do texto e a cor do fundo no verificador. Para texto normal o resultado deve ser 4,5:1 ou mais. Se for menor, escureça a cor.
- **Estudar no PDF:** Cap. 2.1 (cores) e 6.1 (acessibilidade)
- **Estudar fora do PDF:** [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/)
- **Pronto quando:** Todos os pares com 4,5:1 ou mais.

#### T034 · Criar os 5 arquivos tema-*.css só com cor de fundo e de texto
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T033

- **O que fazer:** Crie tema-home.css, tema-joel.css, tema-luiz.css, tema-lais.css e tema-sarah.css. Em cada um escreva: body.tema-NOME { background-color: ...; color: ...; }. Só cores, nada de layout.
- **Estudar no PDF:** Cap. 1.3 (seletor de classe) e 2.1
- **Pronto quando:** 5 arquivos criados, cada um com a regra do body.

## M3 · Casca padronizada

*Navbar, faixa de abertura (hero) com botões e rodapé iguais nas 5 páginas.*

#### T035 · Escrever o HTML da navbar em modelo/navbar.html
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T034

- **O que fazer:** Monte um <header id="topo"> com <nav> contendo a marca "Grupo 1ºC" e 5 links (Início, Sarah, Joel, Laís, Luiz). Cada página vai copiar este bloco.
- **Estudar no PDF:** Cap. 4.2 (para entender como será alinhada)
- **Estudar fora do PDF:** [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Bloco pronto com os 5 links e id="topo".

#### T036 · CSS da navbar: espaçamento da barra (.menu-comum)
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~5 min · **Depois de:** T035

- **O que fazer:** .menu-comum { padding: 10px 0; } dá respiro em cima e embaixo.
- **Estudar no PDF:** Cap. 3.1 (padding)
- **Pronto quando:** Regra escrita.

#### T037 · CSS da navbar: alinhar com Flexbox
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T036

- **O que fazer:** .menu-interno { display: flex; flex-wrap: wrap; justify-content: space-between; align-items: center; gap: 8px; }. O pai manda: a marca vai para a esquerda e os links para a direita; se faltar espaço, quebram de linha.
- **Estudar no PDF:** Cap. 4.2 (Flexbox)
- **Estudar fora do PDF:** [PDF F9: flex (MDN)](https://developer.mozilla.org/en/CSS/flex)
- **Pronto quando:** Marca à esquerda e links à direita no PC.

#### T038 · CSS da navbar: aparência dos links
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T037

- **O que fazer:** .menu-links a { display: block; padding: 6px 14px; text-decoration: none; border-bottom: 3px solid transparent; }. A borda transparente reserva o espaço da aba ativa.
- **Estudar no PDF:** Cap. 4.1 (display), 3.1 (borda)
- **Pronto quando:** Links com área de clique maior e sem sublinhado.

#### T039 · CSS da navbar: versão de celular com @media
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T038

- **O que fazer:** @media (max-width: 575px) { ... } centraliza a marca e os links em telas estreitas. A regra só vale quando a tela tem até 575 px.
- **Estudar no PDF:** Cap. 7.2 (media queries)
- **Estudar fora do PDF:** [PDF F16: Beginner's guide to media queries (MDN)](https://developer.mozilla.org/docs/Learn/CSS/CSS_layout/Media_queries); [Chrome DevTools: device mode](https://developer.chrome.com/docs/devtools/device-mode)
- **Pronto quando:** No DevTools em 360 px a navbar fica centralizada.

#### T040 · Escrever o HTML do hero em modelo/hero.html
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T039

- **O que fazer:** Bloco <section class="hero"> com <div class="container">, o <h1>, o rótulo "TÓPICOS DA PÁGINA" e uma <ul class="atalhos"> com links "btn btn-primary".
- **Estudar no PDF:** Cap. 8.2 (container) e 8.3 (btn)
- **Estudar fora do PDF:** [Bootstrap 5.3: Grid system](https://getbootstrap.com/docs/5.3/layout/grid/); [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements)
- **Pronto quando:** Modelo pronto com um exemplo de botão.

#### T041 · CSS do hero (espaço, tamanhos e lista de botões)
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T040

- **O que fazer:** .hero { padding: 3rem 0 2.5rem; } e tamanhos de h1/h2. Em .atalhos use li { display: inline-block; } para os botões ficarem lado a lado e quebrarem de linha.
- **Estudar no PDF:** Cap. 4.1 (inline-block) e 3.3
- **Pronto quando:** Botões lado a lado abaixo do título.

#### T042 · Escrever o HTML do rodapé em modelo/rodape.html
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T041

- **O que fazer:** <footer> com container, uma linha de 2 colunas (col-md-6): à esquerda "Grupo pertencente ao 1ºC", à direita os links das páginas e "Volte ao topo da página!" (href="#topo").
- **Estudar no PDF:** Cap. 8.2
- **Estudar fora do PDF:** [Bootstrap 5.3: Grid system](https://getbootstrap.com/docs/5.3/layout/grid/)
- **Pronto quando:** Modelo pronto.

#### T043 · CSS do rodapé
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T042

- **O que fazer:** .rodape { padding: 2rem 0 1rem; margin-top: 2rem; } e links em lista com li { display: inline-block; }.
- **Estudar no PDF:** Cap. 3.1 e 4.1
- **Pronto quando:** Rodapé com links lado a lado.

#### T044 · Tema: cores da navbar (fundo, link branco, hover e aba ativa)
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~25 min · **Depois de:** T043

- **O que fazer:** Em cada tema-*.css: fundo da navbar na cor principal; links brancos; .menu-comum a:hover com a cor escura; .ativo com fundo branco e texto escuro.
- **Estudar no PDF:** Cap. 2.1 e 6.1 (:hover)
- **Pronto quando:** Navbar colorida em cada tema.

#### T045 · Tema: cores do hero e do botão branco
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~25 min · **Depois de:** T044

- **O que fazer:** .hero com fundo escuro e texto branco. O btn-primary do Bootstrap é azul: dentro do hero, sobrescreva para fundo branco e texto na cor escura do tema.
- **Estudar no PDF:** Cap. 1.4 (quem vence: especificidade e ordem) e 8.3
- **Pronto quando:** Botões brancos legíveis sobre o hero.

#### T046 · Tema: cores do rodapé
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T045

- **O que fazer:** .rodape com fundo escuro, texto e links brancos; no hover, cor suave do tema.
- **Estudar no PDF:** Cap. 2.1
- **Pronto quando:** Rodapé colorido em cada tema.

## M4 · Seções em grade

*O conteúdo está organizado em seções com container, row e col (Bootstrap) e em cartões.*

#### T047 · CSS .secao e .secao-alt (espaçamento e fundo alternado)
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T046

- **O que fazer:** .secao { padding: 2.5rem 0; }. Em cada tema, .secao-alt recebe fundo branco: as seções alternam claro/branco e o olho separa os blocos.
- **Estudar no PDF:** Cap. 3.1 (padding)
- **Pronto quando:** Seções separadas visualmente.

## M5 · Estilo final

*Cores do tema, cartões com borda arredondada e sombra, efeito hover/foco e barra colorida nos títulos.*

#### T048 · CSS .titulo e a barra colorida com ::before
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~25 min · **Depois de:** T047

- **O que fazer:** .titulo::before { content: ""; display: inline-block; width: 10px; height: 1.1em; margin-right: 10px; border-radius: 4px; }. O ::before desenha uma peça que não existe no HTML; o content é obrigatório, mesmo vazio. A cor vem do tema.
- **Estudar no PDF:** Cap. 6.3 (::before e ::after)
- **Estudar fora do PDF:** [PDF F13: Pseudo-classes (MDN)](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Selectors/Pseudo-classes)
- **Pronto quando:** Barra colorida antes dos h2 com class="titulo".

#### T049 · CSS .cartao com cantos arredondados e sombra
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~25 min · **Depois de:** T048

- **O que fazer:** .cartao { height: 100%; padding: 16px; border-radius: 16px; box-shadow: 3px 3px 8px rgba(0,0,0,0.18); }. Os 2 primeiros valores da sombra deslocam, o terceiro desfoca, o último é a cor (com transparência).
- **Estudar no PDF:** Cap. 3.4 (border-radius e box-shadow)
- **Estudar fora do PDF:** [PDF F14: Advanced styling effects (MDN)](https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_boxes/Advanced_box_effects)
- **Pronto quando:** Caixa branca com canto redondo e sombra suave.

#### T050 · CSS .foto (figura com canto redondo e sombra)
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T049

- **O que fazer:** .foto { display: block; margin: 0; border-radius: 12px; box-shadow: ...; } e ".foto img { display: block; width: 100%; border-radius: 12px; }" para a imagem preencher a coluna.
- **Estudar no PDF:** Cap. 3.4 e 7.3
- **Pronto quando:** Fotos com canto redondo preenchendo a coluna.

#### T051 · CSS de hover e foco (:hover e :focus-visible)
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T050

- **O que fazer:** .cartao:hover, .cartao:focus-within e .foto:hover, .foto:focus-visible aumentam a sombra. Quem navega com Tab também vê o destaque.
- **Estudar no PDF:** Cap. 6.1 (pseudoclasses)
- **Estudar fora do PDF:** [PDF F13: Pseudo-classes (MDN)](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Selectors/Pseudo-classes)
- **Pronto quando:** Passar o mouse ou apertar Tab destaca cartão e foto.

#### T052 · CSS de apoio: listas de cartões, legendas e imagens pequenas
**Quem:** Joel (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T051

- **O que fazer:** .lista-cartoes { list-style: none; padding-left: 0; }, .legenda (lista numerada de 1 item), .mini { width: 48%; max-width: 200px; } e .midias para agrupar imagens.
- **Estudar no PDF:** Cap. 3.3 (%) e 7.3
- **Pronto quando:** Listas sem bolinhas dentro de cartões; imagens pequenas lado a lado.

#### T053 · Tema: cores do cartão, da barra do título e do contorno das fotos
**Quem:** Laís (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~30 min · **Depois de:** T052

- **O que fazer:** Em cada tema: .titulo::before com a cor principal; .cartao com borda suave; no hover a borda vira a cor principal; .foto:hover com contorno na cor principal.
- **Estudar no PDF:** Cap. 2.1 e 6.1
- **Pronto quando:** Os 5 temas com as cores aplicadas.

## M6 · Revisão e entrega v3

*HTML validado, nada perdido, testado em celular/tablet/PC, Pull Request aprovado e versão v3 marcada.*

#### T054 · Escrever o checklist de revisão do Pull Request
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T053

- **O que fazer:** Lista curta para o revisor: HTML válido, mesma quantidade de imagens e links do original, texto igual, navbar/rodapé iguais, testado em 360/768/1200 px.
- **Estudar fora do PDF:** [GitHub Docs: Creating a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request); [Validador de HTML do W3C](https://validator.w3.org/)
- **Pronto quando:** Checklist no README.

#### T055 · Testar navbar e rodapé nas 5 páginas depois do último merge
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~20 min · **Depois de:** T054

- **O que fazer:** Abra cada página e clique nos 5 links da navbar e nos do rodapé. Confira se a página ativa está destacada.
- **Estudar no PDF:** Cap. 4.2
- **Pronto quando:** Nenhum link leva a página errada.

#### T056 · Consolidar os links externos quebrados e decidir o que fazer
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~30 min · **Depois de:** T055

- **O que fazer:** Junte as listas de links que cada integrante testou. Para cada link quebrado: trocar por um que funcione ou remover, combinando com o dono da página.
- **Pronto quando:** Lista final de links decididos.

#### T057 · Conferir se o repositório tem só o necessário
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~10 min · **Depois de:** T056

- **O que fazer:** Veja o repositório no GitHub: não deve haver arquivos de teste, rascunhos ou o sarah.html antigo.
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2)
- **Pronto quando:** Repositório limpo.

#### T058 · Marcar a versão v3 e registrar no README
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~15 min · **Depois de:** T057

- **O que fazer:** Rode "git tag v3" e "git push --tags". No README escreva o que mudou da V1 para a V3 (em 5 linhas).
- **Estudar fora do PDF:** [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2); [GitHub Docs: Hello World](https://docs.github.com/en/get-started/start-your-journey/hello-world)
- **Pronto quando:** Tag v3 criada e README atualizado.

#### T059 · Publicar o site no GitHub Pages (opcional)
**Quem:** Sarah (sugerido) · **Prazo:** A definir · **Status:** Não Iniciada · **Esforço:** ~30 min · **Depois de:** T058 · *opcional*

- **O que fazer:** Ative o GitHub Pages nas configurações do repositório para ter um endereço público. Procure "GitHub Pages" em docs.github.com.
- **Pronto quando:** Endereço público abre a home.

## Fontes desta frente

- [GitHub Docs: Hello World](https://docs.github.com/en/get-started/start-your-journey/hello-world) (aberta em 17/11/2026)
- [Pro Git (pt-br), caps. 2 e 3](https://git-scm.com/book/pt-br/v2) (aberta em 17/11/2026)
- [GitHub Docs: Creating a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) (aberta em 17/11/2026)
- [Bootstrap 5.3: Get started](https://getbootstrap.com/docs/5.3/getting-started/introduction/) (aberta em 17/11/2026)
- [Chrome DevTools: device mode](https://developer.chrome.com/docs/devtools/device-mode) (aberta em 17/11/2026)
- PDF F7: [CSS values and units (MDN)](https://developer.mozilla.org/docs/Learn/CSS/Building_blocks/Values_and_units) (citada na lista de fontes do PDF; não reaberta nesta sessão)
- [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/) (aberta em 17/11/2026)
- [MDN: Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Reference/Elements) (aberta em 17/11/2026)
- PDF F9: [flex (MDN)](https://developer.mozilla.org/en/CSS/flex) (citada na lista de fontes do PDF; não reaberta nesta sessão)
- PDF F16: [Beginner's guide to media queries (MDN)](https://developer.mozilla.org/docs/Learn/CSS/CSS_layout/Media_queries) (citada na lista de fontes do PDF; não reaberta nesta sessão)
- [Bootstrap 5.3: Grid system](https://getbootstrap.com/docs/5.3/layout/grid/) (aberta em 17/11/2026)
- PDF F13: [Pseudo-classes (MDN)](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Selectors/Pseudo-classes) (citada na lista de fontes do PDF; não reaberta nesta sessão)
- PDF F14: [Advanced styling effects (MDN)](https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_boxes/Advanced_box_effects) (citada na lista de fontes do PDF; não reaberta nesta sessão)
- [Validador de HTML do W3C](https://validator.w3.org/) (aberta em 17/11/2026)
