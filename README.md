<div align="center">
<img src="https://raw.githubusercontent.com/FortAwesome/Font-Awesome/6.x/svgs/solid/graduation-cap.svg" width="60" height="60" alt="Academic">
<h1>Projeto Integrador: Freitas Autocenter</h1>
<p><strong>Sistema de Gestão e Automação de Processos Automotivos</strong></p>
<hr>
<p>
<strong>Instituição:</strong> UNIVERSIDADE ESTADUAL DO MARANHÃO


<strong>Curso:</strong> ANALISE E DESENVOLVIMENTO DE SISTEMAS


<strong>Acadêmico:</strong> Rikelmy Rabelo e Guilherme Moreira | <strong>Orientador:</strong> João Pedro
</p>
</div>

📄 Resumo do Projeto </p>
Este sistema foi desenvolvido como requisito parcial para a obtenção da terceira nota na disciplina de Engenharia de Software, servindo como instrumento de avaliação técnica e prática. O objetivo deste projeto é demonstrar a proficiência na aplicação de conceitos fundamentais de engenharia de software, incluindo arquitetura de sistemas distribuídos, modelagem relacional de dados, implementação de APIs RESTful e criação de interfaces SPA (Single Page Application) modernas e responsivas.

🏗️ Arquitetura e Stack Técnica </p>
A aplicação foi construída sobre uma arquitetura desacoplada (Client-Server), utilizando:

Backend: ASP.NET Core Web API (NET 10.0) com padrão Repository/Controller.

Frontend: Blazor WebAssembly (WASM) para uma experiência de usuário rica (SPA).

Persistência: Entity Framework Core com suporte a Migrations e SQLite.

Testes: Suíte de testes de unidade e integração utilizando xUnit.

🧩 Implementações de Engenharia de Software
1. Lógica de Negócio: Itens Externos
Diferente de sistemas de varejo comum, este projeto implementa uma regra de "IsExternal". Peças fornecidas pelo cliente são registradas para fins de auditoria e garantia, mas são isoladas por meio de algoritmos de filtragem para não inflarem o patrimônio líquido da empresa em relatórios financeiros.

2. Agrupamento Dinâmico de Dados
Para otimizar a visualização de grandes volumes de dados, foi implementada uma lógica de agrupamento no Frontend que consolida itens com nomes idênticos mas identificadores únicos (códigos), reduzindo a carga cognitiva do usuário e mantendo a precisão do estoque.

3. Persistência de Dados e Segurança
Utilização do conceito de Soft Delete em Ordens de Serviço. Os dados excluídos são mantidos em uma camada lógica de lixeira, permitindo a recuperação de registros e garantindo a rastreabilidade histórica exigida em auditorias financeiras.

💻 Instruções de Instalação e Execução
Utilize os comandos abaixo no terminal para clonar, configurar e inicializar o ambiente de desenvolvimento.

<div align="left">
<pre style="background: #1e1e1e; color: #d4d4d4; padding: 15px; border-radius: 8px; border: 1px solid #333; font-family: 'Cascadia Code', 'Courier New', monospace; line-height: 1.5;">
<span style="color: #6a9955;">// 1. Obtenção do código fonte</span>
<span style="color: #9cdcfe;">git clone</span> https://github.com/RikelmyRabelo/NotaTresEngenhariaDeSoftware.git </p>

<span style="color: #6a9955;">// 2. Aplicação das Migrations (Database Initializer)</span>
<span style="color: #9cdcfe;">cd</span> OficinaAPI
<span style="color: #9cdcfe;">dotnet ef</span> database update

<span style="color: #6a9955;">// 3. Execução da API e Web Client</span>
<span style="color: #9cdcfe;">dotnet run</span> --project OficinaAPI
<span style="color: #9cdcfe;">dotnet run</span> --project OficinaBlazor
</pre>

</div>

🧪 Verificação de Qualidade (Q.A.)
O projeto foi submetido a testes rigorosos de integração para validar as regras de negócio críticas, como cálculos de inadimplência e baixas automáticas de estoque.

<div align="left">
<pre style="background: #1e1e1e; color: #d4d4d4; padding: 15px; border-radius: 8px; border: 1px solid #333; font-family: 'Cascadia Code', 'Courier New', monospace;">
<span style="color: #ce9178;">Microsoft (R) Test Execution Command Line Tool</span>
<span style="color: #9cdcfe;">dotnet test</span>

<span style="color: #b5cea8;">Test Run Successful.</span>
<span style="color: #b5cea8;">Total tests: 15. Passed: 15. Failed: 0.</span>
</pre>

</div>

<div align="center">
<p><em>Este sistema representa a aplicação prática dos conceitos de programação orientada a objetos, banco de dados e design de sistemas web.</em></p>
<sub>Última atualização: Março de 2026</sub>
</div>
