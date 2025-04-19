<div align="center">
  <h1>🎯 Goal Tracking API</h1>
  <p>API para gerenciamento de metas semanais com acompanhamento de progresso.</p>
</div>

<h2>🧩 Funcionalidades</h2>

<ul>
  <li>Cadastrar novas metas com frequência semanal</li>
  <li>Registrar completamentos de metas</li>
  <li>Visualizar metas pendentes na semana atual</li>
  <li>Obter resumo semanal de progresso</li>
  <li>Persistência de dados em PostgreSQL</li>
  <li>Validação de dados com Zod</li>
</ul>

<h2>📁 Estrutura do Projeto</h2>

<pre>
📦 Server
├── src/
│   ├── db/
│   │   ├── index.ts         # Configuração do Drizzle ORM
│   │   ├── schema.ts        # Modelos de banco de dados
│   │   └── seed.ts          # Dados iniciais para desenvolvimento
│   ├── functions/
│   │   ├── create-goals.ts               # Lógica de criação de metas
│   │   ├── create-goals-completions.ts   # Lógica de registro de completamentos
│   │   ├── get-week-pending-goals.ts     # Consulta de metas pendentes
│   │   └── get-week-summary.ts           # Geração de resumo semanal
│   ├── http/
│   │   └── routes/
│   │       ├── create-completions.ts     # Rota POST /completions
│   │       ├── create-goals.ts           # Rota POST /goals
│   │       ├── get-pending-goals.ts      # Rota GET /pending-goals
│   │       └── get-week-summary.ts       # Rota GET /summary
│   ├── server.ts            # Configuração do servidor Fastify
│   └── env.ts               # Validação de variáveis de ambiente
├── biome.json               # Configuração do linter/formatter
├── docker-compose.yml       # Configuração do PostgreSQL
├── drizzle.config.ts        # Configuração do Drizzle Migrations
└── tsconfig.json            # Configuração do TypeScript
</pre>

<h2>💡 Como Funciona</h2>

<p>
  A API permite criar metas semanais (como "Estudar 6x por semana") e registrar cada vez que a meta é cumprida.
  O sistema calcula automaticamente seu progresso semanal e mostra quais metas ainda precisam ser completadas.
  Tudo isso através de endpoints RESTful com validação de tipos.
</p>

<h2>🛠️ Tecnologias Utilizadas</h2>

<ul>
  <li><strong>Fastify</strong> – Servidor HTTP rápido e eficiente</li>
  <li><strong>TypeScript</strong> – Tipagem estática</li>
  <li><strong>Drizzle ORM</strong> – ORM typesafe para PostgreSQL</li>
  <li><strong>Zod</strong> – Validação de schemas</li>
  <li><strong>Day.js</strong> – Manipulação de datas</li>
</ul>

<h2>⚙️ Requisitos</h2>

<ul>
  <li>Node.js 18+</li>
  <li>PostgreSQL ou Docker</li>
  <li>Yarn ou NPM</li>
</ul>

<h2>🚀 Como Rodar</h2>

<ol>
  <li>Clone este repositório:
    <pre><code>git clone https://github.com/seu-usuario/goal-tracking-api</code></pre>
  </li>
  <li>Instale as dependências:
    <pre><code>npm install</code></pre>
  </li>
  <li>Suba o PostgreSQL com Docker:
    <pre><code>docker-compose up -d</code></pre>
  </li>
  <li>Execute as migrações:
    <pre><code>npm run migrate</code></pre>
  </li>
  <li>Inicie o servidor:
    <pre><code>npm run dev</code></pre>
  </li>
</ol>

<h2>📌 Créditos</h2>

<p>
  Projeto desenvolvido com base nos ensinamentos do curso <strong>Rocketseat NLW 17 - Pocket</strong>.<br>
  Feito com ❤️ por <a href="https://github.com/eivini">@eivini</a>
</p>