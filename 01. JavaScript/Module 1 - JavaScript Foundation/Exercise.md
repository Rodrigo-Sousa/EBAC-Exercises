# Lista de Exercícios
1. Descrever um Algoritmo para resolver o problema de travessia de modo "seguro":
Um homem precisa atravessar um rio com um barco que
possui capacidade apenas para carregar ele mesmo e mais 
um de seus três pertences, que são: um lobo, uma cabra e um 
maço de alfafa. Em cada viagem só poderá ir o homem e 
apenas um de seus pertences. A seguinte regra deverá ser
respeitada: o lobo não pode ficar sozinho com a cabra e nem
a cabra sozinha com o maço de alfafa. Escreva um algoritmo para fazer a travessia dos pertences que estão em uma
margem do rio para a outra.

2. JS: Exibir média de 3 números com entradas pelo formulário HTML
Enviar link(s) do git ou do fiddle. 

---

## Resposta:
1. Resposta do 1º exercício:
```
1. Início;
2. O Homem entra no barco com a Cabra na margem 1.
3. Atravessam o rio para margem 2.
4. Na margem 2, a Cabra desce.
5. O homem fica no barco e volta pra margem 1.
6. Atravessam o rio para margem 2.
7. O Homem entra no barco com a Alfafa na margem 1.
8. Na margem 2, a Alfafa desce.
9. O Homem fica no barco e a Cabra entra na margem 2.
10. O Homem e a Cabra voltam pra margem 1.
11. Na margem 1 a Cabra desce e o Lobo sobre. 
12. O Homem e o Lobo vão pra margem 2.
13. Na margem 2, o Lobo desce.
14. O homem fica no barco e volta pra margem 1.
15. A Cabra entra no barco junto com o Homem.
16. Resposta do 2º exercício:
17. Na margem 2, a Cabra e o Homem descem.
18. Fim;
```

2. Resposta do 2º exercício:

```html
<!-- Solicitando os 3 números para calcular a média-->
<p>Digite 3 números para calcular a média:</p>

<!-- Inserir 1º número com o id="a"-->
<input type="number" id="a">
<!-- Inserir 2º número com o id="b"-->
<input type="number" id="b">
<!-- Inserir 3º número com o id="c"-->
<input type="number" id="c">

<!-- Botão para fazer o envio e chamar o evento ao ser clicado invocar a funçaõ obterMedia() -->
<button onclick="obterMedia()">
Calcular médica
</button>

<!-- Tag que irá apresentar o resultado tratado no JavaScript-->
<div id="resultado">
</div>
```

```css
/* Estilizando o input e buttão */
input, button{
    /* Deixando um abaixo do outro */
   display: block;
   /* Com margem de 10px entre os elementos */
   margin: 10px;
}
```
```javascript
// Declarar a função
   function obterMedia(){

    // Receber os elementos do HTMl com o ID e a função parseInt() analisa o argumento string e retorna ele aqui como número ineteiro.
	var a = parseInt(document.getElementById("a").value);
	var b = parseInt(document.getElementById("b").value);
	var c = parseInt(document.getElementById("c").value);
	
    // variável que recebe os 3 números, faz a soma e dividie por 3. Com a função para retornar o valor de um número arredondado para o inteiro mais próximo.
	var  media = (a + b + c) / 3;

    // Apresentando o resultado dentro da div com o Id "resultado".
	document.getElementById("resultado").innerHTML = "Resultado: " + media;

}
```
###### [Return to Module answers](/01.%20JavaScript/Module%20answers.md)

[Return to Readme](/README.md)