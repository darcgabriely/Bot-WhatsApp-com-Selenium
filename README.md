
# 📱 Bot WhatsApp com Selenium

Este projeto é um **bot automatizado para o WhatsApp Web** que utiliza **Selenium** para interagir com a interface do navegador e responder mensagens automaticamente com base nas informações fornecidas por uma API local.

## 🚀 Funcionalidades

- Acessa o WhatsApp Web com Selenium
- Detecta a última mensagem recebida em uma conversa
- Captura o número de telefone do contato
- Envia a mensagem e o número via `requests` para uma API (PHP)
- Envia a resposta da API automaticamente no chat

## 🛠️ Tecnologias utilizadas

- [Python](https://www.python.org/)
- [Selenium](https://www.selenium.dev/)
- [Requests](https://docs.python-requests.org/)
- WebDriver do Google Chrome

## ⚙️ Como executar o projeto

### 1. Instale as dependências

```bash
pip install selenium requests
```

### 2. Baixe o ChromeDriver

- Acesse: https://sites.google.com/a/chromium.org/chromedriver/downloads
- Baixe a versão compatível com o seu Chrome
- Coloque o `chromedriver` no mesmo diretório do script (ou adicione ao PATH)

### 3. Execute o bot

```bash
python bot.py
```

## 📁 Estrutura esperada

```plaintext
📦bot-whatsapp-selenium
 ┣ 📜bot.py
 ┣ 📜README.md
 ┗ 📷Captura de tela 2025-08-08 112117.png
```

## 🧠 Lógica do bot

1. Acessa https://web.whatsapp.com/
2. Aguarda o usuário escanear o QR Code
3. Abre uma conversa ativa
4. Lê a última mensagem recebida
5. Coleta o número do contato
6. Envia os dados para uma API PHP local (localhost)
7. Recebe e envia a resposta no chat

## 📄 Licença

Este projeto está sob a licença MIT.
