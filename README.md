<div align="center">

# 🎬 MovieCity

### Landing page de streaming feita com React + Vite

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&duration=3500&pause=1000&color=BB9AF7&center=true&vCenter=true&width=520&lines=Componentes+com+React+19;CSS+puro%2C+sem+framework;Layout+100%25+responsivo" alt="Typing SVG" />

![React](https://img.shields.io/badge/React_19-1a1b26?style=for-the-badge&logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite_7-1a1b26?style=for-the-badge&logo=vite&logoColor=BB9AF7)
![JavaScript](https://img.shields.io/badge/JavaScript-1a1b26?style=for-the-badge&logo=javascript&logoColor=F7DF1E)
![CSS3](https://img.shields.io/badge/CSS3-1a1b26?style=for-the-badge&logo=css3&logoColor=7AA2F7)
![ESLint](https://img.shields.io/badge/ESLint-1a1b26?style=for-the-badge&logo=eslint&logoColor=8080F2)

<br />

<img src="docs/preview.png" alt="Prévia da landing page MovieCity" width="92%" />

</div>

---

## ✨ Sobre o projeto

A **MovieCity** é a landing page de um serviço de streaming fictício. Fiz esse projeto para praticar o que mais importa no front-end: **componentização**, **CSS de verdade** (sem Bootstrap, sem Tailwind) e **adaptação do layout para qualquer tela**.

A página tem duas áreas:

- 🧭 **Header:** logo, menu de navegação (Filmes, Categoria, Sobre, Contato) e botão de Login.
- 🎞️ **Main:** o texto "Seus Filmes" com o botão **Mais** e um grid de 6 pôsteres (Afterlife, Transformers, Mowgli, Shift, Round 6 e Harry Potter).

No celular, as colunas se empilham, o grid vira 2 colunas e o menu se transforma em um **hambúrguer animado**. 🍔

## 🛠️ Tecnologias

| Tecnologia | Uso no projeto |
|---|---|
| ⚛️ **React 19** | Componentes (`Home`, `Header`, `Main`) e estado do menu |
| ⚡ **Vite 7** | Servidor de desenvolvimento com HMR e build de produção |
| 🎨 **CSS puro** | Layout com Flexbox e Grid, animações e media queries |
| 🧹 **ESLint** | Padronização e análise do código |

## 🚀 Como rodar

Você precisa do **Node.js 20.19+** (ou 22.12+) instalado.

```bash
# 1. clone o repositório
git clone https://github.com/anaasrv/Landing-Page-MovieCity.git

# 2. entre na pasta
cd Landing-Page-MovieCity

# 3. instale as dependências
npm install

# 4. rode o projeto
npm run dev
```

Abra **http://localhost:5173** no navegador. 💜

| Comando | O que faz |
|---|---|
| `npm run dev` | Inicia o servidor de desenvolvimento |
| `npm run build` | Gera a versão de produção em `dist/` |
| `npm run preview` | Pré-visualiza o build |
| `npm run lint` | Roda o ESLint |

## 📁 Estrutura

```
src/
├── assets/            # pôsteres dos filmes
├── components/
│   ├── Header.jsx     # logo, navegação e menu hambúrguer
│   ├── Main.jsx       # texto de chamada + grid de cards
│   └── Home.jsx       # junta Header + Main
├── App.jsx            # renderiza <Home />
├── index.css          # estilos globais + responsividade
└── main.jsx           # ponto de entrada do React
```

## 📱 Responsividade

| Largura | Alvo | O que muda |
|---|---|---|
| até **1100px** | Tablets em paisagem | Espaçamentos e fontes menores |
| até **900px** | Tablets e celulares grandes | Colunas empilham e o menu hambúrguer aparece |
| até **600px** | Celulares | Grid de 2 colunas, cards mais baixos |
| até **380px** | Celulares pequenos | Ajustes finos de fonte e altura |

📏 **Altura dos cards:** `170px` no desktop, `140px` até 600px e `120px` até 380px (propriedade `height` da classe `.card` em `src/index.css`).

## 🧠 O que eu pratiquei

- Dividir a interface em **componentes** reutilizáveis
- Usar `useState` para abrir e fechar o menu no mobile
- Renderizar a lista de links com `.map()`
- Montar layouts com **Flexbox** e **CSS Grid** (`minmax(0, 1fr)`)
- Criar o ícone de hambúrguer **só com CSS**
- Escrever **media queries** para 4 tamanhos de tela
- Cuidar de **acessibilidade** básica (`aria-label` e `aria-expanded` no botão do menu)

## 💡 Próximos passos

- [ ] Trocar as `div` dos cards por `button` (acessibilidade e teclado)
- [ ] Mostrar título e nota de cada filme
- [ ] Buscar os filmes de uma API (ex.: TMDB)
- [ ] Carrossel horizontal no mobile
- [ ] `prefers-reduced-motion` para quem prefere menos animação

---

<div align="center">

## 👩‍💻 Feito por Ana Lara

Estudante de Desenvolvimento de Sistemas no **SENAI**, em São Paulo, a caminho de uma carreira em **desenvolvimento web full-stack**. 🚀

[![LinkedIn](https://img.shields.io/badge/LinkedIn-1a1b26?style=for-the-badge&logo=linkedin&logoColor=7AA2F7)](https://linkedin.com/in/ana-saraiva-31b637399)
[![Gmail](https://img.shields.io/badge/Gmail-1a1b26?style=for-the-badge&logo=gmail&logoColor=BB9AF7)](mailto:saraiva.analara@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-1a1b26?style=for-the-badge&logo=github&logoColor=white)](https://github.com/anaasrv)

<sub>Feito com 💜 e muito café</sub>

</div>
