> ESTRUTURAS DE REPETIÇÃO:

Assim, as estruturas de repetição que também são conhecidas como iteração, ou laços (loops), são utilizadas para executar, repetidamente, uma instrução ou um bloco 
de instruções enquanto determinada condição estiver sendo satisfeita.

As estruturas while e for processam uma instrução ou grupo de instrução, zero ou mais vezes, se a condição de continuação do loop for verdadeira ou 
enquanto ela for verdadeira, mas se esta condição for falsa a ação não será executada. O do… while, processa uma instrução ou grupo de instruções uma ou mais vezes.

Cada sistema ou programa de computador faz uso de quantas combinações de estruturas de repetição e/ou estruturas de decisão forem necessárias. 
E toda estrutura de repetição compõem-se de quatro elementos, a saber, inicialização, condição, corpo e interação.

A inicialização em estruturas de repetição é o primeiro passo em sua formatação. A expressão condicional em si é, assim como nas estruturas de decisão uma expressão booleana que é avaliada a cada iteração, para determinar se haverá ou não uma nova iteração. O corpo pode ser composto por uma única instrução ou um conjunto de instruções. A iteração é instrução booleana que deverá ser executada depois do corpo e antes de uma nova repetição.

> ESTRUTURA DE REPETIÇÃO WHILE:

Uma estrutura de repetição while, que em português significa enquanto, especifica que um sistema ou programa de computador deve repetir uma instrução 
ou um conjunto de instruções enquanto a condição que é uma expressão booleana permanece verdadeira.

> EXEMPLO:

num = 0;

while (num < 100){

       System.out.println("Formação Java web");
       num++;
       
}


> ESTRUTURA DE REPETIÇÃO DO… WHILE

Você já deve imaginar que a estrutura de repetição do… while é uma variação da while. 
A principal diferença entre elas é que, como já dissemos, o while processa uma instrução ou grupo de instrução, zero ou mais vezes, ao passo que o do…while 
processa uma instrução, obrigatoriamente pelo menos uma vez, e se necessário outras tantas vezes.

Assim, implica que o corpo da estrutura, ou seja, o bloco de instrução será executado pelo menos uma vez 
antes que a condição do loop seja testada. Nosso pseudocódigo ficaria assim:

num = 0

do{

   System.out.println("Formação Java web");
   
   num+-+;
   
}while (num < 100);


> ESTRUTURA DE REPETIÇÃO FOR:

O formato da sintaxe da instrução de repetição for fica assim:

Detalhando a estrutura acima temos a palavra reservada for, a variável de controle seguida do seu valor de inicialização,
e então esse bloco do cabeçalho é separado por um ponto e vírgula, 
continuando temos a condição de continuação do loop que é uma expressão booleana, o ponto e vírgula e o incremento.

> EXEMPLO:

for(int num = 0; num < 10; num++){

   System.out.println("Formação Java web");
   
} 

Note que dessa vez não foi necessário declarar a variável “num” fora da estrutura, nós a declaramos localmente dentro do cabeçalho do for. 
Obviamente haverá algumas restrições quanto ao uso dessa variável fora do laço de repetição.

> EM POUCAS PALAVRAS]

Antes de fazermos um resumo do que aprendemos sobre as estruturas de repetição, como dizia Steve Jobs, “só mais uma coisa”, recomenda-se 
usar o for quando já soubermos a quantidade de vezes que uma dada instrução deverá ser repetida, 
e o while quando não soubermos exatamente, porém, neste caso, impomos uma condição de parada.

E ainda, existe uma situação qual chamamos de repetição definida, esta situação ocorre quando o número de execuções é antecipadamente conhecido, ou seja, 
a quantidade de repetições é conhecida antes do loop começar.
Esta repetição definida, pode acontecer também com o while. 
Mas recomendamos que você adote as boas práticas de programação e principalmente o bom senso.

O nosso “Em poucas palavras” de hoje se estendeu um pouco, mas foi por uma boa causa, aprendemos hoje sobre os laços de repetição, while, do…while e for 
e o poder dessas três estruturas. 
