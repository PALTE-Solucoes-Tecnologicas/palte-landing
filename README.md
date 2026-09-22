# palte-landing

Landing page de captura de lead do Palte, assistente de IA para contabilidades pequenas que coleta, classifica e cobra documentos de clientes via WhatsApp.

## Objetivo

Captar leads de escritórios de contabilidade interessados no Palte. Este site é independente do produto principal; quando o hub estiver pronto, haverá um link para o aplicativo em app.<dominio>.

## Stack

- **Web:** Next.js + TypeScript (App Router), deploy na Vercel
- **API:** NestJS + TypeScript, containerizado com Docker
- **Banco de dados:** Postgres (armazenamento de leads)

## Estrutura de pastas

```
palte-landing/
├── web/     Next.js (App Router, TypeScript) — interface da landing page
├── api/     NestJS — recebe e persiste leads, expõe endpoint de cadastro
└── docs/    Decisões de arquitetura e anotações do projeto
```

## Fluxo de branches

- `feature/*` e `fix/*` saem de `dev`
- PR de `feature/*` ou `fix/*` para `dev`
- Release via PR de `dev` para `main`
- `main` está protegida: 1 aprovação obrigatória, sem push direto

## Convenção de commits

Seguimos [Conventional Commits](https://www.conventionalcommits.org):

- `feat`: nova funcionalidade
- `fix`: correção de bug
- `chore`: tarefas de manutenção e configuração
- `docs`: documentação
- `refactor`: refatoração sem mudança de comportamento
- `test`: adição ou correção de testes

## Como rodar localmente

A definir após scaffold.

## LGPD

Leads são dados pessoais. O formulário deve coletar consentimento explícito antes de enviar os dados. Não versionar dados reais em nenhuma circunstância.

## Time

| Membro | Papel                   |
|--------|-------------------------|
| Pedro  | Infra, segurança, cloud |
| Tacin  | Dev + IA                |
| Luccas | Dev + IA                |
| Junior | Dados                   |
| Erik   | Dados + IA              |

## Contexto

Projeto acadêmico do CESAR School com potencial de virar startup.
