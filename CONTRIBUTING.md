# Contribuindo para projetos MSC

## Stack padrão

- **Frontend:** TypeScript + React
- **Backend:** Node.js/Express ou FastAPI
- **Banco/Auth:** Supabase
- **Deploy:** Docker

## Conventional Commits

Use o formato: `tipo(escopo): descrição curta em português`

| Tipo | Quando usar |
|---|---|
| `feat` | Nova funcionalidade |
| `fix` | Correção de bug |
| `docs` | Apenas documentação |
| `chore` | Manutenção, deps, config |
| `refactor` | Refatoração sem mudança de comportamento |
| `test` | Adicionar ou corrigir testes |
| `ci` | Pipelines e automações |

**Exemplos:**
```
feat(auth): adicionar login com Google
fix(api): corrigir erro 500 na rota de contratos
docs(readme): atualizar instruções de setup
chore(deps): atualizar dependências de segurança
```

## Branches

| Prefixo | Uso |
|---|---|
| `feat/*` | Novas funcionalidades |
| `fix/*` | Correções de bug |
| `docs/*` | Documentação |
| `chore/*` | Manutenção e infra |

Nomeie com kebab-case: `feat/login-google`, `fix/erro-500-contratos`.

## Fluxo de trabalho

1. Abra uma issue descrevendo o problema ou funcionalidade
2. Crie a branch a partir de `main`
3. Implemente com commits atômicos e descritivos
4. Certifique-se de que CI passa antes de abrir PR
5. Abra o PR referenciando a issue (`Ref #N` ou `Closes #N`)
6. Aguarde revisão — merge apenas após aprovação

## CI obrigatório antes de merge

Todos os PRs devem passar nos checks de CI antes do merge. Não faça bypass de checks sem justificativa documentada no PR.

## O que nunca commitar

- Arquivos `.env` reais
- Tokens (GitHub, Supabase, Vercel, HF, OpenRouter etc.)
- Bancos de dados locais (`*.db`, `*.sqlite`)
- Dados de clientes ou documentos institucionais sem autorização

Use `.env.example` com valores fictícios como referência.

## Dúvidas

Abra uma issue com a label `pergunta` ou entre em contato via canal interno da MSC.
