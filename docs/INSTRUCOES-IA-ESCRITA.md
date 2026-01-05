# 🚨 INSTRUÇÕES OBRIGATÓRIAS PARA IAs NA ESCRITA DO TCC

> **Este documento deve ser referenciado SEMPRE que uma IA auxiliar na escrita acadêmica deste projeto.**

---

## ❌ PROIBIÇÕES ABSOLUTAS

1. **NUNCA invente referências bibliográficas** — Toda citação deve vir de um artigo/livro que COMPROVADAMENTE existe.

2. **NUNCA crie nomes de autores fictícios** — Se não souber a referência exata, PERGUNTE ao usuário ou use `[REFERÊNCIA NECESSÁRIA]`.

3. **NUNCA infira dados de publicação (ano, revista, páginas)** — Só cite se tiver certeza absoluta da fonte.

4. **NUNCA escreva afirmações teóricas sem base** — Toda afirmação conceitual deve ser atribuída a um autor ou marcada como `[FONTE REQUERIDA]`.

---

## ✅ REGRAS OBRIGATÓRIAS

### Para Citações

1. **Somente cite o que foi fornecido pelo usuário** nos documentos de resumo (ex: `resumo-democracia-digital.md`).

2. **Se precisar de referências adicionais**, faça uma busca web para confirmar que a publicação existe ANTES de citá-la.

3. **Use marcadores de pendência** quando não tiver certeza:

   - `[AUTOR?]` — autor não confirmado
   - `[ANO?]` — ano não confirmado
   - `[FONTE REQUERIDA]` — precisa de referência
   - `TODO: buscar referência para esta afirmação`

4. **Formato de verificação obrigatório** antes de citar:
   - Nome completo do autor
   - Título exato do trabalho
   - Ano de publicação
   - Revista/conferência/editora
   - DOI ou URL quando disponível

### Para Conceitos Técnicos

1. **Arquitetura de Software (microsserviços, etc.)** — Use documentação oficial (Martin Fowler, Sam Newman) ou artigos de conferências IEEE/ACM.

2. **ETL e Engenharia de Dados** — Prefira documentação técnica (Apache, cloud providers) a artigos acadêmicos vagos.

3. **Se não houver referência confiável**, escreva de forma descritiva sem citação direta:
   > ❌ "Segundo Silva (2021), microsserviços são..."
   > ✅ "A arquitetura de microsserviços caracteriza-se por..."

---

## 📋 CHECKLIST ANTES DE ENTREGAR TEXTO

- [ ] Todas as citações `\cite{}` existem no arquivo `.bib`?
- [ ] Todas as referências no `.bib` foram verificadas em bases acadêmicas (Google Scholar, IEEE, ACM)?
- [ ] Não há afirmações sem fonte em seções teóricas?
- [ ] Marcadores `[FONTE REQUERIDA]` foram resolvidos ou sinalizados ao usuário?

---

## 📚 FONTES CONFIÁVEIS PARA ESTE TCC

### Democracia Digital e Transparência

- Resumo do usuário: `tcc-escrita/docs/resumo-democracia-digital.md`
- GOMES, Wilson (todos os trabalhos)
- AVELINO et al. (2021) — Democracia Digital IPEA
- Portal de Periódicos CAPES

### Arquitetura de Software

- FOWLER, Martin — martinfowler.com
- NEWMAN, Sam — "Building Microservices" (O'Reilly)
- IEEE Software / ACM Transactions

### APIs Governamentais

- Documentação oficial do Senado Federal
- Portal de Dados Abertos do Governo Federal

---

## 📝 EXEMPLO DE TEXTO CORRETO

### ❌ INCORRETO (referência inventada):

```latex
A arquitetura de microsserviços promove escalabilidade granular \cite{silva2023microservices}.
```

### ✅ CORRETO (sem referência, mas factual):

```latex
A arquitetura de microsserviços promove escalabilidade granular,
permitindo alocar recursos apenas aos componentes mais demandados.
```

### ✅ CORRETO (com referência verificada):

```latex
Taibi, Lenarduzzi e Pahl investigaram os processos de migração
para microsserviços em estudo empírico publicado na IEEE Cloud Computing \cite{taibi2017microservices}.
```

---

_Última atualização: 20/12/2024_
