# 🧠 Lógica de Programação - facilitando sua vida

> E aí, pessoal!  
>  
> Esse conteúdo foi criado com a ideia de ser mais leve e amigável para quem tá começando em Lógica de Programação — sem despejar termos técnicos de cara, mas também sem deixar trazer detalhes importantes.  
>  
> A verdade é que lógica é uma etapa pela qual todo dev precisa passar. E, infelizmente, também é uma das que mais assustam quem tá no começo, levando muita gente a desistir. Pensando nisso, criei esse repositório.  
>  
> **Antes de começar, queria deixar um conselho:**  
>  
> Não se prende à escolha da linguagem agora. Qualquer uma vai te ajudar a aprender. O mais importante neste momento é desenvolver seu raciocínio lógico.  
>  
> A forma como você pensa, estrutura e resolve problemas é o que vai definir a qualidade das suas soluções. A linguagem é só a ferramenta que traduz isso em código.  
>  
> Foca em aprender lógica — e o resto vem com o tempo. 💡

---

## 🗺 Navegação

- [🛠 O que você vai aprender](#-o-que-você-vai-aprender)
- [📈 Conceitos Básicos](#-conceitos-básicos)
- [💭 O que é um Algoritmo?](#-o-que-é-um-algoritmo)
- [💻 Ambiente de Desenvolvimento](#-ambiente-de-desenvolvimento)
- [🔄 Condicionais](#-condicionais)
- [📅 Entrada de Dados (Scanner)](#-entrada-de-dados-scanner)
- [🔢 Estrutura Sequencial](#-estrutura-sequencial)
- [🧲 Funções Matemáticas](#-funções-matemáticas)
- [🧵 Vetores](#-vetores-arrays)
- [🔢 Matrizes](#-matrizes-arrays-bidimensionais)
- [🧪 Funções (Métodos)](#-funções-métodos)
- [✨ Pratique!](#-pratique)
- [🔮 Desafios](#-desafios)
- [👨‍💼 Contatos](#-sobre-mim)

---

## 🛠 O que você vai aprender:

- Conceitos básicos da programação
- Tipos de dados e variáveis
- Estruturas condicionais (if, else, switch)
- Operadores lógicos e matemáticos
- Condições ternárias e casting
- Entrada e saída de dados com `Scanner`
- Estruturas sequenciais
- Funções matemáticas básicas
- Vetores e matrizes

---

<div align="center">
  <img src="https://media.giphy.com/media/26AHONQ79FdWZhAI0/giphy.gif" width="300"/>
  <p><i>Bora codar?</i></p>
</div>

---

## 📈 Conceitos Básicos


### O que é uma variável?

Variáveis são elementos no código que irão receber um nome dado por você para armazenar algum valor, que pode sofrer alterações com o decorrer do código.  
Em Java, por ser uma linguagem tipada, ela exige que você declare o tipo dos elementos.

**Constante:** semelhante à variável, também recebe um nome dado por você e armazena um valor, a diferença é que esse valor **não tende a mudar** com o decorrer do código, como a variável.

**Classes:** são como moldes que definem o comportamento e as características de um objeto.  
Você pode imaginar como um modelo para criar vários objetos com as mesmas propriedades e ações.

### Operadores Matemáticos

| Operador | Significado     | Exemplo     | Resultado |
|----------|------------------|-------------|-----------|
| `+`      | Adição           | `2 + 3`     | `5`       |
| `-`      | Subtração        | `5 - 2`     | `3`       |
| `*`      | Multiplicação    | `4 * 2`     | `8`       |
| `/`      | Divisão inteira  | `25 / 3`    | `8` se for `int`, `8.33` se for `double` |
| `%`      | Módulo (resto)   | `14 % 3`    | `2`       |

**Prioridade:**
1. `*`, `/`, `%`
2. `+`, `-`

### 👨‍🔬 Tipos de Dados


O tipo dos dados define o que e como ele vai armazenar.  
Por exemplo, o tipo `int` armazena números inteiros, então colocar `int idade = 'Breno'` não dará certo, pois meu nome é um conjunto de caracteres, não números inteiros. O mesmo vale para números com casas decimais.

`float` se resume a ser o tipo que armazena números com casas decimais.  
Além disso, mesmo que o número seja redondo e mesmo que você formate a saída, ele ainda vai trazer o 0 depois da vírgula, como por exemplo, `2.0`.

`char` armazena apenas um caractere individual, não aceitando conjuntos, que já valem como `String`.

`boolean` aceita valores que retornam verdadeiro ou falso (`true` ou `false`), como em `1 > 2 = false`.  
Vê que a saída foi **"false"**? Isso ocorre porque o resultado não é verdade.

`String`, caso tenha percebido, tem a letra maiúscula, sendo um tipo de **objeto** e não um tipo primitivo, como os demais citados anteriormente.  
Existe uma diferença importante nisso, inclusive o Java olha para diferença de maiúscula e minúscula, ok? `Int` (objeto) é uma coisa, `int` é outra (tipo primitivo).  
Tipos primitivos são imutáveis e não aceitam outro tipo de valor.

Em Programação Orientada a Objetos você vai ver isso melhor, fica tranquilo (a).


```java
### 🧮 int (números inteiros)
Armazena valores como 5, 10, 25...

### 🔢 float (números com vírgula)
Armazena valores com casas decimais, como 9.5f, 3.14f...

💡 Dica: o `f` no final é obrigatório em Java!

### 🔤 char (caractere único)
Guarda apenas **um** caractere, como 'A', 'b', '9'

### ✅ boolean
Retorna `true` ou `false`, geralmente com base em comparações

### 🧵 String
Armazena textos como `"Olá mundo"`, `"Breno"` etc.
```

**Regras para variáveis:**
- Comece com letra ou `_`
- Nada de acento ou espaços
- Use `camelCase` (primeira inicial minuscula e segunda, maiúscula) para variáveis e `PascalCase` (ambas iniciais maiúsculas) para classes

---

## 💭 O que é um Algoritmo?

> “Um passo a passo para resolver um problema.”

`Algoritmo` é uma sequencia de instruções que tem como objetivo resolver um problema. Não me estenderei muito,  
mas sempre que você encara um problema e precisa pensar em uma solução, isso é um algoritmo. A sequencia de passos  
que você dá para cozinhar uma receita são um algoritmo. Gostou?

Explora um pouco mais com o Livro abaixo, salva muito no começo. (Não to recebendo nada pra isso, ok? kkkkkk)

[Entendendo Algoritmos - Livro Ilustrado para Programadores Curiosos](https://www.amazon.com.br/Entendendo-Algoritmos-Ilustrado-Programadores-Curiosos/dp/8575225634)

Precisa de algo mais interativo? Vai no curso do Gustavo Guanabara, ele vai desenhar pra você sobre isso, e com direito  
a certificado, tá?

[Curso em Vídeo - Algoritmos](https://www.cursoemvideo.com/course/algoritmos/)

Exemplo:  
```pseudo
1. Leia um número
2. Multiplique por 2
3. Mostre o resultado
```
<div align="center"> <img src="https://media.giphy.com/media/QBd2kLB5qDmysEXre9/giphy.gif" width="300"/> </div>

---

## 💻 Ambiente de Desenvolvimento (IDE)

Nada mais é do que o ambiente que você coda. Existem IDEs que possuem mais recursos para determinadas linguagens,
o que te direciona para escolher a medida que se encaixar com suas necessidades.

- **IDE**: Onde você programa (Ex: Eclipse, IntelliJ, VSCode)
- **Compilador**: Traduz seu código para bytecode
- **JVM**: Executa o bytecode em qualquer sistema (Java)

Exemplo básico em Java:
```java
public class HelloWorld {
  public static void main(String[] args) {
    System.out.println("Olá, mundo!");
  }
}
```

---

## 🔄 Condicionais

💡 Condicionais são estruturas que permitem criar cenários baseados em comparações ou verificações.

Por exemplo: “Se eu for maior de 18 anos, posso ingerir bebidas alcoólicas.”
Isso é uma condição sendo aplicada.

Em programação, as condicionais servem exatamente pra isso: tomar decisões com base em valores.
Elas se dividem em:

- Operadores relacionais (comparam valores);

- Operadores lógicos (criam combinações de condições).



### 📉 Operadores Relacionais

São usados pra comparar 2 valores. Por exemplo:

X é igual a Y?

A é maior que B?

Essas comparações retornam um resultado booleano: true (verdadeiro) ou false (falso).

```java
==  // igual
!=  // diferente
>   // maior
<   // menor
>=  // maior ou igual
<=  // menor ou igual
```
Exemplo:

```
java
Copiar
Editar
int a = 10;
int b = 20;

System.out.println(a == b);  // false
System.out.println(a < b);   // true
```

### 🔄 Operadores Lógicos

```java
&&  // E (AND)
||  // OU (OR)
!   // NÃO (NOT)
```

---

### ✅ IF/ELSE

```java
if (idade >= 18) {
  System.out.println("Maior de idade");
} else {
  System.out.println("Menor de idade");
}
```

### 🌐 SWITCH

```java
switch (dia) {
  case 1: System.out.println("Domingo"); break;
  case 2: System.out.println("Segunda"); break;
  default: System.out.println("Dia inválido");
}
```

---

### ⚖️ Condição Ternária

```java
String status = (idade >= 18) ? "Adulto" : "Menor";
```

---

### ⚡ Casting (Conversão de tipos)

```java
int a = 5;
double resultado = (double) a / 2;
String texto = String.valueOf(123);
```

---

## 📥 Entrada de Dados (Scanner)

```java
import java.util.Scanner;

Scanner sc = new Scanner(System.in);
int idade = sc.nextInt();
String nome = sc.next();
double altura = sc.nextDouble();
char letra = sc.next().charAt(0);
sc.close();
```

💡 **Dica**: Sempre feche o Scanner com `sc.close()` para evitar vazamentos de memória!

---

## 🔢 Estrutura Sequencial

Fluxo que segue linha por linha, do início ao fim:

```java
int x = 10;
double y = 20.5;
System.out.println(x + y);
```

### Saída formatada

```java
System.out.printf("%.2f%n", 10.0 / 3);  // 3.33
```

### Locale (ponto como separador decimal):
```java
import java.util.Locale;
Scanner sc = new Scanner(System.in).useLocale(Locale.US);
```

---

## 🧲 Funções Matemáticas

```java
Math.sqrt(25);     // Raiz quadrada
Math.pow(2, 3);     // Potência (2³)
Math.abs(-10);      // Valor absoluto
```

---

## 🧵 Vetores (Arrays)

```java
String[] nomes = new String[3];
nomes[0] = "João";
```

### For-each
```java
for (String nome : nomes) {
  System.out.println(nome);
}
```

---

## 🔢 Matrizes (Arrays Bidimensionais)

```java
double[][] matriz = new double[2][3];
matriz[0][1] = 7.5;
```

---

## 🧪 Funções (Métodos)

```java
public static int max(int a, int b) {
  return (a > b) ? a : b;
}

public static void mostrar(String mensagem) {
  System.out.println(mensagem);
}
```

---

## ✨ Pratique!

- [Hackerrank](https://www.hackerrank.com/domains/tutorials/10-days-of-javascript)
- [Codewars](https://www.codewars.com/)
- [Visualgo (Fluxogramas)](https://visualgo.net/en)

---

## 🔮 Desafios

Coloque seus conhecimentos em prática com esses desafios simples:

### 1. Número maior

Peça ao usuário para digitar 3 números e imprima qual é o maior entre eles.

### 2. Média escolar

Peça 2 notas (double), calcule a média e mostre se o aluno foi aprovado (média ≥ 6).

### 3. Par ou Ímpar

Leia um número inteiro e informe se ele é par ou ímpar.

### 4. Calculadora básica

Peça dois números e uma operação (+, -, *, /) e mostre o resultado.

### 5. Contagem regressiva

Leia um número inteiro positivo e mostre uma contagem regressiva até 0.

---

## 👨‍💼 Sobre mim

Quer aprender mais ou colaborar?

- GitHub: [Meu Perfil](https://github.com/cssbreno)
- Instagram: @css_breno
- Email: cssbreno.dev@gmail.com

<div align="center">
  
</div>

---

<div align="center">
  <img src="https://media.giphy.com/media/26tPoyDhjiJ2g7rEs/giphy.gif" width="200"/>
  <p><i>Código é poesia. Continue praticando!</i></p>
</div>