<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" type="text/css" href="formulario.css" media="screen"> 
    <title>Formulario</title>
</head>
<body>
   
 <div class="campo">
    <h1 id="titulo">Cadastro de DEVs</h1>
    <p id="subtitulo">Complete suas informações</p>
    <br>
 </div class="campo">

<form>
    <fieldset class="grupo">
        <div class="campo">
            <label for="Nome"><strong>Nome</strong></label>
            <input type="text" name="nome" id="nome" required>
        </div class="campo">

        <div class="campo">
            <label for="Sobrenome"><stromg>Sobrenome</stromg></label>
            <input type="text" name="Sobrenome" id="Sobrenome" required>
        </div class="campo">
        </fieldset class="grupo">

        <div class="campo">
            <label for="email"><strong>Email</strong></label>
            <input type="email" name="email" id="email" required>
        </div class="campo">

        <div class="campo">
           <strong><label>De qual lado da aplicação você desenvolve<strong></label>
            <label>
                <input type="radio" name="devweb" value="Front-End"checked>Front-End
                <input type="radio" name="devweb" value="Back-End">Back-End
                <input type="radio" name="devweb" value="Full-Stack">Full-Stack
            </label>
        </div class="campo">
        <br>
        <div class="campo">
           <label>Senioridade</label> 
           <select id="senioridade">
            <option selected disabled value="">Escolha</option>
            <option>Junior</option>
            <option>Pleno</option>
            <option>Sênior</option>
           </select>
        </div class="campo">

        <fieldset>
            <div id="check">
                <label>Selecione as tecnologias que utiliza</label><br><br>
                <input type="checkbox" id="tecnologia1" name="tecnologia1" value="HTML">
                <label>HTML</label>
                <input type="checkbox" id="tecnologia2" name="tecnologia2" value="CSS">
                <label>CSS</label>
                <input type="checkbox" id="tecnologia3" name="tecnologia3" value="Javascript">
                <label>Javascript</label>
                <input type="checkbox" id="tecnologia4" name="tecnologia4" value="PHP">
                <label>PHP</label>
                <input type="checkbox" id="tecnologia5" name="tecnologia5" value="C#">
                <label>C#</label>
                <input type="checkbox" id="tecnologia6" name="tecnologia6" value="Python">
                <label>Python</label>
                <input type="checkbox" id="tecnologia7" name="tecnologia7" value="Java">
                <label>Java</label>
        </fieldset>

        <div class="campo">
        <br>
        <label>Conte um pouco da sua experiência</label>
        <textarea row="6" style="width:26em" id="experiência" name="experiência"></textarea>
        </div class="campo">

        <button class="botão" type="submit">Concluido</button>

    </form>

</body>
</html>


*{
   margin:0;
   padding: 0; 
}

#titulo{
    font-family:sans-serif;
    color:#2e4dbab9;
    margin-left: 7%;
} 

#subtitulo{
    font-family:sans-serif;
    color:#aaa9ab;
    margin-left: 10%;
}

fieldset{
    border:0;
}

body{
    background-color: #380b61;
    font-family: sans-serif;
    font-size: 1em;
    color:#e7ddf0;
    margin-left: 40%;
    margin-top: 1%; 
    justify-content: center;
}

input,select, textearea, button {
border-radius: 5px;
}

.campo{
   margin-bottom: 1em;
}

.campo label{
margin-bottom: 1em;
color: #f5f0f9;
display: block;
}

fieldset.grupo .campo{
    float: left;
    margin-right: 1em;
}

.campo input [type="text"], .campo input [type="email"], .campo select, .campo textarea{
    padding:0.1em;
    border: 1px solid #dedce0;
    box-shadow: 2px, 2px, 2px rgba(226, 214, 214, 0.2);
    display: inline-block;
}

.campo select, option{
    padding-right: 1em;
}

.campo input:focus, ,campo select:focus, .campo  textarea :focus {
    background:#e8e5ec
}

.botão{
    font-size: 1em;
    background: #f7f4f4c3;
    border:0;
    margin-bottom:2em;
    color: #eaeaf1;
    padding:0.2em 0.6em;
    box-shadow:1px, 1px, 1px rgba(0,0,0,0.2);
    text-shadow: #efedf0;
    position: fixed;
    top: 50%;
    left: 25%;
    margin-right:-50%;
    transform: translate(-50%, -50%);
}

.botão :hover{
    background:#ccbbff;
    box-shadow: inset:2px, 2px, 2px rgba(0,0,0,0.2);
    text-shadow:none; 
}

.botão, select{
    cursor:pointer;
}

#check{
    display: inline-block;
}

.botão, submit{
    background-color: #ccbbff;
}
