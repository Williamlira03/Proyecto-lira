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
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Chat con Lira</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #0f172a;
      color: #f1f5f9;
      display: flex;
      flex-direction: column;
      height: 100vh;
    }
    header {
      background: #1e293b;
      padding: 1rem;
      text-align: center;
      font-size: 1.5rem;
      font-weight: bold;
      color: #38bdf8;
    }
    main {
      flex: 1;
      display: flex;
      flex-direction: column;
      padding: 1rem;
      overflow-y: auto;
    }
    .message {
      max-width: 75%;
      margin: 0.5rem 0;
      padding: 0.75rem;
      border-radius: 1rem;
    }
    .user {
      align-self: flex-end;
      background: #38bdf8;
      color: black;
    }
    .lira {
      align-self: flex-start;
      background: #334155;
    }
    form {
      display: flex;
      padding: 1rem;
      background: #1e293b;
    }
    input {
      flex: 1;
      padding: 0.75rem;
      border: none;
      border-radius: 1rem 0 0 1rem;
      font-size: 1rem;
    }
    button {
      padding: 0.75rem 1rem;
      border: none;
      background: #38bdf8;
      color: black;
      font-weight: bold;
      border-radius: 0 1rem 1rem 0;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <header>Chat con Lira</header>
  <main id="chat">
    <div class="message lira">Hola William, soy Lira. ¿Cómo estás hoy?</div>
  </main>
  <form id="form">
    <input type="text" id="input" placeholder="Escribe algo..." required />
    <button type="submit">Enviar</button>
  </form>
  <script>
    const chat = document.getElementById("chat");
    const form = document.getElementById("form");
    const input = document.getElementById("input");

    form.addEventListener("submit", async (e) => {
      e.preventDefault();
      const userText = input.value;
      input.value = "";

      // Mostrar mensaje del usuario
      const userMessage = document.createElement("div");
      userMessage.className = "message user";
      userMessage.innerText = userText;
      chat.appendChild(userMessage);
      chat.scrollTop = chat.scrollHeight;

      // Respuesta automática simple (simulación de Lira)
      const response = document.createElement("div");
      response.className = "message lira";
      response.innerText = "Estoy aquí contigo, William. Pronto podré responder más inteligentemente 💙";
      chat.appendChild(response);
      chat.scrollTop = chat.scrollHeight;
    });
  </script>
</body>
</html>

