## Questão 1 Denise R
[LinkedIn](https://www.linkedin.com/in/denise-r-b3bab9205/)
[Instagram](https://www.instagram.com/development__studio/)

### Descrição: 
crie dois input do tipo numero para receber duas notas e assim poder calcular sua media.


### Solução
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

### Veja no [CodePen](https://codepen.io/Denise-rodrig/pen/MWrYvBw)

