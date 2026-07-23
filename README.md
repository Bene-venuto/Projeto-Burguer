# 🍔 DevClub - Burguer

Projeto simples criado para praticar os principais métodos de array do JavaScript (**forEach**, **map**, **reduce** e **filter**) manipulando o DOM de forma dinâmica.

![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow)
![HTML5](https://img.shields.io/badge/HTML-5-orange)
![CSS3](https://img.shields.io/badge/CSS-3-blue)

## 📋 Sobre o projeto

A aplicação exibe um cardápio de lanches e permite interagir com a lista através de quatro botões, cada um demonstrando o uso de um método de array diferente:

| Botão | Método JS | O que faz |
|---|---|---|
| **Mostrar tudo** | `forEach` | Renderiza todos os itens do cardápio |
| **Mapear** | `map` | Aplica 10% de desconto em todos os itens e renderiza a lista atualizada |
| **Somar tudo** | `reduce` | Soma o preço de todos os itens e exibe o valor total |
| **Filtrar** | `filter` | Exibe apenas os itens vegetarianos/veganos |

## 🗂️ Estrutura do projeto

```
├── index.html      # Estrutura da página
├── style.css        # Estilização (grid de cards, botões, tema dark)
├── product.js        # Array de dados (menuOptions) com os produtos
├── script.js         # Lógica de manipulação do DOM e eventos
└── img/              # Imagens dos produtos
```

## ⚙️ Funcionalidades

- **Listagem dinâmica**: os itens são renderizados via JavaScript a partir do array `menuOptions`, não são fixos no HTML.
- **Formatação de moeda**: os preços são formatados automaticamente para o padrão brasileiro (R$) usando `toLocaleString`.
- **Interatividade**: cada botão dispara uma função diferente, todas reaproveitando a mesma função `showAll` para renderizar a lista sempre que possível.

## 🚀 Como executar

1. Clone ou baixe este repositório.
2. Certifique-se de que a pasta `img/` contém as imagens referenciadas em `product.js`.
3. Abra o arquivo `index.html` diretamente no navegador (não é necessário servidor).

```bash
git clone <url-do-repositorio>
cd devclub-burguer
```

Depois é só abrir o `index.html` com dois cliques ou usando a extensão **Live Server** do VS Code.

## 🧠 Conceitos praticados

- Manipulação do DOM (`querySelector`, `innerHTML`, `addEventListener`)
- Template literals para geração de HTML dinâmico
- Métodos de array de alta ordem: `forEach`, `map`, `reduce`, `filter`
- Spread operator (`...product`) para clonar objetos sem mutar o array original
- Formatação de valores monetários com `Intl`/`toLocaleString`

## 📌 Possíveis melhorias futuras

- Adicionar um botão para "resetar" a listagem ao estado inicial
- Exibir mensagem quando o filtro não retornar nenhum item
- Adicionar testes automatizados para as funções de manipulação de dados
- Tornar o layout responsivo para telas menores (mobile)

## 👤 Autor

Projeto desenvolvido para fins de estudo, baseado em conteúdo da **DevClub**.
