### Variáveis
[wikipedia](https://pt.wikipedia.org/wiki/Vari%C3%A1vel_(programa%C3%A7%C3%A3o))
> Na programação, uma variável é um objeto (uma posição, frequentemente localizada na memória) capaz de reter e representar um valor ou expressão.

##### Exemplo:
```javascript
example = 'Exemplo!'
alert(example)
other_example = 'Outro '.concat(example)
alert(other_example)
```


***
### Tipos de Variáveis
Cada linguagem de programação possui seus tipos de variáveis, alguns são comuns entre elas, outros poucas possuem.

#### Texto / String
Um Texto escrito dentro de aspas simples: 'texto'; ou duplas: "texto".

```javascript
example = 'Exemplo!'
```

#### Inteiro / Integer
Números sem aspas e sem pontos.

```javascript
example = 1
```

#### Numérico / Number (Float)
Números com pontos representando as casas decimais.

```javascript
example = 1.23
```

#### Booleano / Boolean
true ou false escritos sem aspas.

```javascript
example = true
example = false
```

#### Vetor / Array
Contém múltiplos valores. São acessados pelo número da posição, começando do 0.

```javascript
example = ['Exemplo!', true]
alert(example[1])
```

#### Objeto / Object (Hashmap)
Contém múltiplos valores. São acessados pelo nome dado.

```javascript
example = {
    exemple1: 'Exemplo!',
    'exemple 2': 16
}
alert(example.example1)
alert(example['example 2'])
```

#### Nulo / Null
null escrito sem aspas. Equivale a nenhum tipo de valor.

```javascript
example = null
```


***
### Funções
[wikipedia](https://pt.wikipedia.org/wiki/Sub-rotina)
> no contexto da programação, uma sub-rotina (função, procedimento ou mesmo subprograma) consiste em uma porção de código que resolve um problema muito específico, parte de um problema maior (a aplicação final)

O 'alert' é uma função do javascript. Você pode definir suas próprias funções.

##### Exemplo:
```javascript
function soma(x, y) {
    return x + y
}

quinze = soma(10, 5)
alert(quinze)
```


***
### Eventos
Executa uma função quando alguma ação específica é feita.

##### Exemplo:
```html
<html>
    <head>
        <title>Exemplo Eventos</title>
    </head>
    <body>
        <button onclick="alert('Clicou!')">Nao Clique</button>
    </body>
</html>
```


***
### Exercício
Criar a função cadastrada no evento onclick do botão. Esta função deve acessar o valor do elemento de id "texto".
Dica: use a função document.getElementById para acessar o elemento do html.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Exercício</title>
</head>
<body>
<section>
    <header>
        <h1>Exercício</h1>
    </header>
    <form onsubmit="return false">
        <h3>Formulário:</h3>
        <fieldset>
            <label>Digite:</label>
            <input type="text" id="texto"/>
            <button onclick="alertTexto()">OK</button>
        </fieldset>
    </form>
    <footer>
        <br/>
        <hr/>
        Rodapé
        <br/>
        <a href="https://github.com/dutradda/devcourses">devcourses©</a>
    </footer>
</section>
<script type="text/javascript">

</script>
</body>
</html>
```