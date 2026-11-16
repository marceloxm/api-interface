# 🐙 GitHub API Interface (Front-end Componentizado em ReactJS)

## 📖 Sobre o Projeto

O **API Interface** é uma aplicação front-end desenvolvida em **ReactJS** como parte de um desafio prático da **[Digital Innovation One (DIO)](https://dio.me)**.

O objetivo principal do projeto é construir uma interface **totalmente componentizada, reutilizável e desacoplada** que consome a **API pública do GitHub** para pesquisar perfis de desenvolvedores e exibir de forma organizada suas informações públicas, estatísticas, repositórios criados e repositórios marcados com estrela (*starred*).

---

## ✨ Funcionalidades

- **Busca Dinâmica de Usuários:** Campo de pesquisa integrado que consulta diretamente a API REST do GitHub (`https://github.com{username}`) a partir do nome de usuário digitado.
- **Exibição de Perfil Completo:** Apresentação do avatar, nome completo, username com link direto para o GitHub, empresa, localização, blog/portfólio e contadores de **Seguidores**, **Seguindo**, **Gists** e **Repositórios Públicos**.
- **Navegação por Abas (Tabs):** Alternância rápida e sem recarregamento entre:
  - **Repositories:** Lista de repositórios públicos do usuário pesquisado;
  - **Starred:** Lista de repositórios favoritados (com estrela) pelo usuário.
- **Gerenciamento de Estado Global:** Compartilhamento limpo dos dados retornados pela API entre todos os componentes da árvore React utilizando **Context API** e **Hooks customizados**.

---

## 🛠️ Tecnologias Utilizadas

Com base na estrutura do repositório (`package.json`, `yarn.lock`, `src/`) e na arquitetura do projeto, são utilizadas as seguintes ferramentas:

- **[ReactJS](https://react.dev):** Biblioteca principal para criação da interface baseada em componentes funcionais.
- **React Hooks & Context API:** Gerenciamento de estado global da aplicação (`useState`, `useEffect`, `useContext`, `useCallback`).
- **[Axios](https://axios-http.com):** Cliente HTTP utilizado para realizar as requisições assíncronas na API REST do GitHub.
- **[Styled Components](https://styled-components.com):** Estilização isolada por componente (CSS-in-JS) e reset global de estilos.
- **[React Tabs](https://github.com):** Componente acessível para organização das abas de repositórios e favoritos.
- **[Yarn](https://yarnpkg.com) / npm:** Gerenciamento de dependências e scripts de execução.

---

## 📂 Estrutura de Diretórios

```text
api-interface/
├── image/                # Imagens e capturas de tela da aplicação para documentação
├── public/               # Arquivos estáticos e index.html
├── src/                  # Código-fonte React (components, providers, services, hooks)
├── package.json          # Dependências do projeto e scripts de execução
├── yarn.lock             # Árvore exata das dependências instaladas via Yarn
├── package-lock.json     # Árvore de dependências compatível com npm
└── README.md             # Documentação do projeto
```

---

## 🚀 Como Executar o Projeto na Sua Máquina

Como a aplicação consome diretamente a API pública do GitHub, **não é necessário configurar banco de dados ou rodar um servidor back-end local**.

### Pré-requisitos

Certifique-se de ter instalado em sua máquina:
- **[Node.js](https://nodejs.org)** (versão LTS recomendada)
- **[Yarn](https://yarnpkg.com)** (recomendado) ou **npm**
- **[Git](https://git-scm.com)**

### Passo a passo

1. **Clone o repositório:**
   ```bash
   git clone https://github.com
   ```

2. **Acesse a pasta do projeto:**
   ```bash
   cd api-interface
   ```

3. **Instale as dependências:**
   Utilizando o Yarn:
   ```bash
   yarn install
   ```
   *(Ou, caso prefira utilizar o npm: `npm install`)*

4. **Inicie o servidor de desenvolvimento:**
   Utilizando o Yarn:
   ```bash
   yarn start
   ```
   *(Ou com npm: `npm start`)*

5. **Acesse a aplicação no navegador:**
   O projeto abrirá automaticamente ou ficará disponível em `http://localhost:3000/`. Digite qualquer nome de usuário válido do GitHub (por exemplo, `marceloxm`) na barra de pesquisa para visualizar os dados.

---

## 📦 Gerando Build de Produção

Caso deseje compilar e otimizar os arquivos para publicação em produção, execute:

```bash
yarn build
```
*(Ou `npm run build`)*

Os arquivos finais serão gerados dentro da pasta `build/`.

---

## 🤝 Contribuição

Contribuições são sempre bem-vindas! Se você quiser melhorar este projeto:

1. Faça um **Fork** deste repositório.
2. Crie uma **Branch** para sua melhoria (`git checkout -b feature/NovaFuncionalidade`).
3. Faça o **Commit** das suas alterações (`git commit -m 'Adiciona nova funcionalidade'`).
4. Faça o **Push** para a branch (`git push origin feature/NovaFuncionalidade`).
5. Abra um **Pull Request**.

---

## 👨‍💻 Autor

Desenvolvido por **[marceloxm](https://github.com/marceloxm)** durante os estudos na **Digital Innovation One (DIO)**.



