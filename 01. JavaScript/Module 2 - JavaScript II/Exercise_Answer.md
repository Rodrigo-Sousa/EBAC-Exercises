# Lista de Exercícios - Respostas

Exercícios:

## 1. Resolva as operações:
---
● 10 + 15 = **25 (number)**

● “10” + 2 = **102 (string)**

● “10” * 2 = **20 (number)**

● “10” / 3 = **3.3333333333333335 (float)**

● “10” % 3 = **1 (number)**

● 10 + true = **11 (number)**

● 10 == ”10” = **true (boolean)**

● 10 === “10” = **false (boolean)**

● 10 < 11 = **true (boolean)**

● 10 > 12 = **false (boolean)**

● 10 <= 10.1 = **true (boolean)**

● 10 > 9.99 = **true (boolean)**

● 10 != “dez” = **true (boolean)**

● 10 + true = **11 (number)**

● “dez” + true = **deztrue (string)**

● 10 + false = **10 (number)**

● 10 * false = **0 (number)**

● true + true = **2 (number)**

● 10++ = **11 (number) _Increment_**

● 10-- = **9 (number) _Decrement_**

● 1 & 1 = **1 (number)**

● 1 & 0 = **0 (number)**

● 0 & 0 = **0 (number)**

● 1 & 0 = **0 (number)**

● 0 / 1 = **0 (number)**

● 5 + 5 == 10 = **true (boolean)**

● “5” + ”5” == 10 = **false (boolean)**

● “5” * 2 > 9 = **true (boolean)**

● (10 + 10) * 2 = **40 (number)**

● 10 + 10 * 2 = **30 (number)**

## 2. Responda as perguntas de acordo com as variáveis.

var branco = 'preto';

var preto = 'cinza';

var cinza = 'branco';

var carro = 'preto';

var valor = 30000;

var prestacao = 750;

---

a) branco == 'branco'

R: 
```javascript
false 

// Pois dentro da variável branco, o que está contido é a palavra 'preto';

```

b) branco == cinza
R: 
```javascript
false 

// Pois dentro da variável branco, o que está contido é a palavra 'preto';

```

c) carro === branco
R: 
```javascript
true 

// Pois a variável carro possui a palavra 'preto' e a variável branco também, sendo do mesmo tipo e valor em ambas as variáveis.
```

d) var cavalo = carro == 'preto' ? 'cinza' : 'marron';
R: 
```javascript
cinza

// A cor do cavalo fica como cinza: Na variável carro está com a cor 'preta', e na sentença acima, está informando que a variável cavalo, recebe a variável carro, que se possuir a cor preta, irá ficar com a cor cinza, que é o que ocorre, na expressão. 
```

e) Quantas prestações são necessárias para pagar o valor do carro com uma entrada
de 3.000? Demonstre a operação.
R: 
```javascript

// São 36 prestações, tendo em mente que o valor do carro é de R$ 30.000,00, e deu uma entrada de R$ 3.000,00, com parcelas no valor de R$ 750,00. 

var entrada = 3000;
var valorAPagar = valor - entrada;
var prestacoes = valorAPagar / prestacao

console.log(`São necessárias ${prestacoes} prestações, para pagar o valor do carro que é de R$ ${valor}, com entrada R$ ${entrada} e parcelas de valor R$ ${prestacao}`);


```

f) Somando as variáveis de cores é formada uma string de quantos caracteres?
R: 
```javascript
// São 16 caracteres 

var cores = branco + preto + cinza
cores
'pretocinzabranco'

cores.length
16
```
