# ❓ Projeto: Perguntas sobre HTML e JavaScript

Página interativa feita em **HTML, CSS e JavaScript puro** para a disciplina de **Programação de Scripts** na **Fatec Taquaritinga**. O usuário escolhe uma pergunta, vê a resposta e ela fica guardada numa **tabela de histórico**.

🌐 **Página:** [`index.html`](index.html)

---

## ✨ Funcionalidades

- 📋 **Lista de perguntas** num `select`:
  - Qual o propósito da linguagem HTML?
  - Qual o propósito da linguagem JavaScript?
  - O que são funções e como elas são definidas em JavaScript?
- 💬 **Mostrar Resposta:** adiciona a pergunta e a resposta como uma nova linha na tabela
- 🧹 **Limpar Histórico:** apaga todas as linhas da tabela
- ⚠️ **Aviso** (`alert`) se nenhuma pergunta for escolhida
- 🎨 Visual em **tema roxo**, com degradês, sombras e linhas zebradas

---

## 🧠 Conceitos aplicados

| Conceito | Onde aparece |
|---|---|
| **HTML semântico** | `header`, `main`, `section`, `footer` |
| **Eventos** | `onclick` nos botões |
| **Funções** | `mostrarResposta()` e `limpar()` |
| **Condicionais** | `if / else if / else` para escolher a resposta |
| **DOM** | `getElementById`, `insertRow`, `insertCell`, `textContent`, `innerHTML` |
| **CSS** | `linear-gradient`, `box-shadow`, `nth-child(even/odd)` |

```javascript
function mostrarResposta() {
  var select = document.getElementById("pergunta");
  // ...escolhe a resposta conforme o valor selecionado...
  var tabela = document.getElementById("historico").getElementsByTagName("tbody")[0];
  var novaLinha = tabela.insertRow();
  novaLinha.insertCell(0).textContent = texto;
  novaLinha.insertCell(1).textContent = resposta;
}
```

---

## 🚀 Como ver

- **Online:** ative o **GitHub Pages** (Settings → Pages → Branch `main` → Save).
- **No computador:** baixe o repositório e abra o `index.html` no navegador.

---

## 🎓 Informações acadêmicas

| | |
|---|---|
| **Instituição** | Fatec Taquaritinga |
| **Curso** | Análise e Desenvolvimento de Sistemas |
| **Disciplina** | Programação de Scripts |
| **Professor** | Giuliano Scombatti Pinto |

## 👥 Autores

- Juan Gabriel Pereira Augusto
- Daniel Freire Kim
