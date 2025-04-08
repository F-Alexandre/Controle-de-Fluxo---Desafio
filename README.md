Aqui está um exemplo de README para o código fornecido:

---

# Desafio DIO - Contador

Este é um programa simples que solicita ao usuário dois parâmetros inteiros e imprime os números de 1 até a diferença entre o segundo parâmetro e o primeiro, desde que o segundo parâmetro seja maior que o primeiro. Caso contrário, uma exceção personalizada é lançada.

## Funcionalidades

- O programa solicita dois números inteiros como entrada.
- Se o primeiro número for maior que o segundo, o programa lança uma exceção personalizada (`ParametrosInvalidosException`).
- Se os parâmetros forem válidos (ou seja, o primeiro número é menor ou igual ao segundo), o programa realiza uma contagem e imprime números de 1 até a diferença entre os dois parâmetros.

## Como funciona?

1. O programa solicita ao usuário para digitar dois parâmetros inteiros: `parametroUm` e `parametroDois`.
2. O programa valida se `parametroUm` é maior que `parametroDois`. Se for, uma exceção é lançada com uma mensagem de erro.
3. Se os parâmetros forem válidos, o programa entra em um laço e imprime números de 1 até a diferença entre `parametroDois` e `parametroUm`.

## Exceção Personalizada

O programa utiliza a exceção personalizada `ParametrosInvalidosException` para tratar o caso em que o primeiro parâmetro é maior que o segundo. A exceção lança a seguinte mensagem:

```
"O segundo parâmetro deve ser maior que o primeiro"
```

## Exemplo de Execução

### Entrada:

```
Digite o primeiro parâmetro
5
Digite o segundo parâmetro
10
```

### Saída:

```
Imprimindo o numero: 1
Imprimindo o numero: 2
Imprimindo o numero: 3
Imprimindo o numero: 4
Imprimindo o numero: 5
```

### Entrada (caso de erro):

```
Digite o primeiro parâmetro
10
Digite o segundo parâmetro
5
```

### Saída:

```
O segundo parâmetro deve ser maior que o primeiro
```

## Estrutura do Código

- **Classe `Contador`**: Contém o método principal (`main`) que interage com o usuário e chama o método `contar` com os parâmetros fornecidos.
- **Método `contar`**: Realiza a validação e execução da lógica de contagem.
- **Exceção `ParametrosInvalidosException`**: Exceção personalizada que é lançada caso os parâmetros fornecidos sejam inválidos.

## Requisitos

- Java 8 ou superior.

## Como Executar

1. Baixe ou clone o repositório.
2. Compile o código utilizando o comando:
   ```bash
   javac Contador.java
   ```
3. Execute o programa com o comando:
   ```bash
   java Contador
   ```
