# resumo-estudo-logica-de-programacao
Repositório com resumos sobre lógica de programação e alguns exemplos de código

## 1 - O que é algoritmo?
Algoritmo nada mais é do que um conjunto de instruções para atingir um objetivo. Em todo algoritmo você terá:

Entrada → Processamento → Saída 

## 2 - O que é pseudocódigo?
Pseudocódigo é uma forma de você descrever um algoritmo usando uma linguagem simples, uma linguagem natural. O português e inglês são exemplos de linguagens naturais.

## 3 -  O que é linguagem de programação?
É um conjunto de regras e instruções usando uma semântica padronizada que permite a comunicação entre uma pessoa e uma máquina possibilitando gerar uma série de ordens, ações para criar programas que vão controlar o comportamento de uma máquina.

### O que seria uma linguagem de máquina?

É uma linguagem que o computador fala, a forma mais primitiva, constituído por código binário (0 e 1).

0 → circuito fechado

1 → circuito aberto

### O que seria linguagens de baixo nível?

São linguagens mais próximas da linguagem de máquina (difícil entendimento para o ser humano) a vantagem disso é que essas linguagens são mais rápidas (são usadas em sistemas embarcados por exemplo). Um exemplo é a linguagem Assembly.

### O que seria linguagens de alto nível?

São linguagens feitas para seres humanos (é mais fácil para entender a linguagem) e a maioria será convertida em linguagem de máquina para o computador. Um exemplo é a linguagem Java.

Para cada linguagem você precisa seguir a sintaxe, se você não seguir a sintaxe o computador não vai conseguir te entender. 

## 4 - O que é uma variável?
É um objeto (uma posição, frequentemente localizada na memória) capaz de reter e representar um valor ou expressão. É uma forma de armazenar dados no nosso código e dependendo do jeito q você declara a variável, o valor pode ou não ser alterado.

Link para consulta: https://embarcados.com.br/tipos-de-dados/

## 5 - O que são tipos de dados?
Um tipo de dados representa as características de uma variável que determina que tipo de dados ela pode conter.

Exemplo tipos de dados primitivos: 

<incluir imagem do vídeo do willian suane>

### Tipos de dados primitivos:

Essas variáveis guardam valores. Exemplo: números. Tipos de dados byte, short, int, long, float, double e boolean char String.

### Tipos de dados não primitivos:

A aplicação guarda o endereço em memória e não o valor em si. Importantes casos são as arrays e os objetos. Exemplos Arrays e Classes 

Mais informações ver site do w3school.

### A principal diferença entre tipos de dados primitivos e não primitivos são:

Os tipos primitivos são predefinidos (já definidos) em Java. Tipos não primitivos são criados pelo programador e não são definidos por Java (exceto para String).
Tipos não primitivos podem ser usados para chamar métodos para realizar determinadas operações, enquanto tipos primitivos não podem.
Um tipo primitivo sempre tem um valor, enquanto os tipos não primitivos podem ser null.
Um tipo primitivo começa com uma letra minúscula, enquanto os tipos não primitivos começam com uma letra maiúscula.

## 6 - O que são constantes?
Ao contrário das variáveis, que podemos alterar o valor conforme a necessidade do algoritmo a ser desenvolvido, as constantes precisam ser inicializadas e não podem ter o seu valor alterado.

Uma constante é uma variável!! Sim, é uma variável no sentido de que uma constante também reserva um espaço de memória para o tipo de dado que manipulará. Entretanto, uma constante armazenará um valor ÚNICO, um valor que NÃO mudará com o tempo de execução do programa.

Jeito de explicar da Vi: Uma constante é uma variável no sentido que a constante ela também reserva um espaço de memória para o tipo de dado que manipulará. Porém uma constante armazenará um valor ÚNICO, um valor que NÃO mudará com o tempo de execução do programa.

## 7 - Como atribuir valores?
A atribuição de valor é a passagem de informação a determinada variável. O operador de atribuição básico é o "=" (sinal de igual). 
```
int idade = 20;
```
O valor atribuído a variável idade é 20. 
Você também pode usar operadores combinados:
```
int idade = 20;

idade += 10; // Nesse caso ele adiciona um valor a variável existente(20).
```
Se imprimir com System.out.println(idade); // O resultado será 30.

## 8 - Comentários
Existem 3 tipos de comentários no Java:
```
// Comentário em uma linha
```

```
/* 
Isso é 
um comentário 
de múltiplas linhas 
*/
```

```
/**
Isso é um comentário de documentação javadoc
```
## 9 - Entrada e saída de dados
Quando fazemos um programa precisamos pensar numa sequência de passos que devem ser dados para que um problema seja resolvido e essa sequência de passos é chamada de algoritmo, todo algoritmo você terá Entrada - Processamento - Saída

Entrada: Por exemplo o que o usuário digita através do teclado

Processamento: O cálculo que será feito

Saída: Saída de informações na tela do computador 

No Java nós temos um pacote de classes chamado de Java.util e temos a classe Scanner q é uma classe q implementa operações de entrada de dados pelo teclado. E dentro da Scanner temos vários métodos que permitem a entrada de dados de diferentes tipos. Segue exemplo de Entrada e saída de dados:

```
   public static void main(String args[]) {
        
          System.out.println("Digite o seu nome:"); // saída padrão impressa no monitor
         
          String nome; //local que armazena caracteres por exemplo um nome
          Scanner leitura = new Scanner(System.in); // criação do objeto para ler o teclado
          nome = leitura.nextLine(); // entrada padrão, captura o que foi digitado pelo usuário
          
          System.out.println("Olá " + nome + "seja bem vindo(a)");    
          
    }
```


## 10 - Concatenação
Concatenar significa "colocar junto", “juntar-se”, “ligar-se”

Para concatenar duas String, usa-se o método concat.

Note que, já que o tamanho de uma String não pode mudar, a concatenação resulta na criação de um novo objeto.
Também pode-se usar o operador + para a concatenação. Por exemplo, no trecho de código abaixo, a mesma linha é impressa duas vezes:

```
   String s1 = "Olá ";
   String s2 = "Mundo!";
   System.out.println( s1.concat( s2 ) );
   System.out.println( s1 + s2 );
```
https://www.if.ufrgs.br/~betz/jaulas/aula3.htm


## 11 - Operadores aritméticos
Os operadores aritméticos são usados para realizar operações matemáticas básicas. São eles:

"+" (adição)
"-" (subtração)
"*" (multiplicação)
"/" (divisão)
"%" (resto da divisão)

Por exemplo:

```
int a = 10 + 2; // Atribui o valor 12 à variável a
int b = 10 - 2; // Atribui o valor 8 à variável b
int c = 10 * 2; // Atribui o valor 20 à variável c
int d = 10 / 2; // Atribui o valor 5 à variável d
int e = 10 % 3; // Atribui o valor 1 à variável e (o resto da divisão de 10 por 3 é 1)
```


## 12 - Operadores de incremento e decremento
Além dos operadores citados anteriormente, o operador de incremento é usado para aumentar o valor de uma variável em 1. Existem dois tipos de operadores de incremento: o operador de pré-incremento (++variavel) e o operador de pós-incremento (variavel++).

O operador de pré-incremento (++variavel) aumenta o valor da variável em 1 antes de usar a variável em uma expressão. Aqui está um exemplo:

```
int num = 5;
int resultado = ++num; //num é incrementado para 6 e depois atribuído a resultado
System.out.println(num); // imprime 6
System.out.println(resultado); // imprime 6
```

Já o operador de pós-incremento (variavel++) aumenta o valor da variável em 1 depois de usar a variável em uma expressão. Aqui está um exemplo:

```
int num = 5;
int resultado = num++; //num é atribuído primeiramente à variável resultado e depois incrementado para 6
System.out.println(num); // imprime 6
System.out.println(resultado); // imprime 5
```

## 13 - Operadores de igualdade e relacionais
Os operadores relacionais são usados para comparar valores. Eles retornam um valor booleano (verdadeiro ou falso). Trabalharemos melhor com eles quando tivermos na aula de condicionais, onde vamos modificar o fluxo da aplicação dada alguma condição. São eles:

"==" (igual a)
"!=" (diferente de)
">" (maior que)
">=" (maior ou igual a)
"<" (menor que)
"<=" (menor ou igual a)

Exemplo:

```
int a = 10; // Atribui o valor 10 à variável a
int b = 5; // Atribui o valor 5 à variável b
int c = 30; // Atribui o valor 30 à variável c

boolean igual = (b == a); //Nesse caso a variável igual ficará com o valor *false*, pois o valor de b não é igual o valor de a.
boolean diferente = (b != c); //A variável diferente ficará com o valor *true*, pois o valor de b é diferente do valor de c.
boolean maior = (b > a); //A variável maior ficará com o valor *false*, pois o valor de b é menor que o valor de a.
boolean menorIgual = (b <= c); //A variável menorIgual ficará com o valor *true*, pois o valor de b é menor que o valor de c.
```

## 14 - Operadores lógicos
Esses operadores são usados quando queremos verificar duas ou mais condições e/ou expressões na aplicação. Eles fazem a comparação de valores booleanos e retornam também um resultado booleano.

São três operadores: AND (&&), OR (||) e NOT (!).

O operador AND (&&), que traduzindo para o português seria o E, é usado para verificar se duas condições são verdadeiras. Se ambas as condições forem verdadeiras, o resultado será verdadeiro. Caso contrário, o resultado será falso. Aqui está um exemplo:

```
boolean a = true;
boolean b = false;
if (a && b) {
   // Este código não será executado, já que a é verdadeiro e b é falso.
}
```

O operador OR (||), que traduzindo para o português seria o OU, é usado para verificar se pelo menos uma das condições é verdadeira. Se pelo menos uma das condições for verdadeira, o resultado será verdadeiro. Caso contrário, o resultado será falso. Aqui está um exemplo:

```
boolean a = true;
boolean b = false;
if (a || b) {
   // Este código será executado, já que a é verdadeiro, mesmo que b seja falso.
}
```

O operador NOT (!) é usado para negar uma condição. Se a condição for verdadeira, o resultado será falso. Se a condição for falsa, o resultado será verdadeiro. Aqui está um exemplo: 

```
boolean a = true;
if (!a) {
   // Este código não será executado, já que a é verdadeiro.
}
```


## 15 - Precedência de operadores
Os operadores possuem regras que são aplicadas nas expressões aritméticas do Java, que são as mesmas seguidas em álgebra. Quando dizemos que os operadores são aplicados da esquerda para a direita, estamos nos referindo à sua associatividade.

Operadores de multiplicação, divisão e módulo são aplicadas primeiro. Por exemplo, quando aparecer uma expressão com várias dessas operações, elas serão aplicadas da esquerda para a direita.

As operações de adição e subtração são aplicadas em seguida.

Abaixo uma tabela de referência dos operadores e suas ordens de avaliação:

<incluir imagem >

https://www.devmedia.com.br/operadores-logicos-e-matematicos-da-linguagem-java/25248#:~:text=Precedência%20de%20operadores&text=Operadores%20de%20multiplicação%2C%20divisão%20e,subtração%20são%20aplicadas%20em%20seguida

## 16 - Condicionais
Condicionais é uma coisa q vai validar a condição de algo. 

Exemplo:
Vou validar se determinada informação q uma pessoa colocou na minha aplicação corresponde a x valor q eu tenho numa regra e dependendo dessa regra eu libero um desconto ou não.
Estruturas condicionais:

if

if else

switch case

### Estrutura condicional if/else

O if/else é uma estrutura de condição em que uma expressão booleana é analisada. Quando a condição q estiver dentro do if for verdadeira, ela é executada. Já o else é utilizado p/definir o q é executado quando a condição analisada pelo if for falsa
Caso o if seja verdadeiro e, consequentemente executado, o else não é executado.

O if pode ser utilizado em conjunto com o else ou até mesmo sozinho, caso necessário.

Ainda é possível encadear múltiplas estruturas if/else caso necessário.

```
public static void main(String[] args) {
        int resposta = 10;
        if (resposta == 10) { 
            System.out.println(“A resposta é exatamente 10!”);
        } else if (resposta > 10) {
            System.out.println(“A resposta é maior que 10!”);
        } else {
            System.out.println(“A resposta é menor que 10!”);
        }
    }
```
https://www.treinaweb.com.br/blog/estruturas-condicionais-e-estruturas-de-repeticao-em-java

### Estrutura condicional: Switch case. 

Uma alternativa ao if/else é o switch case, q é uma estrutura de controle de fluxo q permite executar diferentes ações com base no valor de uma expressão. É uma forma mais simplificada e legível de escrever vários blocos if/else encadeado:

```
int dia = 3;
String nomeDia;
switch (dia) {
   case 1:
      nomeDia = "domingo";
      break;
   case 2:
      nomeDia = "segunda-feira";
      break;
   case 3:
      nomeDia = "terça-feira";
      break;
   case 4:
      nomeDia = "quarta-feira";
      break;
   case 5:
      nomeDia = "quinta-feira";
      break;
   case 6:
      nomeDia = "sexta-feira";
      break;
   case 7:
      nomeDia = "sábado";
      break;
   default:
      nomeDia = "Dia inválido";
      break;
}

System.out.println("O dia " + dia + " é " + nomeDia);
```

## 17 - Estrutura de repetição:
As estruturas de repetição elas tratam como que a gente determina alguma regra que vai ser executada de determinado valor até determinado valor até determinado cenário 

Nós temos 3 estruturas de repetição dentro do Java (for, while e o do while):

for

Cria um laço de tal valor até determinado valor vc vai fazer x coisa:

```
//for
for (int i = 0; i<=100; i++){
   System.out.println("Exemplo repetição valor i valendo: " + i);
}
```

while

Imagine que tenho um jogo de adivinhação onde vc precisa digitar um número e a aplicação deve parar no momento que vc digitar o número “secreto” (”adivinhar o número secreto”). Enquanto vc não acertar o valor secreto precisa ficar solicitando para pessoa digitar.

```
//while
public class Main {
    public static void main(String args[]) {
     Scanner in  = new Scanner(System.in);
     var valorSecreto = 0;
     while (valorSecreto != 12345){
         System.out.println("adivinha o valor secreto");
         valorSecreto = in.nextInt();
         if (valorSecreto == 12345){
             System.out.println("voce acertou o valor parabéns");
         } else {
             System.out.println("não é esse o valor");
         }
        }
    }
```

do while 

é parecido com o while mas esse vai ser “faça determinada coisa enquanto tal coisa não for atingida”

```
// do while
public class Main {
    public static void main(String args[]) {
        int valor = 10;
        do {
            System.out.println(valor);
            valor++;
        } while (valor <= 50);
    }
```
