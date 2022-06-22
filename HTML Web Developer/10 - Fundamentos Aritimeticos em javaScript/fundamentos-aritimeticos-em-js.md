1.Desafio - Quantidade de numeros positivos

Crie um programa que leia 6 valores, os quais poderão ser negativos e/ou positivos. Em seguida, apresente a quantidade de valores positivos digitados.

Entrada
Você receberá seis valores, negativos e/ou positivos.

Saída
Exiba uma mensagem dizendo quantos valores positivos foram lidos. assim como é exibido abaixo no exemplo de saída. Não se esqueça de incluir na mensagem de saída o sufixo " valores positivos", conforme o exemplo abaixo:

Resposta 

// a função gets é implementada dentro do sistema para ler as entradas(inputs) dos dados e a função print para imprimir a saída (output) de dados e já pula uma linha ("\n")
// Abaixo segue um exemplo de código que você pode ou não utilizar

let quantidadePositivos = 0;

for (let i = 0; i < 6; i++) {

 const valorInformadoPeloUsuario = gets();

 if (valorInformadoPeloUsuario > 0){

   quantidadePositivos=quantidadePositivos+1;

 }

 else {}

//TODO: Complete os espaços em branco com uma possível solução para o desafio


}

print(`${quantidadePositivos} valores positivos`);

2.Desafios - exibindo numeros pares

Crie um programa que leia um número e mostre os números pares até esse número, inclusive ele mesmo.

Entrada
Você receberá 1 valor inteiro N, onde N > 0.

Saída
Exiba todos os números pares até o valor de entrada, sendo um em cada linha. 

Resposta

var valor = 0;

 valor = gets();
  
   for (let i = 1; i <= valor; i++){
      if (i % 2 === 0) {
          console.log(i);
      }
  };

3.Desafio - Analise de numeros

Você deve fazer a leitura de 5 valores inteiros. Em seguida mostre quantos valores informados são pares, quantos valores informados são ímpares, quantos valores informados são positivos e quantos valores informados são negativos. Considere que o número zero é positivo, mas não pode ser considerado como positivo ou negativo.

Entrada
Você receberá 5 valores inteiros.

Saída
Exiba a mensagem conforme o exemplo de saída abaixo, sendo uma mensagem por linha e não esquecendo o final de linha após cada uma.

Resposta

let valoresPares = 0;
let valoresImpares = 0;
let valoresPositivos = 1;
let valoresNegativos = 3;

for (var i = 0; i < 5; i++) {
  const valorInformadoPeloUsuario = parseInt(gets());

  // TODO: Complete os espaços em branco com uma solução possível para o problema.
 
  if ( valorInformadoPeloUsuario % 2 == 0) {
  
    valoresPares++; 
    
  }
    
  else if (valorInformadoPeloUsuario  % 2 != 0 ) {  
    
    valoresImpares++;
  }

  else if (valorInformadoPeloUsuario > 0) {
    
  }

else if (valorInformadoPeloUsuario < 0) {
    
  }

}

console.log(`${valoresPares} par(es)`);
console.log(`${valoresImpares} impar(es)`);
console.log(`${valoresPositivos} positivo(s)`);
console.log(`${valoresNegativos} negativo(s)`);


4.Desafio - contagem de cedulas
Faça a leitura de um valor inteiro. Em seguida, calcule o menor número de notas possíveis (cédulas) onde o valor pode ser decomposto. As notas que você deve considerar são de 100, 50, 20, 10, 5, 2 e 1. Na sequência mostre o valor lido e a relação de notas necessárias.

Entrada
Você receberá um valor inteiro N (0 < N < 1000000).

Saída
Exiba o valor lido e a quantidade mínima de notas de cada tipo necessárias, seguindo o exemplo de saída abaixo. Após cada linha deve ser imprimido o fim de linha.

Resposta

let n = parseInt(gets());
let quantidadeNotas = 0;
let cedulas = [100,50,20,10,5,2,1];

// Função responsável por contar as notas a partir de um valor.
function contaNotas(valor){
  quantidadeNotas = parseInt(n/valor);

  // TODO Subtraia de "n" a "quantidadeNotas" multiplicada por seu respectivo "valor" (parâmetro).
  n -= quantidadeNotas*valor;

  console.log(`${quantidadeNotas} nota(s) de R$ ${valor},00`);
}

console.log(n);

for(let cedula in cedulas){
    contaNotas(cedulas[cedula]);
}



5.Desafio - Consuma medio do automovel
Você deve calcular o consumo médio de um automóvel onde será informada a distância total percorrida (em Km) e o total de combustível consumido (em litros).

Entrada
Você receberá dois valores: um valor inteiro X com a distância total percorrida (em Km), e um valor real Y que representa o total de combustível consumido, com um dígito após o ponto decimal.

Saída
Exiba o valor que representa o consumo médio do automóvel (3 casas após a vírgula), incluindo no final a mensagem "km/l".

Resposta

let X = parseInt(gets());
let Y = parseFloat(gets());
let consumoMedio = parseFloat(X / Y).toFixed(3);

console.log(consumoMedio + " km/l");