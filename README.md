# Gestão de Banco de Dados e BI

Repositório da disciplina de Gestão de Banco de Dados e BI, parte da Pós-Graduação em Data Analytics e Marketing da ESPM, turma 61A1-2.

## Visão geral da disciplina

A disciplina tem como foco a base conceitual e prática necessária para compreender como dados estruturados são armazenados, modelados, consultados e transformados em informação útil para a tomada de decisão. O percurso combina fundamentos de banco de dados relacionais, modelagem de dados, arquitetura de dados, SQL, modelagem dimensional e Business Intelligence.

Ao longo do curso, os estudantes trabalham com os principais conceitos que conectam tecnologia, dados e negócio: integridade referencial, normalização, modelos ER, star schema, Data Warehouse, análise de requisitos, uso de SQL e discussão crítica sobre ferramentas e arquiteturas de dados.

A proposta didática valoriza a aprendizagem ativa por meio de problemas reais ou realistas, com atividades semanais e um projeto integrador que conecta teoria e prática no contexto de negócio.

## Objetivo deste site

Este site funciona como material de apoio do curso: ele centraliza as aulas e as atividades avaliativas em uma interface simples e navegável.

A ideia não é repetir em excesso o conteúdo do curso, mas sim organizar a disciplina em uma estrutura prática para consulta rápida, acompanhamento das atividades e acesso aos materiais relevantes. O site foi pensado para facilitar:

- a visualização do percurso da disciplina;
- o acesso às aulas e aos materiais de cada unidade;
- a leitura das atividades avaliativas e do fluxo de entrega;
- o uso de arquivos e datasets usados em aula.

## Como navegar no site

A página inicial (`index.html`) é um hub estático com duas grades de cartões — Aulas e Atividades — que linkam diretamente para a página de cada unidade em `content/`. Não há roteamento nem carregamento dinâmico: cada aula e cada atividade é um arquivo HTML autocontido, com sua própria navegação interna por telas (menu → tópicos → menu).

Dentro de cada aula ou atividade, um rodapé de navegação lateral leva à aula anterior/seguinte e à atividade correspondente daquela semana.

## Execução local

Para visualizar o projeto localmente, basta abrir o arquivo index.html em um navegador, ou rodar um servidor simples na pasta do projeto, por exemplo com:

```bash
python -m http.server 8000
```

Depois, acesse:

```text
http://localhost:8000
```

## Estrutura do projeto

- index.html: hub estático com os links para todas as aulas e atividades;
- content/: uma página HTML autocontida por aula (`aula-01.html`…`aula-08.html`) e por atividade (`atividade-01.html`…`atividade-08.html`);
- recursos/: datasets, arquivos de apoio e recursos utilizados na disciplina;
- docs/adr/: decisões de arquitetura registradas ao longo do projeto;
- CONTEXT.md: glossário dos termos usados no repositório;
- README.md: documentação do projeto e orientação geral.

## Observações

Este repositório é um material didático e acadêmico, refletindo a organização do curso em determinada turma e período. As informações de planejamento, avaliação e materiais podem ser atualizadas conforme o desenvolvimento da disciplina, mas a intenção do portal é manter a experiência de consulta clara e acessível.

Para mais detalhes sobre o conteúdo específico de cada aula e atividade, o melhor caminho é navegar diretamente no site e consultar as seções correspondentes.

