## Questão 1 Denise Rodrig
[LinkedIn](https://www.linkedin.com/in/denise-r-b3bab9205/)
[Instagram](https://www.instagram.com/development__studio/)

### Descrição: 
crie um input tipo texto que recebe o nome do usuário e um botão enviar.Se o nome for enviado aparecerá um label em abaixo escrito "olá nome_do_usuario",se enviar input vazia aparecerá um label em vermelho escrito "escreva nome do usuário".O NOME DO USUÁRIO DEVE ESTAR EM MAIÚSCULA E VC PODE ADICIONAR MAIS DETALHES NO CÓDIGO.

### Solução
~~~HTML
<input type='text' placeholder='escreva seu nome' id='nome'></input>
<button id='enviar'>envie</button>

<div>
  <label id='label'></label>
  <label id='texto'></labe>
</div>
~~~
~~~css
#label {
  color: red;
  font-family: arial;
  font-size: 12px;
}
div {
  display: flex;
  flex-direction: column;
  margin-top: 10px;
}
~~~
~~~javascript
let bnt = document.getElementById("enviar");
bnt.addEventListener("click", resultado);

function resultado() {
  let nome = document.getElementById("nome").value.toUpperCase();

  if (nome === "") {
    let labeltexto = (document.getElementById("texto").innerHTML = "");

    let label = (document.getElementById("label").innerHTML =
      "escreva seu nome");
  } else {
    let label = (document.getElementById("label").innerHTML = "");

    let labeltexto = (document.getElementById(
      "texto"
    ).innerHTML = `OLÁ ${nome}!`);
  }
}

~~~

### Veja no [CodePen](https://codepen.io/Denise-rodrig/pen/RwxWZaG?editors=1111)
