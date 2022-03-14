crie dois input do tipo numero para receber duas notas e assim poder calcula sua media.
Acesse [aqui](https://codepen.io/Denise-rodrig/pen/MWrYvBw) para ver funcionando.

### solução
~~~HTML
<input type=number placeholder='nota 1' id=nota1></input>
<input type=number placeholder='nota 2' id='nota2'></input>
<button id='acao'>calcular</button>
~~~

~~~javascript
const action = document.getElementById("acao");

action.addEventListener("click", function () {
  let notaa = document.getElementById("nota1").value;
  let nota = document.getElementById("nota2").value;
  
  let nota1 = Number(notaa);
  let nota2 = Number(nota);
  
  if (nota1 <= 0 || nota2 <= 0) {
    console.log("sem valores");
  }else {
    console.log(nota1);
    console.log(nota2);
    let media = (nota1 + nota2) / 2;
    console.log(media);
  }
});
~~~
