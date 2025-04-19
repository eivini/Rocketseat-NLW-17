<div align="center">
  <h1>🚀 in.orbit - Web</h1>
  <p>Interface web para acompanhamento de metas semanais.</p>
</div>

<h2>🧩 Funcionalidades</h2>

<ul>
  <li>Cadastro de novas metas com frequência semanal</li>
  <li>Registro de completamentos com um clique</li>
  <li>Visualização do progresso semanal</li>
  <li>Dashboard interativo com atividades concluídas</li>
  <li>Design responsivo e acessível</li>
</ul>

<h2>📁 Estrutura do Projeto</h2>

<pre>
📦 web
├── public/                # Arquivos estáticos
├── src/
│   ├── assets/            # Imagens e ilustrações
│   │   ├── lets-start-illustration.svg
│   │   └── logo-in-orbit.svg
│   ├── components/        # Componentes UI
│   │   ├── create-goal.tsx        # Formulário de criação de metas
│   │   ├── empty-goals.tsx        # Tela inicial sem metas
│   │   ├── in-orbit-icon.tsx      # Componente do logo
│   │   ├── pending-goals.tsx      # Lista de metas pendentes
│   │   └── summary.tsx            # Dashboard de progresso
│   ├── http/              # Chamadas à API
│   │   ├── create-goal-completion.ts
│   │   ├── create-goal.ts
│   │   ├── get-pending-goals.ts
│   │   └── get-summary.ts
│   ├── app.tsx            # Componente principal
│   ├── main.tsx           # Ponto de entrada
│   └── index.css          # Estilos globais
├── .gitignore
├── biome.json             # Configuração do linter
├── index.html             # Template HTML
├── package.json           # Dependências
├── postcss.config.js      # Configuração do PostCSS
├── tailwind.config.js     # Configuração do Tailwind
├── tsconfig.json          # Configuração do TypeScript
└── vite.config.ts         # Configuração do Vite
</pre>

<h2>💡 Como Funciona</h2>

<p>
  A aplicação web consome a API de metas, permitindo que usuários visualizem e gerenciem
  suas atividades semanais de forma intuitiva. O progresso é exibido em tempo real
  com gráficos e listas interativas.
</p>

<h2>🛠️ Tecnologias Utilizadas</h2>

<ul>
  <li><strong>React</strong> - Biblioteca para construção de interfaces</li>
  <li><strong>TypeScript</strong> - Tipagem estática</li>
  <li><strong>Tailwind CSS</strong> - Estilização utilitária</li>
  <li><strong>Vite</strong> - Build tool e dev server</li>
  <li><strong>TanStack Query</strong> - Gerenciamento de estado da API</li>
  <li><strong>Zod</strong> - Validação de formulários</li>
</ul>

<h2>⚙️ Requisitos</h2>

<ul>
  <li>Node.js 18+</li>
  <li>API de metas rodando localmente</li>
  <li>Yarn ou NPM</li>
</ul>

<h2>🚀 Como Rodar</h2>

<ol>
  <li>Clone este repositório:
    <pre><code>git clone https://github.com/seu-usuario/in-orbit-web</code></pre>
  </li>
  <li>Instale as dependências:
    <pre><code>npm install</code></pre>
  </li>
  <li>Inicie o servidor de desenvolvimento:
    <pre><code>npm run dev</code></pre>
  </li>
  <li>Acesse no navegador:
    <pre><code>http://localhost:5173</code></pre>
  </li>
</ol>

<h2>📌 Créditos</h2>

<p>
  Projeto desenvolvido com base nos ensinamentos do curso <strong>Rocketseat NLW 17 - Pocket</strong>.<br>
  Feito com ❤️ por <a href="https://github.com/eivini">@eivini</a>
</p>