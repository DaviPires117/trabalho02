<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <title>Formulário</title>
    <style>
     
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 0;
        }

        .container {
            max-width: 600px;
            margin: 20px auto;
            padding: 20px;
            background-color: #fff;
            border-radius: 5px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
        }

        label {
            display: block;
            margin-bottom: 10px;
        }

        input[type="text"],
        textarea {
            width: 100%;
            padding: 10px;
            margin-bottom: 15px;
            border: 1px solid #ccc;
            border-radius: 3px;
        }

        input[type="radio"],
        input[type="checkbox"] {
            margin-right: 5px;
        }

        select {
            width: 100%;
            padding: 10px;
            margin-bottom: 15px;
            border: 1px solid #ccc;
            border-radius: 3px;
        }

        button {
            background-color: #007bff;
            color: #fff;
            border: none;
            padding: 10px 20px;
            cursor: pointer;
        }

        button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <div class="container">
        <h2>Formulário</h2>
        <form action="#" method="post">
            <label for="nome">Nome:</label>
            <input type="text" id="nome" name="nome" required>

            <label>Gênero:</label>
            <input type="radio" id="masculino" name="genero" value="masculino">
            <label for="masculino">Masculino</label>
            <input type="radio" id="feminino" name="genero" value="feminino">
            <label for="feminino">Feminino</label>

            <label>Estilos musicais preferidos:</label>
            <input type="checkbox" id="rock" name="estilos[]" value="rock">
            <label for="rock">Rock</label>
            <input type="checkbox" id="pop" name="estilos[]" value="pop">
            <label for="pop">Pop</label>
            <input type="checkbox" id="hiphop" name="estilos[]" value="hiphop">
            <label for="hiphop">Hip Hop</label>

            <label for="cor">Cor favorita:</label>
            <select id="cor" name="cor">
                <option value="vermelho">Vermelho</option>
                <option value="azul">Azul</option>
                <option value="verde">Verde</option>
                <option value="amarelo">Amarelo</option>
            </select>

            <label for="unidade-ios">Unidade IOS mais próxima:</label>
            <input type="text" id="unidade-ios" name="unidade-ios" list="unidades-ios">
            <datalist id="unidades-ios">
                <option value="Unidade 1">
                <option value="Unidade 2">
                <option value="Unidade 3">
                <option value="Unidade 4">
            </datalist>

            <label for="observacoes">Observações:</label>
            <textarea id="observacoes" name="observacoes" rows="4"></textarea>

            <button type="submit">Enviar</button>
        </form>
    </div>
</body>
</html>
