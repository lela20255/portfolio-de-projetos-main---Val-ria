<!DOCTYPE html>
<html lang="pt-br">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">
    <link rel="stylesheet" href="style.css">
    <title>Meu portfólio</title>
</head>

<body>
    <header class="container text-center">
        <img src="img/gambol.jpeg" alt="avatar da valeria" class="rounded-circle" width="150" height="150"
            srcset="">
        <p class="lead">Eu sou a Valéria_</p>
        <h1>Eu Aprendo Programação</h1>
        <p>Sou Estudante da escola Otto Weiszflog! 
            Já desenvolvi alguns projetos usando HTML e CSS.
             Veja os projetos que já desenvolvi!</p>
        <p>Minhas habilidades</p>
        <div>
            <p class="badge bg-secondary">HTML</p>
            <p class="badge bg-secondary">CSS</p>
        </div>
    </header>

<div class="acessibilidade">


    <div id="opcoesDeAcessibilidade" class="opcoes">
            <button id="aumentar-fonte">Aumentar Fonte</button>
            <button id="diminuir-fonte">Diminuir Fonte</button>
            <button id="alterna-contraste">Alternar Contraste</button>
            <button id="aumentar-largura">Aumentar Largura do Texto</button>
            <button id="diminuir-largura">Diminuir Largura do Texto</button>
            <button id="aumentar-espaco">Aumentar Espaçamento Letras</button>
            <button id="diminuir-espaco">Diminuir Espaçamento Letras</button>
            <button id="modo-escuro">Modo Escuro</button>
        </div>
    </div>
    <main class="container mt-5">
        <h2>Meus projetos</h2>
        <div class="row">
            <!-- Projeto 1 -->
            <div class="col-md-4">
                <div class="card">
                    <img src="img/careta.jpeg" class="card-img-top" alt="Imagem do projeto de biblioteca virtual">
                    <div class="card-body">
                        <h5 class="card-title">Lógica de programação: criando arte interativa com P5.js</h5>
                        <p class="card-text">Este projeto foi desenvolvido por mim no P5.js, ele foi criado com o objetivo
                            de modificar os códigos alterando as cores e movendo os olhos.
                        <button type="button" class="btn btn-link" data-bs-toggle="modal" data-bs-target="#modal1">Veja
                            o projeto</button>
                    </div>
                </div>
            </div>
            <!-- Projeto 2 -->
            <div class="col-md-4">
                <div class="card">
                    <img src="img/corrida.png" class="card-img-top" alt="Imagem do projeto da Joalheria">
                    <div class="card-body">
                        <h5 class="card-title">Listas, funções e repetição: criando um jogo de corrida (pt. 2)</h5>
                        <p class="card-text">Este é o início do meu projeto de uma corrida, criei ele com o objetivo de aprimorar 
                            as minhas tecnícas e aprendizagem!
                        </p>
                        <button type="button" class="btn btn-link" data-bs-toggle="modal" data-bs-target="#modal2">Veja
                            o projeto</button>
                    </div>
                </div>
            </div>

            
    </main>


    <footer class="container py-5">
        <h2>Entre em contato</h2>
        <div>
            <i class="bi bi-github"></i>
            <a href="https://github.com/femascheti">GitHub</a>
        </div>
        <p class="my-5 text-center">© Copyright 2025. Produzido por Valéria Moreira.</p>
    </footer>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
</body>
@import url('https://fonts.googleapis.com/css2?family=Chakra+Petch:ital,wght@0,300;0,400;0,500;0,600;0,700;1,300;1,400;1,500;1,600;1,700&display=swap');

:root {
    --cor-principal: #6E859F;
    --cor-secundaria: #284260;
    --cor-destaque: #C92BFC;
}

body {
    font-family: 'Chakra Petch', sans-serif;
    color: var(--cor-principal);
}

h1, h2, h5 {
    color: var(--cor-secundaria);
    font-weight: 700;
}

.lead, .btn-link {
    color: var(--cor-destaque);
    font-weight: 700;
}

a, .btn-link:hover {
    color: var(--cor-principal)
}

a:hover{
    color: var(--cor-destaque);
}

/* Resetando margens e preenchimentos */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    font-size: 1rem;
    line-height: 1.6;
    background-color: #f4f4f4;
    color: #333;
    transition: all 0.3s ease;
}

/* Estilo dos botões */
button {
    padding: 10px 15px;
    margin: 5px;
    cursor: pointer;
    background-color: #007BFF;
    color: white;
    border: none;
    border-radius: 5px;
    font-size: 1rem;
    transition: background-color 0.3s, transform 0.3s;
}

button:hover {
    background-color: #0056b3;
    transform: scale(1.05);
}

button:focus {
    outline: none;
}

/* Estilos da seção de acessibilidade */
.acessibilidade {
    position: fixed;
    top: 20px;
    right: 20px;
    z-index: 1000;
}

#opcoesDeAcessibilidade {
    display: none;
    flex-direction: column;
}

.opcoes {
    display: flex;
    flex-direction: column;
}

#botaoDeAcessibilidade.rotacao-botao {
    transform: rotate(90deg);
}

#opcoesDeAcessibilidade.apresenta-lista {
    display: flex;
}

/* Estilos do conteúdo */
.conteudo {
    padding: 20px;
    max-width: 80%;
    margin: auto;
    background-color: white;
}

/* Modo Escuro */
.modo-escuro {
    background-color: #121212;
    color: #e0e0e0;
}

/* Alto Contraste */
.alto-contraste {
    background-color: #000;
    color: #fff;
}

/* Ajuste de Largura de Texto */
body {
    max-width: 100%;
    margin: 0 auto;
}

body[max-width="90%"] {
    max-width: 90%;
}

body[max-width="80%"] {
    max-width: 80%;
}

body[max-width="70%"] {
    max-width: 70%;
}

/* Ajuste de Espaçamento das Letras */
body {
    letter-spacing: 0px;
}

body[letter-spacing="0.5px"] {
    letter-spacing: 0.5px;
}

body[letter-spacing="1px"] {
    letter-spacing: 1px;
}

body[letter-spacing="1.5px"] {
    letter-spacing: 1.5px;
}


</html>

