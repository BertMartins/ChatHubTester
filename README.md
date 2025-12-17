# ChatHub Tester 🚀

Ferramenta simples para testar **SignalR Hub (ChatHub)** direto no navegador.
link para testar: https://bertmartins.github.io/ChatHubTester/

## 🧠 Por que esse projeto existe?

Eu tive dificuldade em testar meu **Hub do SignalR pelo Postman**.

No Postman até dá pra bater em endpoint HTTP…  
mas **SignalR não é HTTP comum**, é WebSocket.  
Resultado: eu não conseguia saber:

- Se o Hub estava realmente **conectando**
- Se o endpoint estava **respondendo**
- Se o fluxo de **chat estava funcionando**
- Se a mensagem estava **chegando no método do Hub**

Basicamente:  
> “Tá conectado ou não tá? Tá batendo no endpoint ou não tá?”

Foi daí que nasceu esse projeto 😅

## 🎯 Objetivo

Criar uma forma **visual, simples e direta** de:

- Conectar em qualquer **SignalR Hub**
- Enviar mensagens como se fosse um chat real
- Ver se o backend está respondendo
- Confirmar se o endpoint está correto
- Testar autenticação via **Bearer Token (JWT)**

Sem Postman.  
Sem gambiarra.  
Sem achismo.

## 🛠️ O que essa ferramenta faz

- ✅ Conecta em um Hub SignalR informando a URL
- ✅ Usa **Bearer Token (JWT)** para autenticação
- ✅ Mostra status da conexão (conectando / conectado / erro)
- ✅ Envia mensagens para o método do Hub
- ✅ Recebe mensagens do servidor
- ✅ Simula um chat real
- ✅ Mostra logs em tempo real

Tudo isso direto no navegador, usando apenas HTML + JS.

## 🧪 Como usar

1. Abra o arquivo `index.html` no navegador  
2. Informe:
   - **URL do Hub** (ex: `https://localhost:5001/chathub`)
   - **Bearer Token (JWT)**
3. Clique em **Conectar**
4. Envie mensagens e veja se:
   - O Hub responde
   - O método está sendo chamado
   - O fluxo está funcionando

Se conectou e respondeu:  
👉 Seu endpoint tá vivo. Pode dormir em paz.

## 📦 Tecnologias usadas

- HTML5
- CSS
- JavaScript
- SignalR Client (`@microsoft/signalr`)
- WebSocket

## 🤝 Quando isso é útil?

- Testar Hub sem frontend pronto
- Debugar conexão SignalR
- Validar autenticação JWT
- Confirmar se o método do Hub está sendo chamado
- Evitar perder tempo tentando testar SignalR no Postman (spoiler: não rola direito)

## ⚠️ Observação sincera

Isso **não substitui** um frontend completo.  
Mas resolve exatamente o problema que o Postman **não resolve** quando o assunto é SignalR.

Simples. Direto. Funciona.
