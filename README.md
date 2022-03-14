# desafios_js
desafios simples de javascript

##### Deseja contribuir? Então siga o padrão dos arquivos.md abaixo,com seu nome do github,link do instagram(opcional)e linkedin,descrição do problema e a solução,além do link do codepen para acessar o código funcionando.

### Exemplo 👀

## Questão x Denise R
[LinkedIn](https://www.linkedin.com/in/denise-r-b3bab9205/)
[Instagram](https://www.instagram.com/development__studio/)

### Descrição: 
crie uma função que conta quantas vezes um botão foi clicado

### Solução
~~~HTML
<button id='bnt'>click</button>
<label id='label' for='bnt'></label>
~~~

~~~javascript
let bnt=document.getElementById('bnt');
bnt.addEventListener('click',action)
var d=0;
function action(){
 
  d+=1
  let label=document.getElementById('label').innerHTML=d;
  if(d==4|| d==6 || d==10){
    let label=document.getElementById('label').innerHTML=`chegou no ${d}`;

}
}
~~~

### Veja no [CodePen](https://codepen.io/Denise-rodrig/pen/wvpBmBo)

