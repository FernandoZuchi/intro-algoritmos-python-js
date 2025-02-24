# Introdução aos Algoritmos - Roteiro de Aula Prática - Algoritmos em JavaScript

## Introdução

### O que são Algoritmos?
Antes de iniciarmos a programação propriamente dita, é importante entendermos o conceito de algoritmos. Um algoritmo nada mais é do que uma sequência de passos bem definidos para resolver um problema. Em nosso dia a dia, seguimos diversos algoritmos sem perceber, como por exemplo:

- Uma receita de bolo (passo a passo para preparar um bolo).
- Um manual de montagem de um móvel.
- As instruções para atravessar a rua com segurança.

Na programação, os algoritmos são essenciais, pois definem a forma como os programas resolvem problemas. E hoje vamos explorar alguns algoritmos simples utilizando JavaScript!

Além disso, vamos estruturar nosso código utilizando **funções**, um conceito fundamental na programação. Funções nos permitem reutilizar código e tornar os programas mais organizados e eficientes.

---

## Exercícios Práticos
A seguir, resolveremos alguns exercícios comuns para praticar conceitos fundamentais de algoritmos e lógica de programação em JavaScript e Python.

### 1. Calcular a Média
**Enunciado:**
Crie uma função que recebe um array de números e retorna a média dos valores.

**JavaScript:**
```javascript
function calcularMedia(numeros) {
    let soma = 0;
    for (let i = 0; i < numeros.length; i++) {
        soma += numeros[i]; // Soma todos os elementos do array
    }
    return soma / numeros.length; // Divide pela quantidade de elementos
}
```

**Python:**
```python
def calcular_media(numeros):
    soma = 0
    for num in numeros:
        soma += num # Soma todos os elementos do array
    return soma / len(numeros) # Divide pela quantidade de elementos
```

---

### 2. Verificar se um Número é Par ou Ímpar
**Enunciado:**
Crie uma função que recebe um número e retorna se ele é "par" ou "ímpar".

**JavaScript:**
```javascript
function verificarParOuImpar(numero) {
    if (numero % 2 === 0) {
        return "Par"; // Se o resto da divisão por 2 for 0, é par
    } else {
        return "Ímpar"; // Caso contrário, é ímpar
    }
}
```

**Python:**
```python
def verificar_par_ou_impar(numero):
    if numero % 2 == 0:
        return "Par" # Se o resto da divisão por 2 for 0, é par
    else:
        return "Ímpar" # Caso contrário, é ímpar
```

---

### 3. Somar Apenas os Números Pares de um Array
**Enunciado:**
Crie uma função que recebe um array de números e retorna a soma apenas dos elementos pares.

**JavaScript:**
```javascript
function somarPares(numeros) {
    let soma = 0;
    for (let i = 0; i < numeros.length; i++) {
        if (numeros[i] % 2 === 0) {
            soma += numeros[i]; // Soma apenas se o número for par
        }
    }
    return soma;
}
```

**Python:**
```python
def somar_pares(numeros):
    soma = 0
    for num in numeros:
        if num % 2 == 0:
            soma += num # Soma apenas se o número for par
    return soma
```

---

### 4. Alunos Acima da Média
**Enunciado:**
Dado um array de notas, retorne quantos alunos tiveram nota acima da média.

**JavaScript:**
```javascript
function alunosAcimaDaMedia(notas) {
    let media = calcularMedia(notas);
    let contador = 0;
    for (let i = 0; i < notas.length; i++) {
        if (notas[i] > media) {
            contador++; // Conta quantos alunos estão acima da média
        }
    }
    return contador;
}
```

**Python:**
```python
def alunos_acima_da_media(notas):
    media = calcular_media(notas)
    contador = 0
    for nota in notas:
        if nota > media:
            contador += 1 # Conta quantos alunos estão acima da média
    return contador
```

---

### 5. Multiplicar um Vetor por um Escalar
**Enunciado:**
Crie uma função que recebe um array e um número escalar, e retorna um novo array com cada elemento multiplicado pelo escalar.

**JavaScript:**
```javascript
function multiplicarVetor(vetor, escalar) {
    let resultado = [];
    for (let i = 0; i < vetor.length; i++) {
        resultado[i] = vetor[i] * escalar; // Multiplica cada elemento pelo escalar
    }
    return resultado;
}
```

**Python:**
```python
def multiplicar_vetor(vetor, escalar):
    resultado = []
    for num in vetor:
        resultado.append(num * escalar) # Multiplica cada elemento pelo escalar
    return resultado
```

---

Esses exercícios ilustram conceitos fundamentais de algoritmos e programação, incluindo estruturas condicionais, laços de repetição e manipulação de listas. Ao compreender essas lógicas, você estará preparado para desafios mais avançados no futuro!

