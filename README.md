# Exercício 1075 – Resto 2 | Java

## 📌 Descrição

Este projeto resolve o exercício **1075 – Resto 2**, da plataforma [Beecrowd](https://judge.beecrowd.com/pt/problems/view/1075).

O programa recebe um número inteiro `N` e apresenta todos os números entre 1 e 10000 que possuem **resto igual a 2 quando divididos por N**.

## 🛠️ Tecnologias utilizadas

- Java
- Scanner para entrada de dados
- Estrutura de repetição `for`
- Estrutura condicional `if`
- Operador módulo `%`

## 💻 Código-fonte

```java
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);

        int i, n;

        n = scanner.nextInt();

        for (i = 1; i <= 10000; i++) {
            if (i % n == 2) {
                System.out.println(i);
            }
        }

    }
}
```

## 🧠 Lógica do programa

1. O programa lê um número inteiro `n`.
2. Utiliza um laço `for` para percorrer os números de 1 até 10000.
3. Para cada número, calcula o resto da divisão por `n` utilizando `%`.
4. A condição `i % n == 2` verifica se o resto é igual a 2.
5. Quando a condição é verdadeira, imprime o número.
6. O processo continua até o final do intervalo.

## 📥 Exemplo de entrada

```text
13
```

## 📤 Exemplo de saída (primeiras linhas)

```text
2
15
28
41
54
67
80
93
106
119
...
```

O programa continua exibindo todos os números que atendem à condição até 10000.

## 🔎 Explicação do exemplo

Considerando `N = 13`:

| Número | Operação | Resto |
|---|---|---|
| 2 | 2 % 13 | 2 |
| 15 | 15 % 13 | 2 |
| 28 | 28 % 13 | 2 |
| 41 | 41 % 13 | 2 |
| 54 | 54 % 13 | 2 |

Todos esses números satisfazem a condição estabelecida.

## 📚 Conceitos praticados

- Leitura de dados utilizando `Scanner`
- Estrutura de repetição `for`
- Estrutura condicional `if`
- Operador módulo `%`
- Operadores relacionais
- Percorrimento de intervalos numéricos
- Filtragem de valores por condições matemáticas

## 🎯 Objetivo

Praticar estruturas de repetição e operadores matemáticos em Java, identificando números que apresentam um resto específico em operações de divisão inteira.

---

**Plataforma:** Beecrowd  
**Problema:** 1075 – Resto 2  
**Linguagem:** Java
