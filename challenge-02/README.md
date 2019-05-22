# Desafio da semana #2

Nesse exercício, você está livre para escolher os nomes para suas variáveis e funções! :smile:

```js
// Crie uma função que receba dois argumentos e retorne a soma dos mesmos.
function soma(x, y){ return x+y; }

// Declare uma variável que receba a invocação da função criada acima, passando dois números quaisquer por argumento, e somando `5` ao resultado retornado da função.
var somarCinco = soma(3, 2) +5;

// Qual o valor atualizado dessa variável?
// 10

// Declare uma nova variável, sem valor.
var nova;

/*
Crie uma função que adicione um valor à variável criada acima, e retorne a string:
    O valor da variável agora é VALOR.
Onde VALOR é o novo valor da variável.
*/
function nomeiaNova(){
    nova = "O valor da variável agora é VALOR";
    return nova;
}

// Invoque a função criada acima.
nomeiaNova();

// Qual o retorno da função? (Use comentários de bloco).
/*
    "O valor da variável agora é VALOR"
*/

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos;
2. Se qualquer um dos três argumentos não estiverem preenchidos, a função deve retornar a string:
    Preencha todos os valores corretamente!
3. O retorno da função deve ser a multiplicação dos 3 argumentos, somando `2` ao resultado da multiplicação.
*/
function plus(x, y, z) {
    if(arguments.length != 3) {
        return "Preencha todos os valores corretamente";
    }
    return x * y * z;
}

// Invoque a função criada acima, passando só dois números como argumento.
plus(3,2);

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
// "Preencha todos os valores corretamente"

// Agora invoque novamente a função criada acima, mas passando todos os três argumentos necessários.
plus(2,3,2);

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
// 12

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos.
2. Se somente um argumento for passado, retorne o valor do argumento.
3. Se dois argumentos forem passados, retorne a soma dos dois argumentos.
4. Se todos os argumentos forem passados, retorne a soma do primeiro com o segundo, e o resultado, dividido pelo terceiro.
5. Se nenhum argumento for passado, retorne o valor booleano `false`.
6. E ainda, se nenhuma das condições acima forem atendidas, retorne `null`.
*/
function op(x, y, z) {
    if(op.arguments.length == 0) return false;
    else if(op.arguments.length == 1) return op.arguments[0];
    else if(op.arguments.length == 2) return (op.arguments[0] + op.arguments[1]);
    else if(op.arguments.length === 3) {
        return (op.arguments[0] + op.arguments[1]) / op.arguments[3];
    }
    else { return null;}
}

// Invoque a função acima utilizando todas as possibilidades (com nenhum argumento, com um, com dois e com três.) Coloque um comentário de linha ao lado da função com o resultado de cada invocação.
op(); // false
op(3); // 3
op(3, 7); // 10
op(3, 7, 2); // 5
```