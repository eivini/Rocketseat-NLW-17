<div align="center">
  <h1>📋 Aplicativo de Metas no Terminal</h1>
  <p>Gerencie suas metas diretamente pelo terminal com interface interativa.</p>
</div>

<h2>🧩 Funcionalidades</h2>

<ul>
  <li>Cadastrar novas metas</li>
  <li>Listar metas com seleção múltipla</li>
  <li>Visualizar metas realizadas</li>
  <li>Visualizar metas em aberto</li>
  <li>Deletar metas individualmente</li>
  <li>Persistência de dados em arquivo <code>JSON</code></li>
  <li>Interface com menus interativos via terminal</li>
</ul>

<h2>📁 Estrutura do Projeto</h2>

<pre>
📦 raiz do projeto
├── metas.json             # Armazena as metas cadastradas
├── index.js               # Lógica principal da aplicação
├── package.json           # Dependências do projeto (como o inquirer)
└── README.md              # Documentação do projeto
</pre>

<h2>💡 Como Funciona</h2>

<p>
  A aplicação exibe um menu principal com opções como cadastrar, listar, visualizar metas realizadas/abertas e deletar. 
  Ao interagir, o terminal exibe menus interativos com o auxílio da biblioteca <code>@inquirer/prompts</code>. 
  As metas são salvas em um arquivo local <code>metas.json</code> de forma persistente.
</p>

<h2>🛠️ Tecnologias Utilizadas</h2>

<ul>
  <li><strong>JavaScript</strong> – Puro (sem frameworks)</li>
  <li><strong>Node.js</strong> – Execução via terminal</li>
  <li><strong>@inquirer/prompts</strong> – Menus e inputs interativos</li>
  <li><strong>fs/promises</strong> – Leitura e escrita de arquivos</li>
</ul>

<h2>⚙️ Requisitos</h2>

<ul>
  <li>Node.js instalado</li>
  <li>Terminal com suporte a interatividade (como o do VSCode)</li>
</ul>

<h2>🚀 Como Rodar</h2>

<ol>
  <li>Clone este repositório:
    <pre><code>git clone https://github.com/eivini/metas-terminal</code></pre>
  </li>
  <li>Instale as dependências:
    <pre><code>npm install</code></pre>
  </li>
  <li>Execute o programa:
    <pre><code>node index.js</code></pre>
  </li>
</ol>

<h2>📌 Créditos</h2>

<p>
  Projeto desenvolvido com base nos ensinamentos do curso <strong>Rocketseat NLW 17 - Pocket</strong>.<br>
  Feito com ❤️ por <a href="https://github.com/eivini">@eivini</a>
</p>