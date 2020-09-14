> ESTRUTURAS CONDICIONAIS:

Estruturas condicionais e de repetição são fundamentais para a maioria das linguagens de programação. 
Sem elas, as instruções dos programas seriam executadas sequencialmente sem nenhum tipo de reaproveitamento ou ramificação.
Não é difícil imaginar o quanto seria trabalhoso escrever programas assim.

Felizmente, a linguagem Java está entre as linguagens que oferecem suporte a estruturas condicionais e de repetição, mas é importante lembrar que a estrutura sequencial 
também faz parte da linguagem Java.
Isto significa que, se nenhuma estrutura de repetição ou condição for utilizada, as instruções em Java serão executadas uma após a outra, na ordem em que são escritas.


> if/else


A estrutura condicional if/else permite ao programa avaliar uma expressão como sendo verdadeira ou falsa e, de acordo com o resultado dessa verificação, executar uma ou outra rotina.

Na linguagem Java o tipo resultante dessa expressão deve ser sempre um boolean, pois diferentemente das demais, o Java não converte null ou inteiros como 0 e 1 para os valores 
true ou false.


> else if 

Complementar ao if/else temos o operador else if. Esse recurso possibilita adicionar uma nova condição à estrutura de decisão para atender a lógica sendo implementada.



> EXEMPLO DE USO:

Suponha que você está desenvolvendo um software para controle de estoque que precisa informar como está a quantidade de itens de cada produto: se suficiente, para quantidades superiores a 100; em alerta, para quantidades entre 100 e 50; e abaixo do ideal, para quantidades menores do que 50. Como programar esse código?

Exemplo de uso de if/else:

int estoque = //valor recuperado do sistema

if (estoque >= 100) {

	System.out.println(“Produto com quantidade suficiente.”);
  
} else if (estoque < 100 && estoque > 50) {

	System.out.println(“Alerta: Avaliar possibilidade de novo pedido.”);
} else {

	System.out.println(“ATENÇÃO! Faça um novo pedido.”);
  
  
  Agora, considere que você precisa de uma estrutura de decisão mais simples, apenas para indicar se estamos na primeira ou na segunda quinzena de um mês.

> EXEMPLO DE USO:

int numeroDias = //valor entre 1 e 30

System.out.println((numeroDias <= 15) ? “Primeira quinzena” : “Segunda quinzena”)
