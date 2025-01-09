# Calculando-juros-de-um-boleto-atrasado
import leitor from 'readline-sync';

console.log("Aplicando Juros\n");
let valor_devido = leitor.question("Qual o valor do boleto? ");
let dias_vencidos = leitor.question("Quantos dias que venceu o boleto? ");

console.log("Valor original do boleto: R$"+valor_devido);
console.log("Dias atrasados:"+ dias_vencidos);
let taxa = (dias_vencidos > 15) ? 0.1:0.05;
console.log("A taxa devido a quantidade de dias atrasados foi: "+taxa);
let valor_final = valor_devido * (1 + taxa);
console.log("O boleto no final com juros: R$ "+valor_final)
