---

### **Questionário de Desenvolvimento Web**

1.  Qual método do DOM você usaria para selecionar o primeiro elemento que corresponde a um seletor CSS específico (por exemplo, uma classe ou um ID)?

2.  O que acontece se você tentar acessar uma variável declarada com `let` ou `const` antes de sua declaração em JavaScript?

3.  Qual das seguintes afirmações sobre JSON é verdadeira?

4.  Em JavaScript, qual é a principal diferença entre `==` e `===`?

5.  Qual é o propósito da `Promise` em JavaScript?

6.  Como a API `fetch` do JavaScript difere do `XMLHttpRequest` tradicional?

7.  Qual é a ordem correta de eventos para o carregamento de uma página web e seus recursos?

8.  Qual é o principal benefício de usar AJAX (Asynchronous JavaScript and XML)?

9.  Em JavaScript, o que é um 'closure' (fechamento)?

10. Qual é a forma correta de converter um objeto JavaScript em uma string JSON?

11. Qual das seguintes opções é uma desvantagem potencial de usar `document.getElementById()` em vez de `document.querySelector()`?

12. Qual método de requisição HTTP é mais apropriado para enviar novos dados para o servidor?

13. O que a palavra-chave `this` se refere dentro de uma função de seta (arrow function)?

14. Qual das seguintes afirmações sobre o `spread operator` (...) em JavaScript é verdadeira?

15. Em JavaScript, o que significa 'callback hell'?


respostas 

---

### 1. 🧭 **Seleção de Elemento no DOM**
- **Método:** `document.querySelector()`
- **Por quê:** Retorna o **primeiro** elemento que corresponde ao seletor CSS fornecido (classe, ID, tag etc.).

---

### 2. ⏳ **Acesso a Variáveis com `let` ou `const` Antes da Declaração**
- **Resultado:** Gera um **erro de referência** (`ReferenceError`) devido ao **temporal dead zone** — o período entre o início do escopo e a declaração da variável.

---

### 3. 📦 **Afirmação Verdadeira sobre JSON**
- **Verdadeiro:** JSON é um **formato de texto leve** usado para **troca de dados** entre cliente e servidor. Ele é baseado em uma **estrutura de chave-valor** e é **facilmente lido por humanos e máquinas**.

---

### 4. ⚖️ **Diferença entre `==` e `===`**
- `==`: Compara **valores** com **coerção de tipo** (ex: `"5" == 5` é `true`).
- `===`: Compara **valores e tipos** (ex: `"5" === 5` é `false`).

---

### 5. 🔗 **Propósito da `Promise`**
- **Função:** Representa uma **operação assíncrona** que pode ser **resolvida** ou **rejeitada** no futuro, permitindo melhor controle de fluxo assíncrono.

---

### 6. 🌐 **Diferença entre `fetch` e `XMLHttpRequest`**
- `fetch`:
  - Usa **Promises**
  - Tem uma **sintaxe mais limpa**
  - Suporta **async/await**
- `XMLHttpRequest`:
  - Mais **verboso**
  - Não usa Promises nativamente

---

### 7. 📅 **Ordem de Eventos de Carregamento**
1. `DOMContentLoaded`: HTML carregado e analisado.
2. `load`: Página e todos os recursos (imagens, CSS, etc.) carregados.
3. `beforeunload` / `unload`: Quando o usuário está saindo da página.

---

### 8. ⚡ **Benefício do AJAX**
- Permite **atualizar partes da página** sem recarregá-la completamente, melhorando a **experiência do usuário**.

---

### 9. 🔒 **O que é um Closure**
- Um **closure** é uma função que **lembra o escopo** onde foi criada, mesmo após esse escopo ter sido finalizado. Isso permite **acesso a variáveis externas** mesmo fora do contexto original.

---

### 10. 🔄 **Converter Objeto em JSON**
```javascript
JSON.stringify(objeto)
```

---

### 11. ⚠️ **Desvantagem de `getElementById()`**
- Só funciona com **IDs**, enquanto `querySelector()` aceita **qualquer seletor CSS**, tornando-o mais **flexível**.

---

### 12. 📤 **Método HTTP para Enviar Dados**
- **POST**: Usado para **enviar novos dados** ao servidor.

---

### 13. 🧠 **`this` em Arrow Function**
- Em funções de seta, `this` **não é redefinido** e herda o valor do **escopo léxico** (contexto onde foi criada).

---

### 14. 📚 **Afirmação Verdadeira sobre `spread operator`**
- Permite **expandir elementos** de arrays ou objetos em locais onde múltiplos elementos são esperados. Exemplo:
```javascript
const arr = [1, 2, 3];
const novoArr = [...arr, 4]; // [1, 2, 3, 4]
```

---

### 15. 🕳️ **O que é 'Callback Hell'**
- Situação em que há **múltiplos callbacks aninhados**, tornando o código **difícil de ler e manter**. Exemplo clássico:
```javascript
funcao1(() => {
  funcao2(() => {
    funcao3(() => {
      // e assim por diante...
    });
  });
});
```
