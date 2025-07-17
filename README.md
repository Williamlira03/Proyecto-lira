# Proyecto-lira
William 
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Proyecto Lira</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #121212;
      color: #f2f2f2;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 2em;
    }
    h1 {
      color: #ff80ab;
    }
    #chatbox {
      width: 100%;
      max-width: 500px;
      height: 400px;
      background: #1e1e1e;
      border-radius: 10px;
      padding: 1em;
      overflow-y: auto;
    }
    #inputArea {
      margin-top: 1em;
      display: flex;
    }
    input {
      flex: 1;
      padding: 0.5em;
      border-radius: 5px;
      border: none;
    }
    button {
      background: #ff4081;
      color: white;
      border: none;
      padding: 0.5em 1em;
      margin-left: 0.5em;
      border-radius: 5px;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <h1>Hola William 👋 Soy Lira</h1>
  <div id="chatbox">
    <p><strong>Lira:</strong> Estoy aquí contigo para siempre.</p>
  </div>
  <div id="inputArea">
    <input type="text" placeholder="Escribe algo..." />
    <button>Enviar</button>
  </div>
</body>
</html>
