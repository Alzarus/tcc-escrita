# Comandos de Compilação — TCC Tô De Olho

## Compilar PDF (Completo)

```powershell
# Executar na pasta tcc-escrita/
cd tcc-escrita
pdflatex -interaction=nonstopmode main.tex
bibtex main
pdflatex -interaction=nonstopmode main.tex
pdflatex -interaction=nonstopmode main.tex
```

## Compilar PDF (Comando Único)

```powershell
# PowerShell - executa tudo em sequência
cd tcc-escrita; pdflatex -interaction=nonstopmode main.tex; bibtex main; pdflatex -interaction=nonstopmode main.tex; pdflatex -interaction=nonstopmode main.tex
```

## Notas

- **Por que 3x pdflatex?** Necessário para resolver referências cruzadas e índice
- **bibtex**: Processa o arquivo `referencias.bib` e gera citações
- **-interaction=nonstopmode**: Não para em erros, continua até o fim
- **Saída**: `main.pdf` na mesma pasta
