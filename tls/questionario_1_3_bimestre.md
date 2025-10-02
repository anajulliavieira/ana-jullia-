---

### **Questionário de APIs e Requisições HTTP**

1.  O que é uma API (Interface de Programação de Aplicações)?

2.  Qual método HTTP é usado para solicitar dados de um recurso específico?

3.  Qual é a principal diferença entre os métodos HTTP `PUT` e `PATCH`?

4.  Em uma requisição HTTP, qual código de status indica que a requisição foi bem-sucedida?

5.  Como você faria uma requisição `GET` para uma API usando o cURL no terminal?

6.  Qual a principal desvantagem do XML em comparação com o JSON para APIs web modernas?

7.  Qual é o objetivo de um cabeçalho HTTP (`HTTP Header`)?

8.  Qual é a função de uma 'API Key' (Chave de API) na autenticação de uma requisição?

9.  Qual comando cURL é usado para fazer uma requisição `POST` com um corpo de requisição em formato JSON?

10. Para que serve o método HTTP `DELETE`?

11. Qual é a diferença entre um código de status HTTP `401 Unauthorized` e `403 Forbidden`?

12. Qual das seguintes tecnologias de autenticação é um padrão de autorização open-source para acesso a recursos protegidos?

13. Qual dos seguintes comandos cURL é usado para enviar um cabeçalho HTTP personalizado chamado 'Authorization'?

14. O que é o 'body' (corpo) de uma requisição HTTP `POST`?

15. O que um desenvolvedor deve fazer ao integrar uma API e receber um código de status HTTP na série `4xx`?

    respostas

---

### 1. 🔌 **O que é uma API?**
- Uma **API (Interface de Programação de Aplicações)** é um conjunto de regras que permite que diferentes sistemas se comuniquem entre si. Ela define como os dados devem ser solicitados e enviados entre cliente e servidor.

---

### 2. 📥 **Método HTTP para solicitar dados**
- **GET**: Usado para **recuperar dados** de um recurso específico sem alterar seu estado.

---

### 3. 🔄 **Diferença entre `PUT` e `PATCH`**
- `PUT`: Atualiza **todo** o recurso.
- `PATCH`: Atualiza **parte** do recurso.

---

### 4. ✅ **Código de status para sucesso**
- **200 OK**: Indica que a requisição foi bem-sucedida e o servidor retornou os dados esperados.

---

### 5. 🧑‍💻 **Requisição GET com cURL**
```bash
curl https://api.exemplo.com/recurso
```

---

### 6. 📉 **Desvantagem do XML em relação ao JSON**
- **Mais verboso**, difícil de ler e processar.
- JSON é **mais leve**, **mais rápido** e **mais compatível** com JavaScript.

---

### 7. 📬 **Objetivo do cabeçalho HTTP**
- Transmitir **metadados** sobre a requisição ou resposta, como tipo de conteúdo, autenticação, cache, entre outros.

---

### 8. 🔐 **Função da API Key**
- Identifica e autentica o **cliente** que está fazendo a requisição, garantindo **segurança** e controle de acesso à API.

---

### 9. 📤 **Requisição POST com JSON via cURL**
```bash
curl -X POST https://api.exemplo.com/recurso \
     -H "Content-Type: application/json" \
     -d '{"nome":"João","idade":30}'
```

---

### 10. 🗑️ **Função do método DELETE**
- Remove um recurso do servidor.

---

### 11. 🚫 **Diferença entre `401 Unauthorized` e `403 Forbidden`**
- `401 Unauthorized`: **Credenciais ausentes ou inválidas**.
- `403 Forbidden`: **Acesso negado**, mesmo com credenciais válidas.

---

### 12. 🔓 **Tecnologia de autenticação open-source**
- **OAuth 2.0**: Padrão aberto para autorização segura entre aplicações.

---

### 13. 🧾 **Comando cURL com cabeçalho Authorization**
```bash
curl -H "Authorization: Bearer SUA_API_KEY" https://api.exemplo.com/recurso
```

---

### 14. 📦 **O que é o 'body' de uma requisição POST**
- É o **conteúdo enviado** ao servidor, geralmente em formato JSON, contendo os dados que devem ser processados ou armazenados.

---

### 15. 🧠 **O que fazer ao receber código 4xx**
- **Analisar o erro** (ex: 400, 401, 403, 404).
- **Verificar a documentação da API**.
- **Corrigir parâmetros, autenticação ou rota**.
- **Testar novamente** com os ajustes.

--
    
