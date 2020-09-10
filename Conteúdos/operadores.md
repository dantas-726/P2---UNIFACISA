> Operadores

> OPERADORES DE ATRIBUIÇÃO

é utilizado para definir o valor inicial ou sobrescrever o valor de uma variável. 
Em seu uso, o operando à esquerda representa a variável para a qual desejamos atribuir o valor informado à direita.

> EXEMPLO DE USO:

int lado = 2;
float pi = 3,14;
String texto = "PedroHenrique"
lado = 2;

> OPERADORES ARITMÉTICOS

Os operadores aritméticos realizam as operações fundamentais da matemática entre duas variáveis e retornam o resultado.
Caso seja necessário escrever operações maiores ou mais complexas, podemos combinar esses operadores e criar expressões, 
o que nos permite executar todo tipo de cálculo de forma programática.

> EXEMPLO DE USO:

int area = 2 * 2;

Esse código demonstra como calcular a área de um quadrado de lado igual a 2.

Também podemos utilizar os operadores aritméticos em conjunto com o operador de atribuição, realizando, 
em uma mesma instrução, as ações de calcular o valor e atribuí-lo à variável.

>EXEMPLO DE USO:

int area = 2;
area *= 2;

> OPERADORES ARITMÉTICOS OPÇÕES
+ Operador de adição;
- Operador de subtração;
* Operador de multiplicação;
/ Operador de divisão;
% Operador de módulo ou resto da divisão;


> OPERADORES DE INCREMENTO E DECREMENTO

Os operadores de incremento e decremento também são bastante utilizados.
Basicamente temos dois deles: ++ e --, os quais podem ser declarados antes ou depois da variável e incrementam ou decrementam em 1 o valor da variável.

> EXEMPLO DE USO:

int desafioUm = 5;
System.out.println(desafioUm += ++desafioUm );


int desafioDois = 5;
System.out.println(desafioDois += desafioDois++ );

Quais valores serão impressos no console? 10 e 10, 10 e 11, 11 e 10 ou 11 e 11? A resposta é 11 e 10.

No primeiro println(), desafioUm é incrementado antes de seu valor ser lido para compor a instrução de soma. 
Sendo assim, temos desafioUm = 5 + 6. Já no segundo println(), primeiro o valor é lido, resultando em desafioDois = 5 + 5.
Somente após a leitura desafioDois é incrementado, e depois, recebe o valor da soma, tendo seu valor sobrescrito com o número 10.

> OPERADORES DE IGUALDADE

== Utilizado quando desejamos verificar se uma variável é igual a outra. 
 	
!=  Utilizado quando desejamos verificar se uma variável é diferente de outra.

Os operadores de igualdade verificam se o valor ou o resultado da expressão lógica à esquerda é igual (“==”) ou diferente (“!=”) ao da direita, 
retornando um valor booleano.

> EXEMPLO DE USO: 

int valorA = 1;
int valorB = 2;

if(valorA == valorB){
                System.out.println(“Valores iguais”);
} else {
                System.out.println(“Valores diferentes”);
                
               
               
> OPERADORES RELACIONAIS
Os operadores relacionais, assim como os de igualdade, avaliam dois operandos. 
Neste caso, mais precisamente, definem se o operando à esquerda é menor, menor ou igual, maior ou maior ou igual ao da direita, retornando um valor booleano.

int valorA = 1;
int valorB = 2;

if (valorA > valorB) {
                System.out.println(“maior”);
}

if (valorA >= valorB) {
                System.out.println(“maior ou igual”);
}

if (valorA < valorB) {
                System.out.println(“menor”);
}

if (valorA <= valorB) {
                System.out.println(“menor ou igual”);
}



">"  Utilizado quando desejamos verificar se uma variável é maior que outra.

">=" Utilizado quando desejamos verificar se uma variável é maior ou igual a outra.
"<"  Utilizado quando desejamos verificar se uma variável é menor que outra.
"<=" Utilizado quando desejamos verificar se uma variável é menor ou igual a outra.

> OPERADORES LÓGICOS

Os operadores lógicos representam o recurso que nos permite criar expressões lógicas maiores a partir da junção de duas ou mais expressões. 
Para isso, aplicamos as operações lógicas E (representado por “&&”) e OU (representado por “||”).

> EXEMPLO DE USO:
if((1 == (2 -1)) && (2 == (1 + 1))){
     System.out.println(“Ambas as expressões são verdadeiras”);
}

Uma vez que utilizamos o operador lógico &&, o System.out.println somente será executado se as duas condições declaradas no if forem verdadeiras.

&&  - Utilizado quando desejamos que as duas expressões sejam verdadeiras.
|| -  Utilizado quando precisamos que pelo meno um das expressões seja verdadeira.

> PRECEDÊNCIA DE OPERADORES

Uma vez que os operadores aritméticos buscam reproduzir as operações matemáticas fundamentais,
é natural que eles mantenham as suas regras de precedência, que podem ser manipuladas pelo programador com o uso de parênteses.
Por exemplo, a expressão 1 + 1 * 2, quando analisada pelo compilador, vai retornar o valor 3, porque a multiplicação será resolvida antes da adição. 
Usando parênteses, a expressão (1 + 1) * 2 retornará o valor 4, pois a adição, por estar dentro dos parênteses, será resolvida primeiro.

> EXEMPLO DE USO:


if ((1 != (2 -1)) || (2 == (1+1))) {
  System.out.println(“iguais”);
}



> EXEMPLO PRÁTICO

Suponha que você precisa programar um código simples para definir o salário dos funcionários de uma empresa considerando o tempo que cada um tem nessa empresa 
e o número de horas trabalhadas. Para tanto, podemos utilizar alguns dos operadores apresentados nessa documentação.

int quantidadeAnos = 5;
int horasTrabalhadas = 40;
int valorHora = 50;
int salario = 0;

if (quantidadeAnos <= 1) {
    salario = 1500 + (valorHora * horasTrabalhadas);
} else if ((quantidadeAnos > 1) && (quantidadeAnos < 3)) {
    salario = 2000 + (valorHora * horasTrabalhadas);
} else {
    salario = 3000 + (valorHora * horasTrabalhadas);
}
                
        
                
                
            


