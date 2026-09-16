# Reconstruir o site como páginas HTML estáticas independentes, sem PEA

Status: accepted

O site anterior era um SPA (roteamento por hash em `index.html`, com `assets/js/{router,content,render,nav,progress,theme,app}.js` e `data/{curso,aulas,atividades}.js`) que injetava fragmentos `content/*.js` numa casca compartilhada, e incluía páginas administrativas (Plano de Ensino, Avaliação, Recursos) inteiramente derivadas do PEA da disciplina. Um conjunto de páginas `.html` autocontidas (uma por Aula/Atividade, cada uma com seu próprio `<style>` e navegação `show()`) já cobria o mesmo conteúdo de forma mais rica e sem dependência do SPA. Decidimos adotar essas páginas standalone como formato final, transformar `index.html` num hub estático de cards que linka para elas, e remover inteiramente o SPA (JS, dados e CSS de shell) e as páginas ligadas ao PEA — o site novo cobre apenas Aulas e Atividades.

## Consequences

Perde-se o rastreamento de progresso por `localStorage` (barra de progresso, pontinhos na sidebar, "marcar como concluída") e o alternador de tema claro/escuro, já que nenhuma dessas features existe nas páginas standalone e ambas dependiam do SPA. Conteúdo futuro de Plano de Ensino/Avaliação precisará de um novo lugar fora deste site, caso volte a ser necessário.
