# Javascript

## História e conceitos

- **Lançado** em setembro de 1995

- Já foi chamado de 'Livescript', o que causou muita dúvida, pois alguns acharam que a linguagem baseava-se em Java, mas foi apenas uma estratégia de marketing

- Criado por **Brendan Eich**

- **ECMAScript =** padronização submetida pelo Netscape, serve como base para futuras implementações de outras linguagems

- **TC39** é o comitê responsável pela evolução do Javascript, composto pelo navegadores atuais

  - no **github/tc39** podemos acompanhar as propostas do comitê

    - **Fluxo de proposta:**
      Stage 0 : strawman (avaliação inicial da proposta)
      Stage 1: proposal (proposta formal onde um responsável é definido)

      Stage 2: draft (primeira versão da proposta que entra na especificação)

      Stage 3: candidate (quase finalizada, precisa de um feedback de implementação e de usuários)

      Stage 4: finished  (assinada e liberada)

- **ES2018**

  - Operadores rest/spread
  - Iteração assíncrona
  - Promise.prototype.finally()

- **Es.Next**
  Pode ser testada pelo babeljs.io



### Linguagem interpretada:

O código é executado de cima pra baixo e o resultado da execução é i**mediatamente retornado**. Não precisa ser transformado (compilado) em algo diferente para que o **navegador** possa executar.

- **Linguagem de tipagem fraca e dinâmica**
  significa que não há verificação em todas as operações no JavaScript, ou seja, é possível usar o operador '+' com uma string, sem que ocorra um erro
- **Typescript**
  é um super set do JavaScript, consegue adicionar alguns elementos que o JS não consegue
- **Flow**
  um pouco semelhante ao typescript, mas não é um super set... É como uma versão simplificada do typescript



### Funções de primeira classe e ordem maior

Quer dizer que a função pode ser atribuída a uma variável, atribuida a uma estrutura de dados (object ou array), pode ser usada como argumento e também repassada por outras funções



### Closure

Algumas linguagens como Python usam isso. É conhecido como '**escopo léxico**'. Basicamente, é a c**apacidade de uma função "lembrar" onde foi criada**. Escopo é um assunto bem polêmico, que gera bastante dúvidas. **No JavaScript hoje** em dia existem **3 tipos de escopo: Global, função e bloco.**



### Currying

Comum em linguagens funcionais. O JS por padrão não é funcional, mas pode ser usado pra escrever esse tipo de código. Currying serve para transformar 1 ou mais parâmentos em apenas uma função, que recebe 1 parâmetro. Simplifica processos em que um parâmetro precisa ser repetido diversas vezes.



### Hoisting

Significa 'levantar' ou 'suspender' algo. Isso é um comportamento que ocorre no JavaScript em declarações de variáveis e funções. O Hoisting é separado em 2 tipos = variáveis e funções. O hoisting de variável só eleva a criação da variável e não a sua atribuição. Já a função é içada ao topo como um todo, inclusive sua assinatura. **Uma boa prática é sempre declarar a função antes de usá-la.**



### Imutabilidade

É um conceito de linguagem funcional, mas também temos no JavaScript. Nessas linguagens, os dados que criamos nunca mudam. Caso você precise altera-lá, você terá que criar uma nova.



## Tipos e Variáveis

### Váriaveis

Existem **3 formas de armazenar determinado valor** para ser usado futuramente:
***var*** = foi o pioneiro (não respeita escopo de bloco)
***let***
***const***
Com a implementação do 'let' e 'const' surgiu o escopo de bloco

**Escopo global** = vazio (Não é uma boa prática escrever nesse tipo de escopo)

**Escopo bloco** = entre { }

**Escopo função** = function name( ) { }

**Objetos** - Podem ser alterados diretamente
**Constantes** - Não podem ser alterados diretamente, mas podem ser removidas, ter novos itens incluídos ou substituídos.

### Tipos

O JavaScript permite **6 tipos**:

- **String** - representa textos
- **Number** - números
- **Boolean** - true ou false
- **Null** - nulo
- **Undefined** - a variável ainda não foi setada (hoisting)
- **Symbol** - permite criar valores únicos (foi acrescentado recentemente)

Temos outros tipos que são:

- **Object** - Objetos
- **Function** - Também é um objeto, mas permite que o objeto possa ser chamado
- **Array** - Também é um objeto, mas tem uma relação com os itens (filhos) dele, conseguindo organizar cada item em posição e tipo definido

### Funções

São objetos que permitem serem chamados.

- **fn e arrowfn =** tem a mesma função, porém com arrowfn se for apenas uma expressão não precisa inserir retorno

## Operadores

**Operador binário:**
operando 1 operador operando2
1 + 2

**Operador unário:**
operando 1 operador
operador operando1

- **Aritméticos**

  - **Módulo (%) -** retorna o inteiro restante da divisão dos operandos
    12 % 5 - retorna 2.

  - **Incremento (++) e Decremento (--)**
    ++x - retorna a variável já incrementada
    x++ - retorna a variável atual e incrementa
    --x
    x--

  - **Negação (-) e Adição (+)**
    -3, nega 3
    +3, retorna 3
    +true, retorna 1 
    +false, retorna 0
    -true, retorna -1

  - **Exponenciação (**)**

    2 ** 3, retorna 8
    10 ** -1, retorna 0.1

  - **Agrupamento ( )**
    2 * (3 + 2)
    *Também agrupa condicionais*

- **Atribuição**
  *Pode ser mesclado com atribuições matemáticas*

  - **Atribuição**
    x = y

  - **Atribuição de adição**
    x = x + y ou x += y

  - **Atribuição de subtração**
    x = x - y ou x -= y

  - **Atribuição de multiplicação**
     x = x * y ou x/= y

  - **Atribuição de resto**
    x = x % y ou x %= y

    

- **Comparação**

  - **Igual (==)**
    *retorna verdadeiro caso os operandos sejam iguais*
    "3" == var1
    3 == '3' *(por ser tipagem fraca, o JS retorna como verdadeiro)*
  - **Não igual (!=) **
    *retorna verdadeiro caso os operando não sejam iguais*
    var2 != "3"
  - **Estritamente igual (===)**
    *retorna verdadeiro caso os operandos sem iguais e do mesmo tipo*
    3 === var1
  - **Estritamente não igual (!==)**
    *retorna verdadeiro caso os operandos não sejam iguais e/ou não sejam do mesmo tipo*
    var1 !== "3"
    3 !== '3'
  - **Maior que (>)**
    *retorna verdadeiro caso o operando da esquerda seja maior que o da direita*
    var2 > var1
    "12" > 2
  - **Maior que ou igual (>=)**
    *retorna verdadeiro caso o operando da esquerda seja maior ou igual o operando da direita*
    var2 >= var1
    var1 >= 3
  - **Menor que (<)**
    *retorna verdadeiro caso o operando da esquerda seja maior que o da direita*
    var1 < var2
    "2" < "12"
  - **Menor que ou igual (<=)**
    *retorna verdadeiro caso o operando da esquerda seja maior ou igual o operando da direita*
    var2 <= var1
    var1 <= 2

- **Condicional**
  *operador ternário*
  Condição ? valor1 : valor2 *(A depender da condição, escolhe um ou outro)*
  true ? 'foo' : 'bar', retorna 'foo'
  false ? 'foo' : 'bar', retorna 'bar'

- **Lógicos**
  **&& e ||** ( E e OU)

  exp1 && exp2

  exp1 || exp2
  **&&** - se for string, retorna string, se for booleano, retorna booleano

  **Não lógico** - nega a condição
  !exp1

  !!, converte para booleano no caso de string

- **Spread ...** 
  Consegue iterar a cada item do array ou do objeto e passar para o parâmetro. Funciona com funções também.
  ***var partes = [ 'ombro', 'joelhos'];***
  ***var musica = ['cabeca', ...partes, 'e', 'pés'];***

  **var musica = ['cabeca', 'ombro', 'joelhos', 'e' 'pés'];**

- **Delete** - deletar algo
  delete somethin;

- **typeof** - determinar tipo
  typeof something;

## Estruturas condicionais e repetição

- **if, else e else if**

- **switch**

  

  ## Estruturas de repetição

  - **for**
  - **while**
  - **do...while**
  - **for...in/off**
  - **continue**
  - **break**

## Orientação a objetos

- **Herança**
  - baseada em protótipos
  - prototype (armazena as definições do objeto)
  - constructor
- **Classes**
  - ES6
  - Simplificação da herança de prototipos
  - palavra chave 'class'
- **Modificadores de acesso**
  Atualmente o JavaScript não suporta e os browsers não oferecem suporte.
  - privado / público
- **Encapsulamento**
  oculta detalhes do funcionamento interno
- **Static**
  acessar método/atributos sem instanciar



## Design Pattern

**Definição:**

- São soluções generalistas para problemas recorrentes durante o desenvolvimento de um software. Não se trata de um framework ou um código pronto, mas de uma definição de alto nível de como um problema comum pode ser solucionado.

**A Pattern Language:**

- Feito em 1978 por Christopher Alexander, Sara Ishikawa e Murray Silverstein;
- Catalogaram 253 tipos de problemas/desafios de projetos;

**Formato de um pattern:**

- Nome;
- Exemplo;
- Contexto;
- Problema;
- Solução;

**Tipos**

**Criação -** são aqueles que abstraem e/ou adiam o processo criação dos objetos. Eles ajudam a tornar um sistema independente de como seus objetos são criados, compostos e representados;

- **Padrões de criação:**
  - Abstract Factory;
    - Builder;
      - Factory Method;
        - Prototype; 
          - Singleton;

**Estrutural -** se preocupam com a forma como classes e objetos são compostos para formar estruturas maiores;

- **Padrões estruturais:**
  - Adapter;
    - Bridge;
      - Composite;
        - Decorator;
          - Facade;
            - Business Delegate;
              - Flyweight;
                - Proxy;

**Comportamental -** se concentram nos algoritmos e atribuições de responsabilidades entre os objetos. Eles não descrevem apenas padrões de objetos ou de classes, mas também os padrões de comunicação entre os objetosl;

- **Padrões Comportamentais:**
  - Chain of Responsability;
    - Command;
      - Interpreter;
        - Iterator;
          - Mediator;
            - Observer;
              - State;
                - Strategy;
                  - Template Method;
                    - Visitor
                      

## Patterns mais utilizados

- **Factory -** todas as funções que retornam um objeto, sem a necessidade de chamá-las com o 'new', são consideradas funções Factory (fábrica);
- **Singleton -** o objetivo desse pattern é criar uma única intância de uma função construtora e retorná-la toda vez em que for necessário utilizá-la;
- **Decorator -** recebe uma outra função como parâmetro e estende o seu comportamento sem modificá-la explicitamente;
- **Observer -** A instância (subscriber) mantém uma coleção de objetos (observers) e notifica todos eles quando ocorrem mudanças no estado;
- **Module -** possibilita organizarmos melhor o nosso código, sem a necessidade de expor variáveis globais;



## Manipulação e Iteração de arrays

- **Criar um array**
  **Array.of -** cria uma nova instância a partir do número de parâmetros informados (pode ser string, números, etc);

  **Array -** Cria uma nova instância de array de acordo com os parâmetros informado;

  **Array.from -** Cria uma nova instância de array a partir de um parâmetro array-lie ou iterable object;

- **Inserir ou remover elementos**
  **Push -** acicionar um ou mais elementos no final do array e retorna o tamanho do novo array;

  **Pop -** remove o último elemento de um array e retorna o elemento removido;

  **Unshift -** adicionar um ou mais elementos no início do array e retorna o tamanho do novo array;

  **Shift -** remove o primeiro elemento de um array e retorna o elemento removido (comportamento similar ao pop);

  **Concat -** concatena um ou mais arrays retornando um novo array;

  **Slice -** retorna um novo array "fatiando" o array de acordo com início e fim;

  **Splice -** altera um array adicionando novos elementos enquanto remove elementos antigos;

- **Iterar elementos**

  **forEach -** iteração de cada item dentro de um array;

  **Map -** retorna um novo array, de mesmo tamanho, iterando cada item de um array;

  **Flat -** retorna um novo array com todos os lementos de um sub-array concatenados de forma recursiva de acordo com a profundidade especificada (depth);

  **flatMap -** retorna um novo array assim como a função map e executa um flat de profundidade 1;

  **Keys -** retorna um array iterator que contém as chaves para cada elemento do array;

  **Values -** retorna um array iterator que contém os valores para cada elemento do array;

  **Entries -** retorna um array iterator que contém os pares chave/valor para cada elemento do array;

  **Find -** retorna o primeiro item de um array que satisfaz a condição;

  **findIndex -** retorna o índice do primeiro item de um array que satisfaz a condição;

  **filter -** retorna um novo array com todos os elementos que satisfazem a condição;

  **indexOf -** retorna o primeiro índice em que um elemento pode ser encontrado em um array;

  **lastIndexOf -** retorna o último índice em que um elemento pode ser encontrado;

  **includes -** retorna um booleano verificando se determinado elemento existe no array;

  **some -** retorna um booleano verificando se pelo menos um item do array satisfaz a condição;

  **every -** retorna um booleano verificando se todos os itens de um array satisfazem a condição;

  **sort -** ordena os elementos de um array de acordo com a condição;

  **reverse** - inverte os elementos de um array.

  

  - **Transformar em outro tipo de objeto**

    **join -** junta todos os elementos de um array, separados por um delimitador e retorna uma string;

    **reduce -** retorna um novo tipo de dado iterando cada posição de um array;

    

  

  

  

  



