# Funções avançadas no ES6

**escrevendo funções de maneira classica:**
function log(value) {
      console.log(value);
}
log('test');

**funções anônima (clássicas), omitindo o nome:**

var log = function(value) {
      console.log(value);
};
log('test');

**Retorno de variável:**

var sum = function(a, b) {
      return a+b;
}
console.log(sum(5, 5));

**Com o surgimento do ECMA6, surgiu a arrow function!**

**Arrow functions  '=>'** (funções anônimas), só podem ser atribuídas a uma variável ou como parâmetro para outra função. Também permite omitir o "return" se o lado direito for uma expressão.

var sum = (a, b) => a + b;

console.log(sum(5, 15));

*Pra fazer um statment, é necessário incluir '{ }'*

***Hoisting não funciona com arrow function***



## Default Function Arguments

Antigamente era necessário atribuir cada uma das variáveis a um valor para criar um padrão. Hoje em dia, após o surgimento do ECMA6, não é mais necessário realizar uma validação, podendo simplesmente inserir um valor padrão, de forma enxuta e atribuir um valor padrão pra minha função quando algum valor não é passado.

Além disso, é possível referenciar outros parâmetros.

Fique atento, pois a ordem é importante:
a, b = a 
Não -> b = a, a
(erro de referência, pois não é possível acesasr uma variável antes de  declara-la)

Lazy evaluation: Toda vez que você deixa de passar um parâmetro, você consegue garantir que a função só vai ser executada no momento certo. Serve para gerar id's randômicos, disparar erros quando algo está faltando, entre outras ocasiões.




## Enhanced Object Literals

Maneira clássica que escrever objetos no JS é sempre entre { }

Uma outra maneira de atribuir valor à variáveis e métodos, pode ser referenciando uma variável. Porém, dessa forma você acabava repetindo a mesma palavra, caso o método possuíse o mesmo noem da variável.

Com o ECMA6 você pode omitir o lado direito, sem repetir a palavra. Short Range.




## Rest e Spread Operator

Antigamente era usado a variável "arguments", que representava uma variável reservada que representa todos os argumentos da função.



