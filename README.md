# ArrayListJs

## Tutorial e explicação de como manipular Listas em Javascript utilizando: map, filter e reducer.

### MAP()

Com o método map() é possivel executar uma função em cada ítem de um array, depois ele ira nos retornar um novo array, ou seja, ele não sobrescreve o original, tem melhor desenhepenho que o forEach() e consegue alterar os dados de maneira bem simples.

Exemplo simples da ultilizacão do map():
```
const array = [1, 4, 9, 16];

const map = array.map((x) => x * 2);

console.log(map);
```
A saída desse código vai ser:
```
[2, 8, 18, 32]
```
Nesse exemplo a função callback é chamado pelo método map, que recebe por parâmetro cada elemento do array, x é o nosso primeiro elemento e ele vai ser multiplicado por 2, depois o segundo elemento e assim sucessivamente.

### FILTER()

Esse método cria um novo array com todo os elemntos que passem no teste implementado por uma função fornecida, assim como o map ele também não altera o array original, se nenhum dos elemntos passarem no teste, vai ser retornado uma array vazia.

Exemplo simples da ultilizacão do filter():
```
const alunos = [
  {nome: 'Maria', idade: 18},
  {nome: 'João', idade: 20},
  {nome: 'Anna', idade: 23},
  {nome: 'Diego', idade: 25},
]

const maiorDeVinte = alunos.filter(aluno => aluno.idade >= 20);
console.log(maiorDeVinte);
```
A saída desse código vai ser:
```
[{nome: 'João', idade: 20}, {nome: 'Anna', idade: 23}, {nome: 'Diego', idade: 25}]
```

Nesse código temos uma lista de objetos, o array tem nome e idade de cada aluno, usando o filter eu determino que quero apenas os alunos que tem idade acima de 20. 
Filter vai chamar a função callback uma vez pra cada elemento da lista, e todos os que retornarem true são colocados na nova lista que foi construída.

### REDUCE()

Essa função serve para iterar sobre um array e utilizar o valor de cada item para criar um objeto final com base em função dada. Como o próprio nome da função já diz, ela “reduz” os itens de um vetor a um valor único. Por exemplo, podemos utilizar para somar todos os elemntos de uma lista.


Exemplo simples da ultilizacão do reduce():
```
const numeros = [10, 15, 20, 25, 30, 35];

const soma = numeros.reduce((acumulador, atual) => {
    return acumulador + atual;
}, 0);

console.log(soma);

```
A saída desse código vai ser:
```
135
```

O *acumulador* guarda o resultado das operações, *atual* é o item que está sendo lido na lista no momento, e *0* é o valor inicial, ponto de partida do acumulador.












