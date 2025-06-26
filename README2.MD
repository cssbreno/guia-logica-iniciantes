# 🧠 Lógica de Programação do Zero

> Um guia simples, visual e interativo para iniciantes em Java!

---

## 🧭 Navegação

- [🛠 O que você vai aprender](#-o-que-você-vai-aprender)
- [📈 Conceitos Básicos](#-conceitos-básicos)
- [💭 O que é um Algoritmo?](#-o-que-é-um-algoritmo)
- [💻 Ambiente de Desenvolvimento](#-ambiente-de-desenvolvimento)
- [🔄 Condicionais e Lógica](#-condicionais-e-lógica)
- [🧮 Operadores e Tipos](#-operadores-e-tipos)
- [🧪 Casting e Conversões](#-casting-e-conversões)
- [📥 Entrada e Saída de Dados](#-entrada-e-saída-de-dados)
- [🧠 Funções e Modularização](#-funções-e-modularização)
- [📦 Vetores e Matrizes](#-vetores-e-matrizes)
- [✨ Pratique!](#-pratique)
- [👨‍💻 Sobre mim](#-sobre-mim)

---

## 🛠 O que você vai aprender:

- Como pensar logicamente como um programador
- Conceitos fundamentais da lógica de programação em Java
- Como o código "fala" com o computador
- Construção de algoritmos e estruturas de controle
- Tipos de dados, variáveis, operadores e funções
- Vetores e matrizes (arrays)

---

<div align="center">
  <img src="https://media.giphy.com/media/26AHONQ79FdWZhAI0/giphy.gif" width="300" />
  <p><i>Vamos programar juntos?</i></p>
</div>

---

## 📈 Conceitos Básicos

### 🤔 O que é lógica de programação?

Lógica é o **jeito de pensar para resolver problemas**. Quando você escreve um código, está descrevendo **passo a passo** o que o computador deve fazer.

Imagine uma receita de bolo:

```pseudo
1. Pegue os ingredientes
2. Misture tudo
3. Coloque no forno
4. Espere assar
5. Sirva o bolo
```

É isso que um programa faz! Só que em vez de farinha e ovos, usamos variáveis, funções e condições.

### 💡 Um algoritmo é exatamente isso: **uma sequência ordenada de passos para resolver um problema.**

---

## 💻 Ambiente de Desenvolvimento

Para programar em Java, você precisa de:

- ☕ **Java JDK** (Java Development Kit)
- 💻 **IDE** como Eclipse, IntelliJ ou VSCode
- 👾 JVM (Java Virtual Machine) que executa os programas

### 🛠 Passo a passo para começar:

1. Baixe o JDK: [Download JDK 11](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html)
2. Instale o Eclipse: [Download Eclipse](https://www.eclipse.org/downloads/)
3. Crie seu primeiro projeto e sua primeira classe

Exemplo básico:

```java
public class HelloWorld {
  public static void main(String[] args) {
    System.out.println("Olá, mundo!");
  }
}
```

---

## 🔄 Condicionais e Lógica

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

### ⚖️ Condição Ternária

```java
String status = (idade >= 18) ? "Adulto" : "Menor";
```

### 🧠 Operadores Lógicos

```java
&&  // E (AND)
||  // OU (OR)
!   // NÃO (NOT)
```

Exemplo:
```java
if (idade > 18 && renda > 2000) {
  System.out.println("Aprovado!");
}
```

---

## 🧮 Operadores e Tipos

### 🧮 Operadores Aritméticos

| Operador | Significado     | Exemplo     | Resultado |
|----------|------------------|-------------|-----------|
| `+`      | Adição           | `2 + 3`     | `5`       |
| `-`      | Subtração        | `5 - 2`     | `3`       |
| `*`      | Multiplicação    | `4 * 2`     | `8`       |
| `/`      | Divisão          | `10 / 2`    | `5`       |
| `%`      | Resto da divisão | `14 % 3`    | `2`       |

**Lembre-se:** Se usar inteiros, o resultado da divisão será inteiro!

### 📊 Tipos de Dados

```java
int idade = 25;
float nota = 9.5f;
double salario = 2300.75;
char sexo = 'M';
boolean ativo = true;
String nome = "João";
```

---

## 🧪 Casting e Conversões

Quando você mistura tipos diferentes, pode ser necessário converter:

```java
int x = 5;
double y = (double) x / 2; // Casting explícito
```

Ou forçar o uso de double para evitar arredondamentos:

```java
double media = (nota1 + nota2) / 2.0;
```

---

## 📥 Entrada e Saída de Dados

### 📥 Scanner (entrada de dados):

```java
import java.util.Scanner;

Scanner sc = new Scanner(System.in);
int numero = sc.nextInt();
String texto = sc.next();
char letra = sc.next().charAt(0);
double salario = sc.nextDouble();
sc.close();
```

### 📤 Saída de dados:

```java
System.out.print();     // Sem quebra de linha
System.out.println();   // Com quebra de linha
System.out.printf();    // Com formatação
```

```java
System.out.printf("%.2f", salario); // 2 casas decimais
```

---

## 🧠 Funções e Modularização

Funções servem para **reutilizar código** e **organizar melhor seu programa**.

```java
public static int max(int x, int y, int z) {
  int maior = x;
  if (y > maior) maior = y;
  if (z > maior) maior = z;
  return maior;
}

System.out.println("Maior valor: " + max(10, 15, 5));
```

---

## 📦 Vetores e Matrizes

### 📦 Vetores (Arrays):

```java
int[] numeros = new int[5];
numeros[0] = 10;
```

```java
for (int i = 0; i < numeros.length; i++) {
  System.out.println(numeros[i]);
}
```

### 🔁 For-each:

```java
for (int num : numeros) {
  System.out.println(num);
}
```

### 🔲 Matrizes (Arrays 2D):

```java
int[][] matriz = new int[3][3];
matriz[0][1] = 7;
```

```java
for (int i = 0; i < 3; i++) {
  for (int j = 0; j < 3; j++) {
    System.out.print(matriz[i][j] + " ");
  }
  System.out.println();
}
```

---

## ✨ Pratique!

Sites com desafios para treinar lógica:

- [Hackerrank](https://www.hackerrank.com/domains/tutorials/10-days-of-javascript)
- [Codewars](https://www.codewars.com/)
- [Visualgo (Fluxogramas)](https://visualgo.net/en)

---

## 👨‍💻 Sobre mim

Quer aprender mais ou colaborar?

- 🐙 GitHub: [@SeuPerfil](https://github.com/SeuPerfil)
- 📸 Instagram: [@seuusuario](https://instagram.com/seuusuario)
- 📬 Email: [seuemail@exemplo.com](mailto:seuemail@exemplo.com)

<div align="center">
  <a href="https://github.com/SeuPerfil/logica-do-zero/stargazers">
    <img src="https://img.shields.io/github/stars/SeuPerfil/logica-do-zero?style=social" alt="GitHub stars"/>
  </a>
</div>

---

<div align="center">
  <img src="https://media.giphy.com/media/26tPoyDhjiJ2g7rEs/giphy.gif" width="200"/>
  <p><i>Código é poesia. Continue praticando!</i></p>
</div>
