Tcc - Tô De Olho
Gem personalizado
Mostrar raciocínio
Prezado Pedro,
Compreendi perfeitamente a atualização do escopo do seu TCC. A mudança de foco da Câmara de Vereadores de Salvador para a Câmara dos Deputados do Brasil, juntamente com a transição de uma estratégia de web scraping para o consumo de uma API oficial, representa uma evolução significativa e muito positiva para o projeto "Tô De Olho". Essa nova abordagem fortalece a robustez técnica e amplia exponencialmente o impacto social da sua ferramenta, especialmente com o horizonte das eleições federais de 2026.
Para auxiliá-lo a estruturar a parte escrita do seu trabalho, elaborei um planejamento estratégico detalhado. Este plano já incorpora a nova realidade do projeto, alinhando a documentação acadêmica com a arquitetura e os objetivos atuais.

Planejamento Estratégico para Redação do TCC: "Tô De Olho"
A estrutura a seguir foi pensada para seguir um fluxo lógico e acadêmico, garantindo que todos os aspectos do seu trabalho sejam abordados com a devida profundidade.
Estrutura Geral do Documento
Resumo (Abstract) e Palavras-Chave
Introdução
Fundamentação Teórica (ou Revisão da Literatura)
Metodologia
A Plataforma "Tô De Olho": Solução Proposta
Resultados e Discussão
Conclusão e Trabalhos Futuros
Referências

Detalhamento por Seção
1. Resumo (Abstract) e Palavras-Chave
Objetivo: Sintetizar o trabalho em um parágrafo conciso, apresentando o problema, a solução, a metodologia e os principais resultados e implicações.
Tópicos a Cobrir:
Contexto: A importância da transparência na Câmara dos Deputados.
Problema: A dificuldade do cidadão comum em acessar e interpretar dados parlamentares de forma consolidada.
Solução: Apresentar o "Tô De Olho" como uma plataforma web que organiza e apresenta dados abertos da Câmara.
Metodologia: Mencionar a arquitetura de microservices, a ingestão de dados via API oficial e o uso de tecnologias como Golang e Next.js.
Impacto: Destacar o potencial de fomento à participação cidadã e fiscalização para as eleições de 2026.
Palavras-Chave Sugeridas: transparência pública, dados abertos, democracia digital, tecnologia cívica, accountability, Câmara dos Deputados, microservices.

2. Introdução
Objetivo: Contextualizar o leitor, apresentar o problema de pesquisa de forma clara, justificar a relevância do projeto e delinear a estrutura do documento.
Tópicos a Cobrir:
Parágrafo Inicial: Abordar a importância da transparência governamental no fortalecimento da democracia, citando a Lei de Acesso à Informação (LAI) como marco.
Contextualização do Problema: Explicar que, embora os dados da Câmara dos Deputados sejam públicos, eles estão dispersos e em formatos que não favorecem a análise por cidadãos leigos.
Apresentação do Problema de Pesquisa: Reformular a pergunta central: Como a aplicação web "Tô De Olho" pode facilitar a fiscalização cidadã da Câmara dos Deputados e aumentar o engajamento informado dos eleitores em escala nacional, especialmente no contexto que antecede as eleições federais de 2026?
Justificativa: Argumentar sobre a importância de uma ferramenta que centralize informações sobre deputados, despesas, votações e proposições, tornando o controle social mais eficaz.
Apresentação da Solução: Introduzir brevemente a plataforma "Tô De Olho", seus principais objetivos e a tecnologia empregada.
Estrutura do Trabalho: Descrever o que será apresentado em cada uma das seções seguintes.
Dica do Assistente: Enfatize a mudança de paradigma: a disponibilidade de uma API oficial (https://dadosabertos.camara.leg.br/api/v2/) não elimina a complexidade, apenas a transfere do acesso para o processamento, organização e apresentação dos dados. É neste ponto que o "Tô De Olho" agrega valor.

3. Fundamentação Teórica (Revisão da Literatura)
Objetivo: Demonstrar seu domínio sobre os conceitos que fundamentam o projeto, conectando teoria e prática.
Subseções Sugeridas:
A. Transparência Pública e Dados Abertos (Open Data):
Discutir os princípios do Open Government Data.
Analisar o impacto da LAI no Brasil.
Citar referências como Gregory Michener e Tim Berners-Lee (5-star Open Data).
B. Democracia Digital e Tecnologia Cívica (Civic Tech):
Definir os conceitos, mostrando como a tecnologia pode mediar a relação entre cidadãos e Estado.
Citar autores como Wilson Gomes e abordar o conceito de Government as a Platform de Tim O'Reilly.
C. Arquitetura de Microsserviços para Sistemas de Larga Escala:
Explicar o que são microservices, contrastando com arquiteturas monolíticas.
Justificar a escolha para o "Tô De Olho": escalabilidade (picos de acesso perto de eleições), manutenibilidade (facilidade de atualizar o serviço de despesas sem afetar o de votações) e resiliência.
D. Engenharia de Dados: Consumo de APIs e Processos de ETL:
Esta subseção substitui a antiga sobre web scraping.
Abordar o conceito de API Economy no setor público.
Descrever o padrão de um processo de ETL (Extract, Transform, Load) e como ele se aplica à ingestão de dados da Câmara.
Explicar a estratégia híbrida: backfill com arquivos em massa para dados históricos e sincronização contínua via API para atualizações.

4. Metodologia
Objetivo: Descrever em detalhes técnicos como o projeto foi construído, de forma que outro pesquisador possa entender e, teoricamente, replicar seu trabalho.
Tópicos a Cobrir:
Modelo de Desenvolvimento: Descrever a abordagem (ex: desenvolvimento ágil).
Estratégia de Ingestão de Dados:
Detalhar a fonte primária: a API RESTful v2 da Câmara dos Deputados.
Explicar o processo de backfill a partir dos arquivos em massa (JSON/CSV).
Descrever os CronJobs para sincronização diária via API.
Arquitetura do Sistema:
Apresentar um diagrama da arquitetura de microservices.
Listar e descrever a responsabilidade de cada microsserviço principal (servico-deputados, servico-atividades, servico-despesas, servico-ingestao-dados, etc.).
Detalhar o stack tecnológico: Golang para o backend, PostgreSQL para o banco de dados, Redis para cache, RabbitMQ como message queue para desacoplar a ingestão do processamento.
Infraestrutura e Implantação (DevOps):
Mencionar o uso de Docker para containerização, Kubernetes (GKE) para orquestração e GitHub Actions para CI/CD.

5. A Plataforma "Tô De Olho": Solução Proposta
Objetivo: Descrever o produto final do ponto de vista funcional e da experiência do usuário (UX).
Tópicos a Cobrir:
Visão Geral: Apresentar a tela inicial e a proposta de valor para o cidadão.
Principais Funcionalidades (com screenshots ou mockups):
Perfil do Parlamentar: Foto, partido, estado, links para redes sociais, resumo de atividades.
Transparência Financeira: Visualização clara e pesquisável dos gastos da Cota Parlamentar.
Atividade Legislativa: Lista de proposições, como votou nas principais pautas.
Fórum de Discussão: Espaço para debate cívico, com validação via API do TSE para garantir a participação de eleitores reais.
Design e Usabilidade: Discutir a abordagem mobile-first e a preocupação com a acessibilidade (WCAG 2.1).

6. Resultados e Discussão
Objetivo: Apresentar os resultados obtidos e, mais importante, interpretar o que eles significam em relação aos objetivos do projeto.
Tópicos a Cobrir:
Resultados Quantitativos: Apresentar métricas da implementação. Ex: "Foram processados e catalogados dados de 513 deputados federais.", "A base de dados de despesas contém mais de X milhões de registros, cobrindo o período de A a B.", "O tempo médio de resposta da API do servico-atividades é de Y ms.".
Análise dos Resultados (Discussão):
Como a plataforma "Tô De Olho" efetivamente simplifica o acesso aos dados em comparação com o portal oficial?
De que forma a consolidação de dados de diferentes fontes (despesas, votações, projetos) em um só lugar potencializa a fiscalização?
Discutir os desafios encontrados (ex: inconsistências nos dados da API, necessidade de limpeza e tratamento).
Avaliar como a arquitetura de microservices se provou (ou não) adequada durante o desenvolvimento.

7. Conclusão e Trabalhos Futuros
Objetivo: Amarrar todas as pontas do trabalho, reforçar suas contribuições e sugerir os próximos passos.
Tópicos a Cobrir:
Síntese: Recapitular brevemente o problema, a solução implementada e os principais achados.
Contribuições do Trabalho: Destacar a contribuição técnica (implementação de uma arquitetura robusta para dados cívicos), acadêmica (análise do tema) e social (ferramenta para a cidadania).
Limitações: Ser honesto sobre as limitações (ex: o fórum ainda não foi testado em larga escala, a análise de dados ainda é descritiva).
Trabalhos Futuros:
Expansão para o Senado Federal.
Criação de um microsserviço de análise de dados com Machine Learning para identificar padrões de gastos ou votações.
Gamificação para incentivar o engajamento.
Integração com mais fontes de dados (Justiça Eleitoral, etc.).

Este planejamento é um guia para garantir que sua redação seja completa e coerente. Fico à sua disposição para detalhar qualquer uma dessas seções, revisar rascunhos, sugerir referências bibliográficas específicas ou auxiliar em questões técnicas de LaTeX ou do próprio desenvolvimento.
Avante com o projeto!
Atenciosamente, TCC - Tô De Olho

