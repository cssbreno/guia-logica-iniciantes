# 🧠 Lógica de Programação do Zero

> Um guia simples, visual e interativo para iniciantes!

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
- [👨‍💼 Sobre mim](#-sobre-mim)

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
  <p><i>Vamos programar juntos?</i></p>
</div>

---

## 📈 Conceitos Básicos

### 📊 Operadores Matemáticos

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

```java
int idade = 25;           // Inteiro
float nota = 9.5f;        // Decimal
char letra = 'A';         // Caractere
boolean ativo = true;     // Verdadeiro ou falso
String nome = "João";     // Texto
```

**Regras para variáveis:**
- Comece com letra ou `_`
- Nada de acento ou espaços
- Use `camelCase` para variáveis e `PascalCase` para classes

---

## 💭 O que é um Algoritmo?

> “Um passo a passo para resolver um problema.”

Exemplo:
```pseudo
1. Leia um número
2. Multiplique por 2
3. Mostre o resultado
```

<div align="center">
  <img src="https://media.giphy.com/media/QBd2kLB5qDmysEXre9/giphy.gif" width="300"/>
</div>

---

## 💻 Ambiente de Desenvolvimento

- **IDE**: Onde você programa (Ex: Eclipse, IntelliJ, VSCode)
- **Compilador**: Traduz seu código para bytecode
- **JVM**: Executa o bytecode em qualquer sistema

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

### 📉 Operadores Relacionais

```java
==  // igual
!=  // diferente
>   // maior
<   // menor
>=  // maior ou igual
<=  // menor ou igual
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

## 👨‍💼 Sobre mim

Me acompanhe ou entre em contato:

- 👩‍💻 GitHub: [@cssbreno](https://github.com/cssbreno)
- 📸 Instagram: [@css_breno](https://instagram.com/css_breno)
- 📨 Email: [cssbreno.dev@gmail.com](mailto:cssbreno.dev@gmail.com)

<div align="center">
  <a href="https://github.com/cssbreno/logica-do-zero/stargazers">
    <img src="https://img.shields.io/github/stars/cssbreno/logica-do-zero?style=social" alt="GitHub stars"/>
  </a>
</div>

---

<div align="center">
  <img src="https://media.giphy.com/media/26tPoyDhjiJ2g7rEs/giphy.gif" width="200"/>
  <p><i>Código é poesia. Continue praticando!</i></p>
</div>
