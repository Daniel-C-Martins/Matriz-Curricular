<h1>📘 Matriz Curricular Interativa – Projeto PET-Informática</h1>
<br>
<h2>🎯 Objetivo</h2>
<p>
  O projeto busca aprimorar a forma de visualização das matrizes curriculares dos cursos de tecnologia da PUCRS. 
  A proposta é oferecer uma interface dinâmica e interativa, que facilite a compreensão dos pré-requisitos, 
  da progressão acadêmica e dos detalhes de cada disciplina, tornando as informações mais acessíveis e intuitivas 
  para estudantes e professores.
</p>
<br>
<h2>💡 Motivação</h2>
<p>
  A matriz curricular atualmente é disponibilizada em formato de imagem estática, com diversas setas conectando disciplinas 
  e seus pré-requisitos. Embora funcione como referência oficial, esse modelo pode se tornar de difícil leitura, 
  principalmente em cursos com grande quantidade de disciplinas e conexões, gerando confusão visual.
</p>
<p>
  Motivados por essa limitação, desenvolvemos uma nova visualização digital que busca <strong>complementar</strong> a atual, 
  explorando os mesmos dados de forma mais clara e interativa. Acreditamos que a tecnologia pode transformar a matriz curricular 
  em uma ferramenta de apoio real ao planejamento acadêmico, permitindo que os estudantes tenham uma visão mais prática de seus percursos dentro do curso.
</p>
<br>
<h2>🌐 O que é o projeto</h2>
<p>
  Este projeto consiste em uma aplicação web que disponibiliza matrizes curriculares de forma padronizada e interativa, 
  acessível por meio de uma lista de cursos. Entre as funcionalidades principais, destacam-se:
</p>

<ul>
  <li><strong>Interatividade na visualização:</strong> ao passar o mouse sobre uma disciplina, todas as outras sem relação direta ficam com menor opacidade, enquanto as conectadas ganham destaque visual com bordas e etiquetas.</li>
  <li><strong>Sistema de etiquetas:</strong> disciplinas recebem marcações como “REQ” (quando possuem requisitos) e “HAB” (quando habilitam outras), facilitando a leitura rápida das relações.</li>
  <li><strong>Detalhes das disciplinas:</strong> ao selecionar uma disciplina, o sistema exibe informações como pré-requisitos, carga horária e ementa, além de listar todas as disciplinas subsequentes, oferecendo uma visão clara da progressão acadêmica.</li>
  <li><strong>Design integrado:</strong> a interface foi inspirada no portal oficial da PUCRS, pensando em sua futura implementação como uma aba complementar dentro do site da universidade.</li>
</ul>

<p>
  Com isso, o projeto não apenas facilita a compreensão das matrizes curriculares, mas também transforma a experiência em algo mais dinâmico, 
  intuitivo e útil para o planejamento dos estudantes.
</p>
<br>
<h2> Imagem da aplicação </h2>
<br>
<h2> 🖥️ Front-end </h2>
<p> No desenvolvimento da interface, optamos por utilizar o React, principalmente pela sua simplicidade, flexibilidade e pelo bom funcionamento na construção de interfaces dinâmicas. A biblioteca nos permitiu estruturar componentes reutilizáveis, garantindo maior consistência e facilidade de manutenção no projeto.

Além disso, utilizamos TypeScript como linguagem principal, já que buscávamos os benefícios de um sistema de tipos estático. Essa decisão trouxe mais segurança no desenvolvimento, reduzindo erros comuns e oferecendo um melhor controle sobre os dados trafegados entre os componentes.

Para estilização, escolhemos o Sass em vez do CSS puro. O Sass proporciona recursos adicionais, como variáveis, aninhamento e mixins, que tornam o código de estilos mais organizado, modular e fácil de manter em projetos maiores. </p>
<br>
<h2>⚙️ Back-end </h2>
<p> Para o desenvolvimento da camada de back-end, utilizamos Java como linguagem principal. A escolha se deve à sua robustez, segurança e ampla utilização no mercado, além de ser a linguagem base ensinada nos cursos de tecnologia da PUCRS. Isso garantiu que todos os integrantes do grupo já possuíssem familiaridade e pudessem contribuir de forma mais eficiente no projeto.

O framework escolhido foi o Spring Boot, que nos ofereceu recursos modernos para criação de APIs de forma ágil, escalável e com boa integração ao ecossistema Java. A simplicidade de configuração do Spring Boot permitiu maior foco nas regras de negócio em vez de detalhes de infraestrutura.

Na organização do sistema, optamos por adotar a Clean Architecture como modelo de arquitetura de software. Essa abordagem, aliada à aplicação dos princípios SOLID, favoreceu a separação de responsabilidades, a independência entre camadas e a facilidade de manutenção e evolução do código ao longo do tempo.</p>
<br>
<h2>🏗️ Infraestrutura</h2>
<p>
  O sistema foi construído de forma totalmente <strong>dockerizada</strong>, garantindo padronização do ambiente de desenvolvimento 
  e facilidade na execução do projeto em diferentes máquinas.
</p>
<ul>
  <li>Utilizamos o <strong>MySQL</strong> como banco de dados principal, rodando em um container Docker dedicado.</li>
  <li>Um arquivo <code>docker-compose.yml</code> foi configurado para orquestrar todos os serviços necessários, incluindo back-end, front-end e banco de dados.</li>
  <li>Com isso, a inicialização do projeto é simplificada: basta executar um único comando para que todos os containers sejam criados e executados em conjunto.</li>
</ul>
<br>
<h2>🗄️ Banco de Dados</h2>
<p>
  O modelo do banco foi elaborado para organizar e relacionar as disciplinas, pré-requisitos e informações adicionais como carga horária e ementa.
</p>
<p align="center">
</p>
<p align="center"><em>Figura 2: Diagrama UML do banco de dados</em></p>
<br>
<h2>🚀 Como rodar o programa</h2>
<ol>
  <li>
    <p><strong>Clonar o repositório</strong></p>
    <pre><code>git clone https://github.com/usuario/repositorio.git
cd repositorio</code></pre>
  </li>
  <li>
    <p><strong>Subir os containers com Docker Compose</strong></p>
    <pre><code>docker-compose up --build</code></pre>
  </li>
  <li>
    <p><strong>Acessar a aplicação</strong></p>
    <ul>
      <li>Front-end: <code>http://localhost:3000</code></li>
      <li>Back-end (API): <code>http://localhost:8080</code></li>
      <li>Banco de Dados: disponível em <code>localhost:5432</code></li>
    </ul>
  </li>
</ol>


