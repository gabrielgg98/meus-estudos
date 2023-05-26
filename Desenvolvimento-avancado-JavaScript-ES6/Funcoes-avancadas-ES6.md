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

