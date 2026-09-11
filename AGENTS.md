# AGENTS.md — Regras do repositório `liz_isabelly_260911`

## Regra obrigatória: auto commit + push
Toda alteração feita por qualquer agente (código, docs, config) DEVE ser commitada e pushada imediatamente ao final da tarefa.

### Workflow obrigatório
1. `git status` para ver o que mudou.
2. `git add -A` (ou `git add <arquivos específicos>`).
3. `git commit -m "<tipo>: <descrição curta>"` — usar conventional commits (`feat:`, `fix:`, `chore:`, `docs:`).
4. `git push origin main` — sempre para a branch `main`, que é a branch do GitHub Pages.
5. Confirmar com `git status` que está limpo e `git log --oneline -3` + link do push.

### Proibições
- NUNCA deixar alterações apenas locais / não commitadas ao fim da resposta.
- NUNCA finalizar uma tarefa com `nothing to commit` pendente sem ter dado push.
- Se o push falhar (conflito, auth), corrigir (`git pull --rebase origin main`) e tentar de novo, e reportar.

### Contexto
- Repo: https://github.com/larandreluizinfo/liz_isabelly_260911
- Branch de deploy: `main` (`/` → GitHub Pages legacy)
- Pages: https://larandreluizinfo.github.io/liz_isabelly_260911/
