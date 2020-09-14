# Classes e Objetos

Uma classe é um elemento do código Java que utilizamos para representar objetos do mundo real. 
Dentro dela é comum declararmos atributos e métodos, que representam, respectivamente, as características e comportamentos desse objeto. 
Neste documento será apresentado como declarar e utilizar uma classe em Java.

> SINTAXES

A declaração de uma classe em Java é bastante simples. 
Utilizamos a palavra reservada class seguida pelo nome da classe. Logo após, entre chaves, definimos os elementos a ela 
relacionados: atributos, construtores e métodos. 
Sintaxe de declaração de classe:

<modificador de acesso> class NomeDaClasse {


  // Local onde atributos, construtores e métodos são criados
  

}

Note que também é possível especificar o modificador de acesso.
Por meio dele informamos a visibilidade da classe, que pode ser public, private ou default.

Exemplo de declaração de classe:


public class Produto {


  private String nome;
  
  private int quantidade;
  

  public Produto() {
    // Código do construtor
    
  }

  public void apresentarProduto() {
    // Código do método
    
  }


}


Este exemplo apresenta o código da classe Produto. Como foi declarada como public, poderá ser utilizada por todas as classes do projeto. Além disso, ela possui dois atributos (nome e quantidade), um construtor sem argumentos e um método.

> REGRAS PARA NOMEAÇÃO DE CLASSES:

Ao nomear uma classe algumas convenções devem ser seguidas:

Manter o nome simples e descritivo;

Usar palavras inteiras, isto é, sem siglas e abreviações;

A primeira letra de cada palavra deve estar em caixa alta.

200
200

Marcar como concluído
 
Anotar
Artigos
Java
Java: Declaração e utilização de classes
Uma classe é um elemento do código Java que utilizamos para representar objetos do mundo real. Dentro dela é comum declararmos atributos e métodos, que representam, respectivamente, as características e comportamentos desse objeto. Neste documento será apresentado como declarar e utilizar uma classe em Java.

Sintaxe
A declaração de uma classe em Java é bastante simples. Utilizamos a palavra reservada class seguida pelo nome da classe. Logo após, entre chaves, definimos os elementos a ela relacionados: atributos, construtores e métodos. Sintaxe de declaração de classe:

<modificador de acesso> class NomeDaClasse {

  // Local onde atributos, construtores e métodos são criados

}
Note que também é possível especificar o modificador de acesso. Por meio dele informamos a visibilidade da classe, que pode ser public, private ou default.

Exemplo de declaração de classe:

public class Produto {

  private String nome;
  private int quantidade;

  public Produto() {
    // Código do construtor
  }

  public void apresentarProduto() {
    // Código do método
  }

}
Este exemplo apresenta o código da classe Produto. Como foi declarada como public, poderá ser utilizada por todas as classes do projeto. Além disso, ela possui dois atributos (nome e quantidade), um construtor sem argumentos e um método.

Regras para nomeação de classes
Ao nomear uma classe algumas convenções devem ser seguidas:

Manter o nome simples e descritivo;
Usar palavras inteiras, isto é, sem siglas e abreviações;
A primeira letra de cada palavra deve estar em caixa alta.
Como utilizar
Para utilizar uma classe devemos declará-la da mesma maneira que se declara uma variável de tipo primitivo. Declaramos o tipo (neste caso o nome da classe) seguido pelo nome da variável.

>Exemplo de instanciação de classe:

Produto produtoUm;

produtoUm = new Produto();

produtoUm.apresentarProduto();

A segunda linha deste código representa o processo de instanciação de uma classe. Na linha anterior, a variável produtoUm foi definida como sendo do tipo Produto. 
Em seguida, com a palavra reserva new, um espaço é criado na memória para armazenar um novo objeto do tipo Produto. 
O construtor Produto() especifica como o objeto deve ser criado. Por fim, uma referência a esse objeto é atribuída à variável produtoUm.

Assim, através de produtoUm podemos acessar o objeto criado (e seus atributos e métodos).

Na terceira linha, por exemplo, utilizando a variável, acessamos o objeto e chamamos o método apresentarProduto().

Apesar do exemplo acima, o código para criar um objeto e definir a variável que conterá sua referência normalmente é declarado em apenas uma linha.

> Exemplo de instanciação de classe:

Produto produtoUm = new Produto();

200

Marcar como concluído
 
Anotar
Artigos
Java
Java: Declaração e utilização de classes
Uma classe é um elemento do código Java que utilizamos para representar objetos do mundo real. Dentro dela é comum declararmos atributos e métodos, que representam, respectivamente, as características e comportamentos desse objeto. Neste documento será apresentado como declarar e utilizar uma classe em Java.

Sintaxe
A declaração de uma classe em Java é bastante simples. Utilizamos a palavra reservada class seguida pelo nome da classe. Logo após, entre chaves, definimos os elementos a ela relacionados: atributos, construtores e métodos. Sintaxe de declaração de classe:

<modificador de acesso> class NomeDaClasse {

  // Local onde atributos, construtores e métodos são criados

}
Note que também é possível especificar o modificador de acesso. Por meio dele informamos a visibilidade da classe, que pode ser public, private ou default.

Exemplo de declaração de classe:

public class Produto {

  private String nome;
  private int quantidade;

  public Produto() {
    // Código do construtor
  }

  public void apresentarProduto() {
    // Código do método
  }

}
Este exemplo apresenta o código da classe Produto. Como foi declarada como public, poderá ser utilizada por todas as classes do projeto. Além disso, ela possui dois atributos (nome e quantidade), um construtor sem argumentos e um método.

Regras para nomeação de classes
Ao nomear uma classe algumas convenções devem ser seguidas:

Manter o nome simples e descritivo;
Usar palavras inteiras, isto é, sem siglas e abreviações;
A primeira letra de cada palavra deve estar em caixa alta.
Como utilizar
Para utilizar uma classe devemos declará-la da mesma maneira que se declara uma variável de tipo primitivo. Declaramos o tipo (neste caso o nome da classe) seguido pelo nome da variável.

Exemplo de instanciação de classe:

Produto produtoUm;
produtoUm = new Produto();
produtoUm.apresentarProduto();
A segunda linha deste código representa o processo de instanciação de uma classe. Na linha anterior, a variável produtoUm foi definida como sendo do tipo Produto. Em seguida, com a palavra reserva new, um espaço é criado na memória para armazenar um novo objeto do tipo Produto. O construtor Produto() especifica como o objeto deve ser criado. Por fim, uma referência a esse objeto é atribuída à variável produtoUm.

Assim, através de produtoUm podemos acessar o objeto criado (e seus atributos e métodos). Na terceira linha, por exemplo, utilizando a variável, acessamos o objeto e chamamos o método apresentarProduto().

Apesar do exemplo acima, o código para criar um objeto e definir a variável que conterá sua referência normalmente é declarado em apenas uma linha.

Exemplo de instanciação de classe:

Produto produtoUm = new Produto();

> Extends

Quando uma classe precisa herdar características de outra, fazemos uso de herança, conceito da orientação a objetos que em Java é representado pela palavra-chave extends.

Sintaxe de declaração de herança:

public class MinhaClasse extends ClasseQualquer {

}

Com extends, todos os atributos e métodos não-privados de ClasseQualquer serão herdados por MinhaClasse.
Por isso, é comum dizer que a classe herdada (ClasseQualquer) é pai da classe que herdou seus elementos (MinhaClasse).

Exemplo de herança em Java:

public class Produto {

  public double valorCompra;
  
  protected double valorVenda;

}

public class Computador extends Produto {

   private String processador;

}

