# Caderno virtual - Lógica da Programação e Algoritmos
Boas vindas! Este é seu caderno virtual. Aqui você deverá guardar todos os conceitos aprendidos e atiuvidades dessa unidade curricular. 


## História de Js
Javascript em sua historia começou no ano de 1995 por Brendan Eich, a pedido de uma empresa chamada Netscape, o js foi criado com o intuito de que scripts pudessem ser executados do lado do clietne e interagissem com o usuário sem que o script tivesse que passar pelo servidor.

## O que o javascript é capaz de fazer
Uma função de JavaScript do lado do servidor pode acessar o banco de dados, realizar diferentes operações lógicas e responder a diversos eventos acionados pelo sistema operacional do servidor.
o Javascript funicona bem mais do lado do cliente.
# variável
variáveis é como se fosse semi declarações automaticas, ou seja, você não precisa declarar antes do código, pode ser feito na hora usando :
### var
Ela pode ser reatribuída e redeclarada.

 ```js
var nome = 'Raian'
console.log(nome)

``` 
### let
ela pode somente reatribuida, mas nunca redeclarada
 ```js
let batata = 'pure'
// reatribuição
batata = 'batata frita'

``` 

### const
não pode ser redeclarado nem reatribuída, e assim como a let ela também tem escopo de bloco.

 ```js
const a = 20
const b = 30
const soma = (a+b)
console.log(soma)

``` 
## String
São dados que o computador entende como texto, para que o que você escreveu seja uma string basta colocar aspas ( normal ou dupla), crase ou apóstrofo no inico e no final da palavra ou frase.

# Tipos primitivos
## Boolean
Boolean é usado cmo true/ false
 ```js
let x = 5;
let y = 10;

// condição: x é menor que y
let resultado = x < y;

// mostrar o resultado na tela
if (resultado0 {
console.log("verdadeiro);
} else {
console.log("Falso");
}
```
## Undefined
Undefined é um valor não definido, aparece quando há uma interação com o usuario por exemplo: há três perguntas, o computador pergunta o nome, idade e endereço do usuario, aí ele fornece seu nome e sua idade mas não o seu endereço. Nesta ocasião aparece o Undefined

## Null
Representa um valor vazio Por exemplo: let minhaVariavel = null; Aqui, a variável “minhaVariavel” é atribuída ao valor null, indicando que não há um valor válido associado a ela. É importante ressaltar que o valor null não é considerado um objeto, mas sim um valor especial de tipo primitivo.

## Number
são valores numéricos ( podem ser inteiro ou decimais)

# Operadores 
a = 2 -> atribui valor de 2 para a
## Lógicos
&& significa E || siginifica Ou
## Comparação 
"==" igual

"===" igual

">"  maior que

"<" menor que

">="   maior igual a

"<=" menor igual a

"!==" diferente

"!=" diferente

# Matemáticos
"+" mais

"-" menos

"*" multiplicação

"/" divisão

"%" módulo ( ou resto)

"**" poténcia



# Arrays em JavaScript

## O que é um Array?
Em JavaScript, um array é um tipo de estrutura de dados que armazena uma lista ordenada de valores. Esses valores podem ser de qualquer tipo, como números, strings, objetos ou até mesmo outros arrays. Os arrays são zero-indexados, o que significa que o primeiro elemento tem o índice 0, o segundo elemento tem o índice 1 e assim por diante.

## Criando Arrays
Existem várias formas de criar um array em JavaScript:

## Usando a Notação de Colchetes:

``` js
let frutas = ['maçã', 'banana', 'laranja'];
```
## Usando o Construtor Array:
``` js
let numeros = new Array(10, 20, 30);
```
## Ou, se você quiser criar um array com um tamanho específico (sem valores definidos):

``` js
let vazio = new Array(5); // Um array com 5 posições, todas indefinidas

```

# Tipos de Arrays
Embora todos os arrays em JavaScript sejam do mesmo tipo (Array), eles podem conter diferentes tipos de elementos:

## Arrays de Números:
``` js
let numeros = [1, 2, 3, 4, 5];
```
## Arrays de Strings:
``` js
let palavras = ['hello', 'world', 'JavaScript'];
```
## Arrays Mistas:
``` js
let misto = [1, 'texto', true, { chave: 'valor' }, [1, 2, 3]];
```
## Arrays de Objetos:
``` js
let pessoas = [
  { nome: 'João', idade: 30 },
  { nome: 'Maria', idade: 25 }
];

```
## rrays Multidimensionais (Arrays de Arrays):
``` js
let matriz = [
  [1, 2, 3],
  [4, 5, 6],
  [7, 8, 9]
];
```
# Manipulando Arrays
Aqui estão alguns exemplos de como você pode manipular arrays:

## Acessar Elementos:
``` js
let frutas = ['maçã', 'banana', 'laranja'];
console.log(frutas[0]); // 'maçã'

```
## Adicionar Elementos:
``` js
let frutas = ['maçã', 'banana'];
frutas.push('laranja'); // Adiciona 'laranja' ao final do array
console.log(frutas); // ['maçã', 'banana', 'laranja']

```
## Remover Elementos:
``` js
let frutas = ['maçã', 'banana', 'laranja'];
frutas.pop(); // Remove 'laranja' do final
console.log(frutas); // ['maçã', 'banana']

```
## Iterar Sobre um Array:
``` js
let frutas = ['maçã', 'banana', 'laranja'];
frutas.forEach(function(fruta) {
  console.log(fruta);
});
```
## Filtrar Elementos:
``` js
let numeros = [1, 2, 3, 4, 5];
let pares = numeros.filter(function(numero) {
  return numero % 2 === 0;
});
console.log(pares); // [2, 4]
```
## Transformar Elementos:
``` js
let numeros = [1, 2, 3];
let aoQuadrado = numeros.map(function(numero) {
  return numero * numero;
});
console.log(aoQuadrado); // [1, 4, 9]
```
## Encontrar Elementos:
``` js
let frutas = ['maçã', 'banana', 'laranja'];
let encontrada = frutas.find(function(fruta) {
  return fruta === 'banana';
});
console.log(encontrada); // 'banana'

```
## Ordenar Elementos:
``` js
let numeros = [3, 1, 4, 1, 5, 9];
numeros.sort(function(a, b) {
  return a - b;
});
console.log(numeros); // [1, 1, 3, 4, 5, 9]

```

# Métodos Úteis de Arrays
concat(): Junta dois ou mais arrays.
join(): Junta todos os elementos de um array em uma string.
reverse(): Inverte a ordem dos elementos.
slice(): Retorna uma cópia superficial de uma parte do array.
splice(): Adiciona ou remove elementos em uma posição específica.

# Conclusão
Arrays são uma estrutura de dados fundamental em JavaScript e oferecem uma grande flexibilidade para armazenar e manipular listas de valores. Eles são amplamente utilizados em várias operações e são uma parte essencial do desenvolvimento em JavaScript.



## Atividades desenvolvidas
Escreva aqui as atividades desenvolvidas em sala e para casa. Você pode detelhar a atividade e usar links das atividades do codepen e vídeos desenvolvidos em sala. 


