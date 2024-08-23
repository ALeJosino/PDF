# PDF
Estágio

# Introdução á Programação
**Aula 07**
## Funçôes
***

#### Agenda
* Funções
* Passagem de parâmetros
* Funções Com Retorno
* Modularização de Programas
***

# Funções

#### Funções
Funções em programação são blocos de código que realizam uma
determinada tarefa e podem ser chamados em qualquer ponto do programa
para executar a tarefa novamente. 

As funções ajudam a modularizar o código e torná-lo mais fácil de ler,
entender e manter.


Elas podem receber parâmetros como entrada, realizar alguma operação e
retornar um valor de saída.


As funções também podem ser aninhadas, onde uma função chama outra.
***

#### Exemplo de Função
```python
    def imprimeOi():
        print("Oi. Tudo bem?")
    imprimeOi()
```
Nesse exemplo, foi definida a função **imprimeOi** que exibe uma mensagem de texto na tela. 

Mas a mensagem só será impressa quando a função for chamada (invocada) em algum local do programa.
***

# Passagem de Parâmetros

#### Passagem de Parâmentros
Funções com passagem de parâmetros são funções que recebem valores como entrada para serem processados.

Os parâmetros são valores que a função espera receber como entrada para executar uma ação específica.

Essa abordagem é útil porque permite reutilizar código e torna o programa mais modular e fácil de manter.
***

#### Passagem de Parâmentros
A passagem de parâmetros pode ser realizada de diferentes maneiras: por valor, por referência e por nome.

Na passagem por valor, é criada uma cópia do valor do parâmetro original e a cópia é usada na função.

Já na passagem por referência, é passado um ponteiro para a variável original, permitindo que a função modifique diretamente o valor.

Na passagem por nome, os parâmetros são passados pelo nome em vez da posição, permitindo que os argumentos sejam passados em qualquer ordem.
***

#### Exemplo de Passagem de Parâmetros
```python
def calcular_media(n1, n2, n3):
    media = (n1 + n2 + n3) / 3
    print(media)
# Chamada da função passando os valores 8, 7 e 9 como parâmetros
calcular_media(8,7,9)
```
***

### Exemplo de Passagem de Parâmetros
No exemplo, a função **calcular_media** recebe três parâmetros (n1, n2 e n3) e calcula a média aritmética dos valores.

Ao chamar a função com os valores **8**, **7** e **9**, a função é executada e o resultado **8** é impresso na tela usando a função **print()**.
***

## Exercício
Escreva uma função que receba dois números e imprima a soma entres eles.
***

## Exercício
Escreva uma função que receba
dois números e informe qual o
maior entre eles.
***

# Funções Com Retorno

#### Funções Com Retorno
Funções com Retorno são funções que podem retornar um valor ou objeto calculado internamente para o código que a chamou.

O retorno é especificado pela instrução **return**.
***

#### Funções Com Retorno
Quando uma função é chamada em um programa, ela é executada, e o valor retornado pode ser armazenado em uma variável ou usado diretamente em uma expressão.

O uso de funções com retorno é útil para encapsular a lógica de um cálculo ou processamento em um módulo separado, permitindo que esse código possa ser reutilizado em diferentes partes do programa.
***

#### Exemplos de Funções Com Retorno
```python
def calcular_media(numeros):

# Calcula a média aritmética de uma lista de números.

    total = sum(numeros)
    media = total / len(numeros)
    return media
numeros = [4, 5, 6, 7, 8]
media = calcular_media(numeros)
print("A média dos números é:", media)
```
***

#### Exemplos de Funções Com Retorno
Neste exemplo, a função **calcular_media** recebe uma lista de números como parâmetro, calcula a média aritmética e retorna o valor da média para o programa principal.

São usadas as funções nativas do Python: **sum** (para calcular a soma de valores de uma lista) e **len** (que retorna a quantidade de itens de uma lista).

O valor retornado é armazenado na variável **media** e exibido na tela usando a função **print**.
***

## Exercício
Escreva uma função que receba uma lista de números e retorne a média aritmética de seus valores.
***

## Exercício
Escreva uma função que receba dois parâmetros e retorne se eles são iguais.
***

## Exercício
Escreva uma função que retorne uma “senha forte”.
***

# Modularização de Programas

#### Modularização de Programas
A modularização de programas é um processo de dividir um programa grande em módulos menores e mais gerenciáveis, com o objetivo de facilitar a manutenção e o desenvolvimento do código.

Esse processo permite que o programa seja dividido em partes que possam ser desenvolvidas, testadas e mantidas independentemente.
***

#### Modularização de Programas
ara realizar a modularização em Python, podemos criar arquivos com extensão .py que contenham funções ou classes relacionadas a uma determinada funcionalidade do programa.

Esses arquivos podem ser importados em outros arquivos Python para utilizar as funções ou classes definidas neles.

Dessa forma, é possível criar uma estrutura modularizada do programa, tornando-o mais organizado e fácil de entender e manter.
***

#### Exemplo de Modularização
Suponha que temos um programa que realiza cálculos matemáticos e queremos modularizá-lo. Podemos criar um arquivo chamado **calculadora.py** com as seguintes funções:
```python
def soma(a, b):
    return a + b
def subtracao(a, b):
    return a - b
def multiplicacao(a, b):
    return a * b
def divisao(a, b):
    if b == 0:
        return "Erro: divisão por zero!"
else:
    return a / b
```
***

#### Exemplo de Modularização
E em outro arquivo Python, podemos importar essas funções e utilizá-las:
```python
import calculadora

resultado = calculadora.soma(2, 3)
print(resultado) # Output: 5
 
resultado = calculadora.divisao(10, 2)
print(resultado) # Output: 5.0
```
***

## Exercício
Escreva um gerador de surpresinhas.

A surpresinha é um jogo aleatório com seis ou mais números para apostar na loteria.
***

# Avaliação

## Encerramento 
* Revisão
* Exercício Complementar
* Próxima Aula
