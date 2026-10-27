# Atividade 01 — Props no React

## Objetivo
Entender o que são **props**, como o componente **pai** envia dados para o componente **filho** e como o filho usa esses dados.

## Como rodar
```bash
npm install
npm run dev
```
Abra o endereço que aparecer no terminal (normalmente http://localhost:5173).

## Como fazer
Procure no código os comentários **`✏️ TAREFA`** e faça na ordem.
Dica: no VS Code, aperte `Ctrl+Shift+F` e pesquise `TAREFA`.

| Parte | Arquivo(s) | O que você vai aprender |
|-------|------------|-------------------------|
| 1 | `src/components/Saudacao.jsx` + `src/App.jsx` | O que é uma prop (exemplo pronto) |
| 2 | `src/components/CartaoAluno.jsx` + `src/App.jsx` | Várias props, desestruturação, texto vs número |
| 3 | `src/components/Produto.jsx` + `src/App.jsx` | Prop booleana, valor padrão, renderização condicional |
| 4 | `src/components/Botao.jsx` + `src/App.jsx` | A prop `children` e funções como props |
| 5 | `src/App.jsx` | **Desafio:** criar componentes a partir de um array com `.map()` |

## Resumo rápido
```jsx
// PAI envia a prop
<CartaoAluno nome="Ana" idade={17} />

// FILHO recebe e usa
function CartaoAluno({ nome, idade }) {
  return <p>{nome} tem {idade} anos</p>
}
```

- Texto vai entre **aspas**: `nome="Ana"`
- Número, booleano, função, array, objeto vão entre **chaves**: `idade={17}`
- Props são **somente leitura**: o filho nunca altera uma prop.

## Arquivos que você NÃO precisa mexer
`main.jsx`, `index.css`, `index.html`, `vite.config.js`, `package.json`
