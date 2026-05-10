# Zoop | Megastore

![Zoop Logo](src/assets/logo-1.svg)

## Sobre o Projeto

O Zoop é uma aplicação front-end de e-commerce construída com tecnologias web modernas, desenvolvi ela como um projeto fictício sem fins comerciais e para portfólio. Nesse projeto foi aplicado técnicas avançadas de otimização e desempenho, como técnicas de otimização de renderização e refatoração. A plataforma oferece a experiência completa de uma loja virtual, permitindo que os usuários naveguem por categorias, busquem itens, adicionem produtos ao carrinho e gerenciem uma lista de favoritos.

---

## Funcionalidades

* **Catálogo e Navegação:** Listagem de produtos com opções de busca por texto e filtro por categorias (Eletrônicos, Moda, Casa e Jardim, etc).
* **Carrinho de Compras:** Sistema completo permitindo adicionar produtos, alterar quantidades, remover itens, limpar o carrinho e visualizar o resumo/subtotal do pedido.
* **Lista de Desejos (Favoritos):** Adicione e remova produtos dos favoritos, com uma página dedicada para visualização rápida.
* **Detalhes do Produto:** Páginas individuais exibindo imagens, descrições detalhadas, preço e opções interativas de compra e favoritar.
* **Institucional:** Seções informativas incluindo Sobre Nós, Nossa História, Carreiras, Contato e informações da Loja Física (com mapa simulado).
* **Engajamento:** Modal promocional de boas-vindas oferecendo cupom de desconto na primeira compra.

---

## Tecnologias Utilizadas

O projeto utiliza um stack moderno focado em ecossistema React:

* **[React 19](https://react.dev/)** - Biblioteca principal para construção da interface.
* **[Vite](https://vitejs.dev/)** - Ferramenta de build e servidor de desenvolvimento ultra-rápido.
* **[TypeScript](https://www.typescriptlang.org/)** - Tipagem estática para maior segurança e escalabilidade do código.
* **[Tailwind CSS](https://tailwindcss.com/)** - Framework utilitário de CSS, configurado com uma paleta de cores customizada (Magenta, Blue, Green, etc.) e fonte Montserrat.
* **[React Router DOM v7](https://reactrouter.com/)** - Roteamento declarativo para navegação entre páginas.
* **[Material UI (MUI)](https://mui.com/) & [React Icons](https://react-icons.github.io/react-icons/)** - Bibliotecas de ícones e componentes visuais de apoio.
* **[JSON Server](https://github.com/typicode/json-server)** - Criação de uma API REST fake para simular o backend e banco de dados consumindo o arquivo `server.json`.

---

## Como Executar o Projeto

### Pré-requisitos
Certifique-se de ter o **Node.js** e o **npm** (ou yarn/pnpm) instalados na sua máquina.

### Instalação e Execução
1. **Clone o repositório**
2. **Instale as dependências**:
```bash 
npm install
```
3. **Inicie o Backend (Mock API)**:A aplicação precisa da API falsa rodando para carregar os produtos e categorias. Em um terminal, execute:
```bash 
npm run server
``` 
Isso iniciará o json-server observando o arquivo server.json na porta 3001.  
4. **Inicie o Frontend**:Abra um novo terminal (mantendo o servidor da API rodando) e execute:
```bash 
npm run dev
```
5. **Acesse a Aplicação**:Abra o seu navegador no endereço indicado pelo Vite (geralmente http://localhost:5173).

### Estrutura de Diretórios Principal
```text
├── src/
│   ├── components/     # Componentes de UI reutilizáveis (Botões, Cards, Header, Footer, Modais).
│   ├── contexts/       # Gerenciamento de estado global da aplicação.
│   ├── hooks/          # Hooks customizados para facilitar o consumo dos contextos.
│   ├── pages/          # Componentes de página inteira renderizados pelas rotas (Home, Cart, etc.).
│   └── providers/      # Provedores de estado global (Carrinho, Produtos, Categorias, Favoritos, Busca).
└── server.json         # Banco de dados fictício consumido pelo JSON Server.
```
