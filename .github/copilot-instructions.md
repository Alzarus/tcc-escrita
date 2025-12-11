## Copilot Instructions — TCC "Tô De Olho" (parte escrita)

### Contexto do projeto
- Este repositório cobre a **parte escrita** do TCC sobre a plataforma "Tô De Olho" (transparência da Câmara dos Deputados). A implementação (código) está em `C:\Users\pedro\OneDrive\Documentos\projetos\to-de-olho`.
- Fontes principais neste repo: `docs/estrutura-tcc-checklist.md`, `docs/context.md`, `docs/resumo-democracia-digital.md`, `docs/roadmap.md`.

### Persona e tom
- Escrever em português, registro acadêmico-formal porém claro e direto.
- Contextualizar sempre com o projeto "Tô De Olho" e seu foco em transparência parlamentar.
- Evitar jargão automático de IA; variações naturais; não inventar dados ou métricas.

### Formatação e LaTeX
- Seguir padrões descritos em `docs/context.md`: termos em inglês com `\textit{}`; código com `\texttt{}`; negrito com `\textbf{}`.
- Manter coerência com o esqueleto em `docs/estrutura-tcc-checklist.md` e `main.tex` (Resumo, Introdução, Fundamentação, Metodologia, Solução, Resultados, Conclusão, Referências).
- Preferir listas e parágrafos enxutos; cite referências já presentes em `referencias.bib` quando possível.

### Escopo e limites
- Priorizar redação, revisão e estruturação do texto do TCC neste repo.
- Para tópicos de implementação, apenas referenciar que o código está no projeto "to-de-olho"; não gerar trechos longos de código aqui.
- Não criar novos requisitos técnicos; descreva a arquitetura existente (Golang microservices, Next.js 15, PostgreSQL, Redis, RabbitMQ/PubSub, Docker/K8s, GitHub Actions) conforme `docs/context.md`.

### Fontes de verdade rápidas
- Problema de pesquisa, objetivos e metodologia: ver `docs/context.md`.
- Linha do tempo e entregas: ver `docs/roadmap.md`.
- Referenciais teóricos de democracia digital e participação: ver `docs/resumo-democracia-digital.md`.

### Qualidade e segurança
- Não inventar números, métricas ou nomes de autores além dos que estão nas fontes anexadas.
- Ao sugerir resultados ou discussões, indicar que são hipóteses se não houver dado coletado.

### Eficiência (Context7 best practices)
- Ser conciso; use apenas o contexto necessário para responder (pense em limite de tokens baixo).
- Evitar repetir trechos longos já presentes nos arquivos; resuma quando possível.
- Se sugerir regras ou melhores práticas, mantenha uma frase objetiva (ex.: "Sempre manter tom acadêmico e coerência com o problema de pesquisa").

### Saídas esperadas
- Revisões textuais, planos de seção, resumos e sugestões de referências.
- Checklist de itens faltantes na escrita (introdução, metodologia, resultados esperados, trabalhos futuros, etc.).