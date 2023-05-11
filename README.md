# AluraBooks
Projeto de página feito junto com aulas da Alura sobre CSS focado na responsividade em diferentes tamanhos de tela.
## Índice
* [HTML e CSS](https://github.com/MotiMortal/AluraBooks#html-e-css)
* [Mobile-first](https://github.com/MotiMortal/AluraBooks#mobile-first)
   - [Responsividade](https://github.com/MotiMortal/AluraBooks#responsividade)

## HTML e CSS
No `<head>` do HTML é possível notar ligações com o Google Fonts que é origem dos modelos e pesos de fontes utilizados no projeto (_Josefin-sans e Poppins_). Há, também, ligações com as folhas de estilo: reset.css e style.css; e um script. Onde o reset (https://meyerweb.com/eric/tools/css/reset/) funciona para tirar todas os estilos padrões de cada navegador, afim de padronizar a experiência do usuário, mesmo que ele acesse de diferentes navegadores (o projeto foi desenvolvido utilizando o Mozilla Forefox como visualizador).
O style.css é uma folha de estilo geral, onde há a declaração de variáveis `:root{}`, o estilo base de todo o `<body>` e os imports para todas as outras folhas de estilo, cada uma responsável por uma seção do html (`<section>`).
* Header - topo da página com menu de navegação.
* Banner - barra de pesquisa.
* Carrossel - o _swiper_ dos livros e cards de destaques.
* Topicos - tópicos em destaque.
* Contato - barra para inserção de email.
* Rodape - rodape com o Grupo Alura.

O script utilizado foi a API _Swiper.js_ (https://swiperjs.com/) para tornar possível o desenvolvimento do menu em forma de carrossel de forma simples, uma vez que o foco do projeto era a prática de css e _media queries_. 

## Mobile-first
A ideia principal do projeto foi de utilizar _media queries_ partindo da interface menor (smartphone) e, assim, progredir para maiores (tablets e PCs). A disposição de blocos, elementos, imagens e texto foram pré-definidas por um designer através da plataforma _Figma_.
Os limites de responsividade foram definidos na largura de:
* 428 pixels (smartphone)
* 1024 pixels (tablet)
* 1728 pixels (PC)

Como o projeto foi pensado inicialmente para celular (_mobile first_) foi utilizado um tamanho mínimo de largura (_min-width_) para que o estilo específico seja aplicado.

`@media screen and (min-width: "x"px){}`

### Responsividade

De acordo com o tamanho da tela foi preciso ocultar alguns items utilizando na sua devida _query_ o `display:none`.Além disso, foi utilizado o `display:flex` para ordenar os items em diferentes formas (colunas e linhas) tal como em cantos diferentes da tela.
Outro fator importante para a melhor resposividade foi o uso de variáveis relativas e porcentagens, além da mudança dentro de cada _media query_ de medidas absolutas.

