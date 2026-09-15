# ArrayListJs

## Tutorial e explicação de como manipular Listas em Javascript utilizando: map, filter e reducer.

### MAP()

Com o método map() é possivel executar uma função em cada ítem de um array, depois ele ira nos retornar um novo array, ou seja, ele não sobrescreve o original, tem melhor desenhepenho que o forEach() e consegue alterar os dados de maneira bem simples.

Exemplo simples da ultilizacão do map():
```
const array = [1, 4, 9, 16];

const map = array1.map((x) => x * 2);

console.log(map1);
```
A saída desse código vai ser:
```
[2, 8, 18, 32]
```
Nesse exemplo a função callback é chamado pelo método map, que recebe por parâmetro cada elemento do array 
