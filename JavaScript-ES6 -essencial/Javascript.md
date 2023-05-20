

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

## Linguagem interpretada:

O código é executado de cima pra baixo e o resultado da execução é i**mediatamente retornado**. Não precisa ser transformado (compilado) em algo diferente para que o **navegador** possa executar.

- **Linguagem de tipagem fraca e dinâmica**
  significa que não há verificação em todas as operações no JavaScript, ou seja, é possível usar o operador '+' com uma string, sem que ocorra um erro
- **Typescript**
  é um super set do JavaScript, consegue adicionar alguns elementos que o JS não consegue
- **Flow**
  um pouco semelhante ao typescript, mas não é um super set... É como uma versão simplificada do typescript



## Funções de primeira classe e ordem maior

Quer dizer que a função pode ser atribuída a uma variável, atribuiía a uma estrutura de dados (object ou array), pode ser usada como argumento e também repassada por outras funções