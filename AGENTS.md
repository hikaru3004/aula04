# Instruções do projeto

- `opencode.json` roda `servidor.py` via `.venv/bin/python`; não use o python global.
- Skill `relatorio-de-atividade` (`.opencode/skills/relatorio-de-atividade/SKILL.md`) define o formato obrigatório do relatório: `git log --oneline`, `git diff --stat`, seções em ordem fixa (`O que foi pedido`, `O que foi feito`, `O que falhou`, `Como foi resolvido`, `Ferramentas de IA`), máximo uma página, português BR, primeira pessoa do singular, terminar perguntando o que faltou.
- Se o repo não tiver commits (`git log` vazio), registre isso explicitamente; não invente histórico.
- `servidor.py`: pesos das avaliações são `N1=3, N2=3, N3=4`; situação: `>=7.0` aprovado, `>=5.0` exame, `<5.0` reprovado, incompleto se faltar nota.
- Não há README; confie em `opencode.json`, `servidor.py` e `.opencode/skills/` como fontes de verdade.
