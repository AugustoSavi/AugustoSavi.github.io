<h1 align="center">
    Maquina de Turing - Teoria da computaçāo
</h1>

## :rocket: [Video Explicativo](https://youtu.be/BZHhdkhuRRk)

## :rocket: [Acesso ao Demo da Aplicação](https://augustosavi.github.io)


## :rocket: Construido por
<div align="center">
  :computer: Jean1dev <br>
  :computer: AugustoSavi <br>
  :art: mbleffa
</div>

## :information_source:  # Referencias 
https://medium.com/@chad.palmer/a-complete-web-page-building-a-turing-machine-in-javascript-d6c32d3708c4?source=friends_link&sk=7569f7204799328c676614eb1b992830

http://vanilla-js.blogspot.com/2016/04/javascript-turing-machine.html

https://plato.stanford.edu/entries/turing-machine/#Aca

https://github.com/NicollasMatheus37/turing-machine

https://github.com/awmorp/jsturing

https://github.com/VittGam/JSTMSimulator

## :information_source:  Tecnologias Usadas
![](https://img.shields.io/github/issues/AugustoSavi/AugustoSavi.github.io.git)
* JavaScript
* html
* css

## :information_source: Executando localmente
To clone and run this application, you'll need [Git](https://git-scm.com),. From your command line:

```bash
# Clone this repository
$ git clone https://github.com/AugustoSavi/AugustoSavi.github.io.git

# Abra o arquivo index.html na raiz do projeto
```

## :information_source: # Exemplos
```
-------Incrementando +1 em binario-------
 fita: 1 0 1 1
 estado: s1 0
{
    "s1": {
        "0": ["s1", "0", "R"],
        "1": ["s1", "1", "R"],
        "B": ["s2", "B", "L"]
    },
    "s2": {
        "0": ["s3", "1", "L"],
        "1": ["s2", "0", "L"],
        "B": ["s3", "1", "L"]
    },
    "s3": {
        "0": ["s3", "0", "L"],
        "1": ["s3", "1", "L"],
        "B": ["sh", "B", "R"]
    }
}


# Exemplo

-------10101 + 11100 = 110001 (21 + 28 = 49):-------

fita: 1 0 1 0 1 B 1 1 1 0 0
estado: s1 10

{
    "s1": {
        "B": ["s9", "B", "L"],
        "0": ["s7", "B", "L"],
        "1": ["s2", "B", "L"]
    },
    "s2": {
        "B": ["s3", "B", "L"],
        "0": ["s2", "0", "L"],
        "1": ["s2", "1", "L"],
        "x": ["s2", "x", "L"],
        "y": ["s2", "y", "L"]
    },
    "s3": {
        "B": ["s5", "y", "R"],
        "0": ["s5", "y", "R"],
        "1": ["s4", "x", "L"],
        "x": ["s3", "x", "L"],
        "y": ["s3", "y", "L"]
    },
    "s4": {
        "B": ["s5", "1", "R"],
        "0": ["s5", "1", "R"],
        "1": ["s4", "0", "L"]
    },
    "s5": {
        "B": ["s6", "B", "R"],
        "0": ["s5", "0", "R"],
        "1": ["s5", "1", "R"],
        "x": ["s5", "x", "R"],
        "y": ["s5", "y", "R"]
    },
    "s6": {
        "B": ["s1", "B", "L"],
        "0": ["s6", "0", "R"],
        "1": ["s6", "1", "R"],
        "x": ["s6", "x", "R"],
        "y": ["s6", "y", "R"]
    },
    "s7": {
        "B": ["s8", "B", "L"],
        "0": ["s7", "0", "L"],
        "1": ["s7", "1", "L"],
        "x": ["s7", "x", "L"],
        "y": ["s7", "y", "L"]
    },
    "s8": {
        "B": ["s5", "x", "R"],
        "0": ["s5", "x", "R"],
        "1": ["s5", "y", "R"],
        "x": ["s8", "x", "L"],
        "y": ["s8", "y", "L"]
    },
    "s9": {
        "B": ["s10", "B", "R"],
        "0": ["s10", "0", "R"],
        "1": ["s10", "1", "R"],
        "x": ["s9", "0", "L"],
        "y": ["s9", "1", "L"]
    },
    "s10": {
        "B": ["sh", "B", "L"],
        "0": ["s10", "0", "R"],
        "1": ["s10", "1", "R"],
        "x": ["s10", "x", "R"],
        "y": ["s10", "y", "R"]
    }
}
´´´
