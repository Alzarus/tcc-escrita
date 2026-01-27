# 📄 TCC - Documentação e Texto Acadêmico

**Autor**: Pedro Batista de Almeida Filho  
**Curso**: Análise e Desenvolvimento de Sistemas (ADS) - IFBA

---

Este diretório contém os arquivos fontes em **LaTeX** referentes à parte escrita (monografia/relatório técnico) do projeto **Tô De Olho** (Plataforma de Transparência Parlamentar do Senado Federal).

## 📂 Estrutura do Documento

A organização dos arquivos segue o padrão para compilação LaTeX:

- **`main.tex`**: Arquivo mestre que estrutura o documento (chamadas de pacotes, metadados e inclusão de capítulos).
- **`src/sections/`**: Contém o texto dividido por capítulos:
  - `introducao.tex`: Contextualização e objetivos.
  - `fundamentacao.tex`: Revisão bibliográfica e conceitos (DDD, Clean Arch, etc).
  - `metodologia.tex`: Método de pesquisa e abordagem de desenvolvimento.
  - `design.tex`, `implantacao.tex`, `testes.tex`: Detalhes técnicos da solução.
- **`src/figures/`**: Diretório para imagens, gráficos e diagramas utilizados.
- **`referencias.bib`**: Base de dados bibliográfica (formato BibTeX).
- **`relatorio_tcc_ads_ifba.cls`**: Classe de formatação customizada para o padrão ABNT/IFBA.

## 🛠️ Como Compilar

### Pré-requisitos

- Distribuição LaTeX (TeX Live, MikTeX ou similar).
- Compilador `pdflatex` e `bibtex`.

### Comandos de Compilação

Para gerar o PDF final (`main.pdf`) com referências e índices atualizados, você pode usar os comandos abaixo.

**Opção 1: Passo a passo (PowerShell)**

```powershell
# Executar na pasta tcc-escrita/
pdflatex -interaction=nonstopmode main.tex
bibtex main
pdflatex -interaction=nonstopmode main.tex
pdflatex -interaction=nonstopmode main.tex
```

**Opção 2: Comando Único (PowerShell)**

```powershell
# Executa toda a sequência de uma vez
cd tcc-escrita; pdflatex -interaction=nonstopmode main.tex; bibtex main; pdflatex -interaction=nonstopmode main.tex; pdflatex -interaction=nonstopmode main.tex
```

### Notas sobre a Compilação

- **Por que 3x pdflatex?** É necessário executar múltiplas vezes para resolver referências cruzadas (`\ref`, `\cite`), sumário e índices de figuras/tabelas.
- **bibtex**: Processa o arquivo `referencias.bib` para gerar as citações corretamente.
- **-interaction=nonstopmode**: Flag que impede a compilação de parar em erros não críticos, continuando até o final.

> **Nota**: O projeto está configurado para o idioma Português (Brasil) e segue as normas da ABNT.
