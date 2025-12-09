Desbravar - https://www.camara.leg.br/transparencia/

Pontos a aproveitar no roadmap do "Tô De Olho" a partir das páginas de transparência da Câmara:

- Resultados legislativos (https://www.camara.leg.br/transparencia/resultados-legislativos/): séries anuais (2014-2024, 2025 em construção) por tema e tipo de proposição; alinhar requisitos de ingestão histórica e visualizações comparativas.
- Receitas e despesas (https://www2.camara.leg.br/transparencia/receitas-e-despesas): execução orçamentária e pesquisa de despesas; mapear como fonte primária para ETL e dashboards de execução.
- Licitações e contratos (https://www.camara.leg.br/licitacoes-e-contratos/): lista de contratos com valores; prever módulo de acompanhamento de contratos e alertas por fornecedor/valor.
- Gastos parlamentares (https://www.camara.leg.br/transparencia/gastos-parlamentares/): cota parlamentar, verba de gabinete, moradia, viagens e remuneração; núcleo para perfis de deputados e comparações.
- Recursos humanos (https://www.camara.leg.br/transparencia/recursos-humanos): distribuição de pessoal (ativos, aposentados, pensionistas); útil para cruzamentos organizacionais e contexto de custos de pessoal.
- Acesso à informação (https://www2.camara.leg.br/transparencia/acesso-a-informacao): canal oficial de pedidos; referenciar como complemento institucional ao que o produto oferece.
- Gestão estratégica (https://www2.camara.leg.br/a-camara/estruturaadm/gestao-na-camara-dos-deputados): visão de planejamento interno; pode embasar indicadores institucionais de apoio.

Sugestões de próximos passos no roadmap:

1) Coleta e catalogação das URLs acima, verificando formatos disponíveis (páginas, CSV, APIs) antes de depender de scraping de gráficos.
2) Ingestão inicial: ingestão incremental por ano para resultados legislativos e execução orçamentária; normalização por deputado e tema.
3) Dashboards: propostas aprovadas/rejeitadas, gastos parlamentares por categoria, contratos por fornecedor/valor e evolução temporal.
4) Alertas: variações atípicas de gastos parlamentares, novos contratos de alto valor e mudanças no andamento de proposições.
5) Documentação: registrar limitações (p. ex., dados gráficos sem download direto) e complementar com fontes alternativas quando necessário.