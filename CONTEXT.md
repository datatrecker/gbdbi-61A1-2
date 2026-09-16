# GBDBI Site

Site da disciplina Gestão de Banco de Dados e BI (ESPM), reconstruído como uma coleção de páginas HTML estáticas e independentes — sem SPA, sem roteamento dinâmico.

## Language

**Aula**:
Página de conteúdo de uma semana de aula: um arquivo `content/aula-NN.html` autocontido, com `<style>` próprio (tema bordô) e navegação interna por `show()`.
_Avoid_: Lesson, lição

**Atividade**:
Página de uma atividade avaliativa/prática vinculada a uma Aula, no mesmo formato de arquivo `content/atividade-NN.html`.
_Avoid_: Exercício, tarefa (como nome de página)

**Hub**:
O `index.html` na raiz do site — página única com grade de cards que lista todas as Aulas e Atividades e linka diretamente para cada uma. Substitui a antiga casca de SPA.
_Avoid_: SPA shell, menu principal, sidebar

**PEA**:
Plano de Ensino e Aprendizagem da disciplina. Fora do escopo do site reconstruído — as páginas administrativas derivadas dele (Plano de Ensino, Avaliação, Recursos) foram removidas junto com o SPA que as gerava.
