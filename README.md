# Caderno virtual - Lógica da Programação e Algoritmos
Boas vindas! Este é seu caderno virtual. Aqui você deverá guardar todos os conceitos aprendidos e atiuvidades dessa unidade curricular. 


# História de Js
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
## Arrays Multidimensionais (Arrays de Arrays):
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

# Switch case js
## O que é um switch case
O switch case em JavaScript é uma estrutura de controle muito útil quando estamos trabalhando com uma variável que pode assumir diferentes valores possíveis e, a partir desses valores, executar diferentes blocos de código correspondentes.

``` js
const fruta = prompt("Que fruta você deseja?")
switch (fruta) {
case 'laranja' :
console.log(" A laranja custa R$1,00 Real a unidade!")
break;
case 'maça' :
console.log("A maça custa R$0,50 a unidade!")
break;
default :
console.log(`mas não temos a fruta ${fruta}.`);
}
```

# explicação
### const fruta
o cont é para criar uma variável, e "fruta" foi o nome da variavél escolhida!

### switch
serve para iniciar o switch case, ele é de entrada, o nome é escolha em português logo você vê que serve para dar opções para úsuario.

### case
serve para dar o caso ao úsuario, de forma mais explicado, "se o úsuario falar tal coisa execute tal coisa".

### break
serve para quebrar o código, num bom sentido claro kkkkk, mas ele vai quebrar o código do case1 para poder dar outra opção de caso.

### default
serve para quando o úsuario escrever algo que não tenha em nenhum dos casos.

# if else
A condicional if é uma estrutura condicional que executa a afirmação, dentro do bloco, se determinada condição for verdadeira. Se for falsa, executa as afirmações dentro de else.
### exemplo
``` js
var frutas = ["maçã", "banana", "caju"];
var pergunta = prompt (" escolha dentre as opções: maçã, banana, caju")

var pos = frutas.indexOf(pergunta);

if (pergunta === "maçã" || pergunta === "banana" || pergunta === "caju"){
    console.log(`a fruta ${pergunta} esta pronta para entrega`);
    }else{
      console.log("Não encontramos essa fruta em nosso estoque");
    }
```
# function (funções)

Funções são blocos de construção fundamentais em JavaScript. Uma função é um procedimento de JavaScript - um conjunto de instruções que executa uma tarefa ou calcula um valor. Para usar uma função, você deve defini-la em algum lugar no escopo do qual você quiser chamá-la.
### para que serve?
Em JavaScript, as funções servem para:
 
Organizar o código: Dividindo o código em funções menores, você torna o seu programa mais fácil de entender e manter. Cada função pode ter uma tarefa específica, como calcular uma área, verificar se um número é par ou fazer uma animação.
Reutilizar código: Uma vez que você criou uma função, pode chamá-la quantas vezes quiser, em diferentes partes do seu programa. Isso evita que você escreva o mesmo código repetidamente.
Abstrair complexidade: Funções permitem esconder detalhes de implementação. Por exemplo, você pode criar uma função para ordenar uma lista de números, mas quem usa essa função não precisa saber exatamente como o algoritmo de ordenação funciona.
Criar programas modulares: Funções são a base para criar módulos em JavaScript, que são partes independentes de um programa. Isso facilita a colaboração em projetos maiores e a reutilização de código em diferentes projetos.



### Exemplo simples: 
``` js
function saudacao(nome) {
  console.log("Olá, " + nome + "!");
}

saudacao("Maria"); // Imprime "Olá, Maria!"
saudacao("João"); // Imprime "Olá, João!"
```



## Atividades desenvolvidas
Escreva aqui as atividades desenvolvidas em sala e para casa. Você pode detelhar a atividade e usar links das atividades do codepen e vídeos desenvolvidos em sala. 


