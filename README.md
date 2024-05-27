
Métodos de Array em JavaScript
Este documento fornece uma visão geral dos métodos mais comuns de array em JavaScript. Arrays são uma estrutura de dados fundamental em JavaScript, permitindo armazenar e manipular coleções de dados.

Índice
Introdução
Métodos de Mutação
push
pop
shift
unshift
splice
Métodos de Acesso
concat
slice
indexOf
lastIndexOf
includes
Métodos de Iteração
forEach
map
filter
reduce
find
findIndex
Métodos de Ordenação
sort
reverse
Conclusão
Introdução
Arrays em JavaScript são objetos que permitem armazenar múltiplos valores em uma única variável. Eles vêm com diversos métodos integrados que facilitam a manipulação e acesso aos dados.

Métodos de Mutação
push
Adiciona um ou mais elementos ao final de um array e retorna o novo comprimento do array.

javascript
Copiar código
let array = [1, 2, 3];
array.push(4); // [1, 2, 3, 4]
pop
Remove o último elemento de um array e retorna esse elemento.

javascript
Copiar código
let array = [1, 2, 3, 4];
let lastElement = array.pop(); // lastElement = 4, array = [1, 2, 3]
shift
Remove o primeiro elemento de um array e retorna esse elemento.

javascript
Copiar código
let array = [1, 2, 3, 4];
let firstElement = array.shift(); // firstElement = 1, array = [2, 3, 4]
unshift
Adiciona um ou mais elementos no início de um array e retorna o novo comprimento do array.

javascript
Copiar código
let array = [1, 2, 3];
array.unshift(0); // [0, 1, 2, 3]
splice
Adiciona ou remove elementos de um array.

javascript
Copiar código
let array = [1, 2, 3, 4];
array.splice(1, 2, 'a', 'b'); // [1, 'a', 'b', 4]
Métodos de Acesso
concat
Retorna um novo array que é a concatenação de dois ou mais arrays.

javascript
Copiar código
let array1 = [1, 2];
let array2 = [3, 4];
let newArray = array1.concat(array2); // [1, 2, 3, 4]
slice
Retorna uma cópia rasa de uma parte de um array em um novo array.

javascript
Copiar código
let array = [1, 2, 3, 4];
let newArray = array.slice(1, 3); // [2, 3]
indexOf
Retorna o primeiro índice em que um determinado elemento pode ser encontrado no array, ou -1 se o elemento não estiver presente.

javascript
Copiar código
let array = [1, 2, 3, 4];
let index = array.indexOf(3); // 2
lastIndexOf
Retorna o último índice em que um determinado elemento pode ser encontrado no array, ou -1 se o elemento não estiver presente.

javascript
Copiar código
let array = [1, 2, 3, 4, 3];
let index = array.lastIndexOf(3); // 4
includes
Determina se um array contém um determinado elemento, retornando true ou false conforme apropriado.

javascript
Copiar código
let array = [1, 2, 3, 4];
let containsElement = array.includes(3); // true
Métodos de Iteração
forEach
Executa uma função fornecida uma vez para cada elemento do array.

javascript
Copiar código
let array = [1, 2, 3];
array.forEach(element => console.log(element)); // 1, 2, 3
map
Cria um novo array com os resultados da chamada de uma função para cada elemento do array.

javascript
Copiar código
let array = [1, 2, 3];
let newArray = array.map(element => element * 2); // [2, 4, 6]
filter
Cria um novo array com todos os elementos que passaram no teste implementado pela função fornecida.

javascript
Copiar código
let array = [1, 2, 3, 4];
let newArray = array.filter(element => element % 2 === 0); // [2, 4]
reduce
Aplica uma função contra um acumulador e cada elemento do array (da esquerda para a direita) para reduzi-lo a um único valor.

javascript
Copiar código
let array = [1, 2, 3, 4];
let sum = array.reduce((accumulator, currentValue) => accumulator + currentValue, 0); // 10
find
Retorna o valor do primeiro elemento no array que satisfaz a função de teste fornecida. Caso contrário, undefined é retornado.

javascript
Copiar código
let array = [1, 2, 3, 4];
let found = array.find(element => element > 2); // 3
findIndex
Retorna o índice do primeiro elemento no array que satisfaz a função de teste fornecida. Caso contrário, -1 é retornado.

javascript
Copiar código
let array = [1, 2, 3, 4];
let index = array.findIndex(element => element > 2); // 2
Métodos de Ordenação
sort
Ordena os elementos do array e retorna o próprio array.

javascript
Copiar código
let array = [3, 1, 4, 2];
array.sort(); // [1, 2, 3, 4]
reverse
Inverte a ordem dos elementos do array e retorna o próprio array.

javascript
Copiar código
let array = [1, 2, 3, 4];
array.reverse(); // [4, 3, 2, 1]
Conclusão
Os métodos de array em JavaScript fornecem uma ampla gama de funcionalidades que facilitam a manipulação de coleções de dados. Conhecer esses métodos é essencial para escrever código eficiente e eficaz em JavaScript.
