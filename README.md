# JavaScript - II - Estruturas de Dados

---
## Instruções Iniciais:

1. Forkem o repositório para a conta pessoal de vocês.
2. Clonem no computador de vocês o repositório forkado em suas contas particulares.

**_ATENÇÃO_: Não modifiquem o conteúdo do projeto original forkado, apenas a que você copiou e renomeou!**

### Façam suas perguntas através do DontPad

[http://dontpad.com/On10-JSI](http://dontpad.com/On10-JSII)

---

## **1. Mas, afinal, qual é a importância da estrutura de dados?**

O trabalho de uma desenvolvedora front-end passa por uma função de extrema importância: o entendimento, manipulação e tratamento de dados.

Um fato que exalta a importância do estudo da estrutura de dados é **a atuação da desenvolvedora front-end dentro do projeto**. 

![front-endxback-end](assets/frontendxbackend.gif)

Normalmente, a desenvolvedora back-end desenvolve endpoints que encaminham os dados do banco de dados à desenvolvedora front-end. Assim, cabe à desenvolvedora front-end administrar e manipular os dados para serem exibidos na aplicação que está sendo construída, e também tratar os dados que serão enviados ao back-end.

![front-endxback-end2](assets/frontendxbackend2.gif)

A administração e manipulação dos dados passam pelo entendimento das estruturas de dados e dos métodos que podem ser utilizados para trabalhar com esses dados.

Logo, **Estrutura de Dados - ou *Data Structure*, é um meio de coletar e organizar informações de uma certa forma em que seja possível realizar operações com essas informações de um jeito efetivo.**

![data-structure](assets/data-structure.gif)

---

## **2. Então, o que são Arrays?**

Explicação Concisa: arrays são estruturas de dados que contêm uma lista ordenada de elementos.

```Javascript
const fruits = ['Apple', 'Banana', 'Pear'];

const numbers = [1, 2, 10, -2, -3, 7];
```

Mas, calma. Nós podemos aprofundar essa definição.

Um dos benefícios do array é que ele possibilita que, ao invés de declarar três variáveis diferentes, você pode declarar um array de variáveis:

```Javascript
let sanduicheQueijo = "Queijo";
let sanduichePresunto = "Rosbife";
let sanduicheVegetariano = "Vegetariano";

let sanduiches = ["Queijo", "Presunto", "Vegetariano"];
```

**Arrays são comumente utilizados para organizar dados de uma forma que os seus valores possam ser facilmente encontrados e manipulados.**

Normalmente, os dados armazenados são do mesmo tipo, como `integer` ou `strings`, ou, ainda, `objects` - que veremos mais para frente. Contudo, cabe mencionar que um array pode ser composto por elementos de tipos diversos.

```Javascript
let miscData = [1, "abajur", {index: "zero"}, 7, "beijinho", 5.6]
```

Bom, foi mencionado que o array engloba uma lista **ordenada** de dados. Ele é **ordenado** pois é possível acessar cada elemento através da sua posição dentro de um array:

```Javascript
const fruits = ['Apple', 'Banana', 'Pear'];

console.log(fruits[0]) 
// retorna a primeira posição do array: 'Apple'

const numbers = [1, 2, 10, -2, -3, 7];

console.log(fruits[1]) 
// retorna a segunda posição do array: 2
```

Essa posição é chamada comumente de **index** do elemento no array. E aqui é importante destacar que **a contagem do index** - ou da posição do elemento no array - **sempre se inicia em 0**.

![array-index](assets/arrayindex.gif)

### **Array.length**

Um array é um agrupamento de dados ordenado, onde é possível acessar um elemento de acordo com a sua posição.

Se é possível acessar a um elemento de acordo com a sua posição, logo se conclui que é possível saber quantos elementos existem dentro de um array.

Para isso existe a propriedade `length` -  que mostra o número de elementos contidos dentro de um array.

```Javascript
const clothing = ['shoes', 'shirts', 'socks', 'sweaters'];

console.log(clothing.length); // 4
```

Podemos usa-lo também para realizar uma operação de subtração com o tamanho total do array e, assim, pegar o último elemento de um array:

```Javascript
const clothing = ['shoes', 'shirts', 'socks', 'sweaters'];

console.log(clothing[clothing.length - 1]); // 'sweaters'
```
