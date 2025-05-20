
# Projeto de Testes com Postman – Engenharia de Qualidade

Este repositório contém um projeto prático de testes automatizados utilizando a ferramenta **Postman**, desenvolvido para a disciplina de **Engenharia de Qualidade**.

---

## 📌 Descrição do Projeto

O objetivo do projeto é demonstrar, de forma prática, como utilizar o Postman para testar APIs REST, explorando diferentes métodos (GET, POST, PUT e DELETE) e validando respostas com scripts automatizados.

A API utilizada foi a **JSONPlaceholder**, uma API pública que simula um backend para testes e prototipação.

---

## 🛠️ Ferramenta Utilizada

- **Nome:** Postman  
- **Tipo:** Gratuita e open-source (versão desktop usada neste projeto)  
- **Link oficial:** [https://www.postman.com/](https://www.postman.com/)

---

## 🚀 Requisições Testadas

1. `GET /posts` – Retorna todos os posts.
2. `GET /posts/1` – Retorna um post específico.
3. `POST /posts` – Cria um novo post com dados simulados.
4. `PUT /posts/1` – Atualiza um post existente.
5. `DELETE /posts/1` – Remove um post.

---

## 🧪 Scripts de Teste Automatizados

Todos os endpoints possuem scripts de validação na aba **Tests**, como:

```javascript
pm.test("Status code é 200", function () {
    pm.response.to.have.status(200);
});
```

Para os métodos `POST` e `PUT`, também foi validado se o campo `title` está presente e correto.

---

## 📂 Estrutura do Repositório

```
/projeto-testes-postman
├── testes-postman.json         # Coleção exportada do Postman
├── prints/                     # Evidências visuais das execuções
│   ├── requisicao-get.png
│   ├── requisicao-post.png
│   ├── aba-tests.png
│   └── runner-resultados.png
├── relatorio.pdf               # Relatório técnico (formato ABNT)
```

---

## ▶️ Como executar os testes

1. Baixe o [Postman](https://www.postman.com/downloads/).
2. Importe o arquivo `testes-postman.json` no Postman.
3. Explore cada requisição individualmente.
4. Use o **Collection Runner** para executar todos os testes automaticamente.
5. Confira os resultados dos testes no painel inferior.

---

## 🎯 Conclusão

Este projeto demonstrou a eficiência do Postman para testar APIs de forma rápida, simples e com automatização. A ferramenta se mostrou de fácil uso e com ótima curva de aprendizado, sendo ideal para iniciantes e profissionais da área de QA e desenvolvimento.

---

## 📘 Créditos

Desenvolvido por **Joana Letícia**  
Trabalho acadêmico individual para a disciplina de **Engenharia de Qualidade**.
