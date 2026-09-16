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

Exemplo simples da ultilizacão do map():
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

Nesse código temos uma lista de objetos, o array tem nome e idade de cada aluno, usando o filter eu determino que quero apenas os alunos que tem idade acima de 20















