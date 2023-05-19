# Introdução a Criação de Websites com HTML5 e CSS3



# HTML5 

## História:

- **Criado por Tim Berners-lee**, motivado para compartilhar textos e documentos
- **HTML 1 - 1991**
- **HTML 2- 1995**
- **HTML 3 - 1997**
- **HTML 4 - 1997**
- **HTML 5 - 2014**



## Estrutura básica:

- O **elemento** é a base do HTML;
  - *Ele começa com uma **tag de abertura, seguido de um atributo, o conteúdo e a tag de fechamento;***
- **!DOCTYPE não é um elemento**; apenas diz ao navegador o tipo do documento a ser lido;
- **Todos os elementos** ficam dentro da tag html;
- **O elemento** **head** contém as meta-informações, para o navegador e o buscador;
  - ***A tag meta** serve para dizer ao navegador como fazer o encode dos caracteres;*
  - ***A tag title** coloca o título na aba do servidor;*
- **Na tag** **body** vem todo o conteúdo que vai estar na nossa página.



## Semântica:

- **Surgiu por volta da versão 5**, trazendo novos elementos para aumentar o nível de organização dos htmls, facilitando a leitura dos elementos por parte dos programadores.
  - Alguns exemplos são: **section, header, article, aside, footer e os h1** (que não surgiram nessa versão, mas servem muito bem para o propósito de trazer sentido, pois representam a importância dos titulos dentro das páginas; use apenas um h1 por página)



## Textos & Links:

- **H1 a H6** títulos e suas importâncias
- **A** **tag 'p'**, representa um parágrafo, que suporta textos, vídeos e outros tipos de conteúdo
- **O** **elemento 'a'** representa uma âncora:
  - **Com 'Href'** direciona a um hyperlink, que pode ser um site, um email ou um telefone
    - No caso do **email/telefone usar 'mailto:'**
  - **A** **tag 'target'** serve para direcionar a abertura do link, sendo **'_blank' = uma nova aba**



## Imagens:

- Representadas pelo **elemento 'img'**, não necessita de fechamento
  - **Contém 'src' e 'alt'**
    - **'src'** indica o local de origem da img, seja local ou remoto
      - **'alt'** representa o texto alternativo que será carregado, caso a imagem dê erro



## Listas:

- **ul, ol e li** são as tags usadas para agrupar coleção de itens
- **'ul'** = uma lista em que a ordem não é importante
- **'ol'** = a ordem é importante e geralmente tem uma numeração
- **'li'** = um item da lista



# CSS3

## Definição:

- **Criado em 1996 é usado para criar regras de estilos para elementos ou grupos de elementos**
- É formada por um **seletor** ou um grupo de seletor
  - **seletores = elementos html**
- Entre { } temos as **declarações**
  - **As declarações são formadas por propriedade e  valor**
- Elementos HTML do mesmo tipo podem ser divididos em **ID e Classe** para ter regras diferentes
  - **Seletores de tipo =** representam um elemento HTML
    - **ID e Classes** podem representar QUALQUER elemento
      - **Uma classe é precedida por um '.'**
        - **Uma id é precedida por um '#' e só pode ser usada uma vez na página**



## Conceitos básicos:

- **Com o CSS conseguimos alterar a aparência da box model**
  
  - **Box model** = margin, border, padding, content
    
    - **margin** = espaçamento entre elementos
      
      - **border** = circundando o padding e o conteúdo, pode ser alterado largura e cor
        ***border**: 3px solid blue (muda tamanho, estilo e cor)*
        ***border- + top, right, bottom, left** (muda as propriedades individualmente de cada lado)*
        ***Estilos =** solid, dotted, dashed (sólida, pontilhada e tracejada)*
        
        ***border-width =** largura*
        
        ***border-color =** cor*
        
        ***border-style =** estilo*
        
        ***border-radius =*** *arredondar cantos*
        ***Podemos unir os lados + os aspectos de forma simplificada ou individual***
        
        
        
        - **padding** = espaçamento entre border e conteúdo
          
          ***padding**: 10px 5px ->** muda superior e inferior*
          ***padding: 10px 10px 5px 0 -**> muda individualmente cada canto, em sentido horário*
          
          ***também pode ser escrito: padding- + top, right, bottom, left***
          
          - **conteúdo** = é o que o bloco representa (txt, img, video)
  
- **background =** atalho para mudar propriedades do fundo
  
  ***background-color =** cor*
      ***background-color + nome da cor***
      ***background-color + HEX***
      **background + COR (nome ou HEX)***
  
  ***background-image =** imagem*
  ***background-position =** posição*
  
- **font-family =** altera a fonte do texto

- **font-size =** altera o tamanho do texto

- **font-style =** altera a aparência do texto (normal=padrão)

- **font-weight =** altera o peso do texto (negrito, por exemplo)

- **text-transform =** altera o texto em maiusculas e minusculas
  *uppercas deixa o texto todo MAIÚSCULO*
  *lowercase deixa o texto todo minúsculo*
  *capitalize deixa o texto com a Primeira Letra De Cada Palavra Maiúscula*

- **text-decoration =** decora o texto
  *underline coloca uma linha abaixo do texto*
  *overline coloca uma linha sobre o texto*
  *line-through risca o texto*



- **list-style-type = ** altera o marcador das listas
  *Os valores mudam de acordo com o tipo de lista*
  ***UL temos o square**, que muda da bolinha para o quadradinho*
  ***OL temos o upper-roman** que muda os números para romanos*
  Além disso, podemos mudar os marcadores da UL para **simbolos como emojis ex: \1f44d = joinha**
      ***E até mesmo inserir imagens** no lugar dos marcadores com **list-style-image**  e a url da imagem*



## Dimensão e alinhamento

**Width ** serve para ajustar a largura em px ou %
**Height** serve para ajustar a altura em px ou %

**Max-width** serve para ajustar a **largura máxima** em px ou %
**Max-height** serve para ajustar a **altura máxima** em px ou %

**Margin** serve para dar espaçamento entre elementos, mas o **valor 'auto'** pode ser usado para alinhar automaticamente elementos

**Text align** serve para alinhar textos, podendo ser **= left, right, center, justify**

