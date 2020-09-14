Para utilizar a classe Scanner em uma aplicação Java deve-se proceder da seguinte maneira:

>[ 1 ]	importar o pacote java.util:

import java.util.Scanner;

>[ 2 ]	Instanciar e criar um objeto Scanner:

Scanner ler = new Scanner(System.in);

>[ 3 ]	Lendo valores através do teclado:

>[ 3.1 ]	Lendo um valor inteiro:

int n;

System.out.printf("Informe um número para a tabuada: ");

n = ler.nextInt();

>[ 3.2 ]	Lendo um valor real:

float preco;


System.out.printf("Informe o preço da mercadoria = R$ ");

preco = ler.nextFloat();

>[ 3.3 ]	Lendo um valor real:

double salario;


System.out.printf("Informe o salário do Funcionário = R$ ");

salario = ler.nextDouble();

>[ 3.4 ]	Lendo uma String, usado na leitura de palavras simples que não usam o caractere de espaço (ou barra de espaço):

String s;


System.out.printf("Informe uma palavra simples:\n");

s = ler.next();

>[ 3.5 ]	Lendo uma String, usado na leitura de palavras compostas, por exemplo, Pato Branco:

String s;

System.out.printf("Informe uma cadeia de caracteres:\n");

s = ler.nextLine();

>[ 3.6 ]	Na leitura consecutiva de valores numéricos e String deve-se esvaziar o buffer do teclado antes da leitura do valor String, por exemplo:

int n;

String s;


System.out.printf("Informe um Número Inteiro: ");

n = ler.nextInt();


ler.nextLine(); // esvazia o buffer do teclado


System.out.printf("Informe uma cadeia de caracteres:\n");

s = ler.nextLine();

>[ 3.7 ]	Lendo um caractere usando o método read() do pacote de classes System.in:

public static void main(String args[]) throws Exception {

char c;


System.out.printf("Informe um Caractere: ");

c = (char)System.in.read();

}

> Método printf()

Outra novidade no Java 1.5 foi a incorporação da função printf() do C como um método do pacote de classes System.out.

O método printf(), utilizado para realizar uma saída de dados no fluxo de saída padrão System.out, tem a seguinte forma geral:

System.out.printf(<em>expressão_de_controle</em>, argumento1, argumento2, ...);

A expressão_de_controle deve ser uma sequência de caracteres (portanto, delimitada por aspas duplas) 
que determina as informações que serão mostradas na tela. 
Nesta expressão podem existir dois tipos de informações: caracteres comuns e códigos de controle (ou especificadores de formato). 
Os códigos de controle, mostrados na Tabela 1, são precedidos por um % e são aplicados aos argumentos na mesma ordem em que aparecem.


%c	Caractere simples (char)

%s	Cadeia de caracteres (String)

%d	Inteiro decimal com sinal (int)

%i	Inteiro decimal com sinal (int)

%ld	Inteiro decimal longo (long)

%f	Real em ponto flutuante (float ou double)

%e	Número real em notação científica com o "e" minúsculo (float ou double)

%E	Número real em notação científica com o "E" maiúsculo (float ou double)

%%	Imprimir o próprio caractere %

> Aplicações Java
Para demonstrar a utilização dos métodos da classe Scanner do pacote java.util em operações de entrada de dados e do método printf() na formatação da saída 
através da utilização de códigos de controle foram implementadas as seguintes aplicações Java:

import java.util.Scanner; // 1. importando a classe Scanner


public class Exemplo1 {


  public static void main(String[] args) {
// 2. instanciando e criando um objeto Scanner

    Scanner ler = new Scanner(System.in);
    

    int i, n;
    

    System.out.printf("Informe o número para a tabuada:\n");
    
    n = ler.nextInt(); // 3.1 entrada de dados (lendo um valor inteiro)

    System.out.printf("\n+--Resultado--+\n");
    
    for (i=1; i<=10; i++) {
    
      System.out.printf("| %2d * %d = %2d |\n", i, n, (i*n));
      
    }
    
    System.out.printf("+-------------+\n");    
  }

}

> EXEMPLO TABUADA DE UM NÚMERO: 

import java.util.Scanner; // 1. importando a classe Scanner


public class Exemplo2 {


  public static void main(String args[]) {
// 2. instanciando e criando um objeto Scanner

    Scanner ler = new Scanner(System.in);

    double pc, alt, vlrIMC;

    System.out.printf("Informe o Peso Corporal em kg: ");
    pc = ler.nextDouble(); // 3.3 entrada de dados (lendo um valor real)

    System.out.printf("Informe a Altura em metros...: ");
    alt = ler.nextDouble(); // 3.3 entrada de dados (lendo um valor real)

    System.out.printf("\n========================================\n");
    vlrIMC = IMC(pc, alt);
    System.out.printf("IMC = %.2f (%s)\n", vlrIMC, interpretacaoIMC(vlrIMC));
    System.out.printf("========================================\n");
  }

  public static double IMC(double pc, double alt) {
  
    return(pc / (alt * alt));
    
  }

  public static String interpretacaoIMC(double vlrIMC) {
  
    if (vlrIMC < 20)
       return("Magro");
       
    else if ((vlrIMC >= 20) && (vlrIMC <= 24))
        return("Normal");
         else if ((vlrIMC >= 25) && (vlrIMC <= 29))
                 return("Acima do peso");
               else if ((vlrIMC >= 30) && (vlrIMC <= 34))
                  return("Obeso");
               else // acima de 34
                     return("Muito obeso");
  }
}

> EXEMPLO IMC:

import java.io.IOException;

import java.util.Scanner; // 1. importando a classe Scanner

public class Exemplo3 {

// através da cláusula throws indicamos que não iremos
// tratar possíveis erros na entrada de dados realizada
// através do método "read" do pacote de classes System.in
  public static void main(String[] args) throws IOException {
// 2. instanciando e criando um objeto Scanner
    Scanner ler = new Scanner(System.in);

    String nome;
    char sexo;

    System.out.printf("Informe um nome:\n");
    nome = ler.nextLine(); // 3.5 entrada de dados (lendo uma String)

    System.out.printf("\nInforme o sexo (M/F): ");
// 3.7 entrada de dados (lendo um caractere)
    sexo = (char)System.in.read();

    System.out.printf("\nResultado:\n");
    if ((sexo == 'M') || (sexo == 'm'))
       System.out.printf("Seja bem vindo Sr. \"%s\".\n", nome);
    else System.out.printf("Seja bem vinda Sra. \"%s\".\n", nome);
  }

}

 > ENTRADA DE DADOS DO TIPO CARACTERE:
 
 public class Exemplo4 {
 
  public static void main(String[] args) {
  
    String nomeMes[] = {"Janeiro", "Fevereiro", "Março",
      "Abril", "Maio", "Junho", "Julho", "Agosto",
      "Setembro", "Outubro", "Novembro", "Dezembro"};

    System.out.println("================");
    System.out.println("Mês- Nome do Mês");
    System.out.println("================");
    for (int i=0; i<12; i++) {
      System.out.printf(" %0,2d- %s\n", (i+1), nomeMes[i]);
    }
    System.out.println("================");
  }

}

