Vamos primeiro aprender a adicionar um estilo no nosso documento HTML, certo?

Começaremos pelo inline, que é dentro do próprio HTML, através da tag style, utilizada das seguintes formas:
<h1 style="color: blue;">Título
	<strong style="color: red;">alo</strong>
</h1>
Ou na head do HTML, assim:
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
	<style>
	h1 {
			color: blue;
			}
	
	strong {
			color: red;
			}
	</style>
</head>
Porém, a forma mais comum, é através da tag link, onde vamos linkar um documento CSS externo, um outro arquivo para nosso documento HTML, feito da seguinte forma:
<link rel="stylesheet" href="style.css">
Neste caso, o nosso documento CSS se chama style.css e sua relação com o HTML é de stylesheet.

A última forma é através do @import, que é na verdade uma regra do CSS, portanto, deve ser usada dentro do css, ao invés de dentro do HTML, como as duas primeiras formas, e seu uso é mostrado a seguir:
@import 'https://fonts.googleapis.com/css2?family=Roboto:wght@300&display=swap'
Não é recomendado seu uso, pois leva um pouco mais de tempo do que através da tag link, fazendo a página ficar menos responsiva, demorando mais para o carregamento da mesma.