1.Desafio - Visita na feira

Você está na feira com a sua sacola e parou em uma banca. O feirante lhe entregou pimentões amarelos e vermelhos. Agora iremos somar os pimetões amarelos e vermelhos para descobrir o total de pimentões na sacola.  Você receberá 2 inteiros que devem ser lidos e armazenados nas variáveis A (pimentões amarelos) e B (pimentões vermelhos). Faça a soma de A e B atribuindo o seu resultado na variável X (total de pimentões). Apresente X como descrito na mensagem de exemplo abaixo. Não apresente outra mensagem além da mensagem especificada.

Entrada
A entrada contém 2 valores inteiros, separados por um espaço.

Saída
Imprimir a mensagem "X = " (sendo a letra X maiúscula) seguido pelo valor da variável X e pelo final de linha. Assegure que exista um espaço antes e depois do sinal de igualdade.

Resposta

// a função gets é implementada dentro do sistema para ler as entradas(inputs) dos dados e a função print para imprimir a saída (output) de dados e já pula uma linha ("\n")
// Abaixo segue um exemplo de código que você pode ou não utilizar

let line = gets().split(" ");
let A = parseInt(line[0]);
let B = parseInt(line[1]);

//TODO: Complete os espaços em branco com uma possível solução para o desafio

let total = A + B ; 
print("X = " + total);


2.Desafio - Multiplicação simples

Você receberá dois valores inteiros. Faça a leitura e em seguida calcule o produto entre estes dois valores. Atribua esta operação à variável PROD, mostrando esta de acordo com a mensagem de saída esperada (exemplo abaixo).   

Entrada
A entrada contém 2 valores inteiros.

Saída
Exiba a variável PROD conforme exemplo abaixo, tendo obrigatoriamente um espaço em branco antes e depois da igualdade.

Resposta

// a função gets é implementada dentro do sistema para ler as entradas(inputs) dos dados e a função print para imprimir a saída (output) de dados e já pula uma linha ("\n")
// Abaixo segue um exemplo de código que você pode ou não utilizar

let valor1 = parseInt(gets());
let valor2 = parseInt(gets());

//TODO: Complete os espaços em branco com uma possível solução para o desafio

let total = valor1 * valor2 ;
print("PROD = " + total      );

3. Desafio - Folha de pagamento

Precisamos saber quanto uma determinada empresa deve pagar para seus colaboradores, porém temos apenas a quantidade de horas trabalhadas e o valor hora. Escreva um programa que leia o número de um colaborador, seu número de horas trabalhadas, o valor que recebe por hora e calcula o salário desse colaborador. Em seguida, apresente o número e o salário do colaborador, com duas casas decimais.

Entrada
Você receberá 2 números inteiros e 1 número com duas casas decimais, representando o número, quantidade de horas trabalhadas e o valor que o funcionário recebe por hora trabalhada.

Saída
Exiba o número e o salário do colaborador, conforme exemplo abaixo, com um espaço em branco antes e depois da igualdade. No caso do salário, também deve haver um espaço em branco após o $.

Resposta 

// a função gets é implementada dentro do sistema para ler as entradas(inputs) dos dados e a função print para imprimir a saída (output) de dados.
// Abaixo segue um exemplo de código que você pode ou não utilizar

let valor1 = parseInt(gets());
let valor2 = parseInt(gets());
let valor3 = parseFloat(gets());

//Complete os espaços em branco com uma possível solução para o problema
let salary = parseFloat(valor2 * valor3).toFixed(2);

console.log("NUMBER = " + valor1);
console.log("SALARY = U$ " + salary);


