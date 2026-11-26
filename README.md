# DRAPHOS Agency Manager — versão 1

CRM local funcional, sem dependências. Abra index.html ou publique no GitHub Pages: crie um repositório, envie index.html, style.css e app.js para a raiz, abra Settings > Pages > Deploy from a branch > main / root.

Módulos: dashboard, prospecção, funil, clientes, tarefas, conteúdo, financeiro, contratos, resultados, WhatsApp, CSV e backup JSON. Começa vazio, sem dados fictícios.

**Limitações:** dados armazenados em localStorage no navegador; não há autenticação, servidor, sincronização, portal de clientes, integração automática com Google/Meta ou IA. O WhatsApp abre uma mensagem para revisão e envio manual. Não publique dados pessoais no repositório. Use backups e não armazene informações sensíveis nesta versão. Para uso em equipe, implementar banco de dados e autenticação com controle de acesso antes de operar com dados reais.

## Importação de prospecções em PDF
Em Prospecção, selecione um PDF com texto pesquisável. O leitor PDF.js é carregado de CDN (internet necessária). O arquivo é processado no navegador, sem envio do PDF ao servidor. Revise a tabela editável e clique em Importar para o funil. O sistema ignora nomes duplicados. Formato preferencial: Nome da empresa: ..., Estrelas: ..., Avaliações: ..., Melhor comentário: ..., Telefone: ..., Site: ...; repita para cada empresa. PDFs escaneados e tabelas sem rótulos podem exigir preenchimento manual; não há OCR. O PDF original não é armazenado. Os dados continuam locais, com a mesma chave da versão anterior.

## V3 — Respostas e agenda
Na Prospecção, use Resposta / retorno para registrar o resultado e agendar uma tarefa vinculada à empresa. A agenda permite filtrar atrasados, hoje, amanhã e próximos dias. O mesmo armazenamento local da V2 é mantido. Não há notificações externas automáticas.

## V4 — Metas semanais
Em Tarefas, selecione a semana (segunda a domingo), crie metas quantitativas e registre progresso manualmente pelos botões +1/-1 ou Editar. O painel contabiliza automaticamente tarefas concluídas e vencidas pelo prazo da semana. Metas são salvas no mesmo armazenamento local e incluídas no backup JSON exportado. A agenda de prospecção e os controles de resposta da V3 permanecem disponíveis.
