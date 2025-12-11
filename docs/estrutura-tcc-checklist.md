## Estrutura sugerida e checklists — alinhado ao `main.tex` (TCC "Tô De Olho")

Use como guia rápido para manter coerência com `main.tex`, `docs/context.md` e padrões de formatação (\textit{}, \texttt{}, \textbf{}). Ajuste conforme o texto evoluir.

### Esqueleto comentado conforme `main.tex`
- **Visão geral**: Breve apresentação do projeto e do propósito do documento.
- **Declaração do Problema**: Contexto de transparência/LAI, dificuldade de acesso e interpretação da API da Câmara, urgência eleitoral 2026.
- **Proposta de Solução de Software**: Descrição do \textit{Tô De Olho} (plataforma web), valor para o cidadão, funcionalidades-chave.
- **Tecnologias adotadas**: Arquitetura de \textit{microservices} em Go; Next.js 15/TypeScript/Tailwind; PostgreSQL, Redis, RabbitMQ/PubSub; Docker/K8s; CI/CD GitHub Actions; fontes de dados (API v2 Câmara + arquivos em massa).
- **Trabalhos Relacionados**: Portal da Transparência, Dados Abertos Câmara, Ranking dos Políticos, Serenata de Amor; diferenciar pelo foco em consolidação + UX acessível.
- **Requisitos**: Funcionais e não-funcionais listados; manter rastreabilidade (ex.: RF01–RF14, RNF01–RNF13) e coerência com a solução proposta.
- **Design (Projeto UML)**: Diagramas exigidos pelo modelo (classes, casos de uso obrigatório; demais conforme orientação). Referenciar se ainda pendente.
- **Visão arquitetural**: Justificativa da arquitetura, microsserviços principais, comunicação síncrona/assíncrona, ingestão híbrida (backfill + sync diário), infraestrutura Docker/K8s.
- **Modelo de Banco de Dados**: Descrição lógica/física se houver banco; relacionar com módulos (deputados, despesas, atividades, usuários).
- **Testes de Software**: Estratégia de testes (manuais/automatizados), ferramentas, cobertura alvo.
- **Implantação**: Plataforma de hardware/software, dependências, passos de deploy (CI/CD).
- **Manual do Usuário**: Fluxos principais, telas, instruções de uso; figuras quando possível.
- **Agradecimentos**: Opcional.
- **Apêndices**: Materiais complementares.
- **Glossário, Siglas e Abreviações**: Definições essenciais para o leitor.

### Checklists rápidos por seção (seguir ordem do `main.tex`)
- **Visão geral**: [ ] Propósito claro; [ ] Escopo do documento situado.
- **Declaração do Problema**: [ ] Problema de pesquisa de `docs/context.md`; [ ] Evidenciar dispersão/complexidade dos dados; [ ] Urgência eleitoral 2026; [ ] Conexão com transparência/LAI.
- **Proposta de Solução**: [ ] Descrever plataforma e público-alvo; [ ] Funcionalidades-chave (perfil, despesas, votações); [ ] Benefício para fiscalização cidadã.
- **Tecnologias adotadas**: [ ] Listar stack completo (Go, Next.js 15, PostgreSQL, Redis, RabbitMQ/PubSub, Docker/K8s, GitHub Actions); [ ] Fontes de dados (API v2 + arquivos em massa); [ ] Motivar escolhas.
- **Trabalhos Relacionados**: [ ] Citar iniciativas e limitações; [ ] Destacar diferenciais do \textit{Tô De Olho}.
- **Requisitos**: [ ] RFs e RNFs enumerados; [ ] Coerentes com funcionalidades; [ ] Sem métricas inventadas não suportadas.
- **Design (UML)**: [ ] Diagramas mínimos (classes, casos de uso) sinalizados; [ ] Outros diagramas conforme combinado com orientador; [ ] Indicar pendências se ainda não desenhados.
- **Visão arquitetural**: [ ] Microsserviços listados; [ ] Comunicação REST + fila; [ ] Ingestão híbrida (backfill + cron); [ ] Infra Docker/K8s; [ ] Justificativa (escalabilidade, resiliência).
- **Modelo de Banco de Dados**: [ ] Entidades principais alinhadas aos serviços; [ ] Normalização e chaves claras; [ ] Seção preenchida ou marcada como a completar.
- **Testes de Software**: [ ] Estratégia (manual/auto); [ ] Ferramentas; [ ] Critérios de aceitação; [ ] Cobertura desejada.
- **Implantação**: [ ] Ambiente alvo; [ ] Dependências; [ ] Pipeline CI/CD; [ ] Passos de deploy.
- **Manual do Usuário**: [ ] Fluxos descritos; [ ] Telas/figuras; [ ] Instruções claras para usuário leigo.
- **Agradecimentos**: [ ] Preenchido ou mantido opcional.
- **Apêndices**: [ ] Materiais extras listados; [ ] Referenciados no texto.
- **Glossário/Siglas**: [ ] Termos-chave definidos; [ ] Padrão de formatação.

### Notas rápidas de estilo
- Linguagem acadêmica em português, direta; evitar jargão automático.
- Usar \textit{} para termos em inglês; \texttt{} para nomes de serviços/tecnologias quando fizer sentido; \textbf{} para ênfases pontuais.
- Resumir trechos longos; não inventar métricas ou autores; se métrica for expectativa, rotular como tal.