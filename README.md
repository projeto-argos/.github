# ARGOS — Configurações da Organização

Arquivos compartilhados por todos os repositórios da organização [projeto-argos](https://github.com/projeto-argos): a página pública, o guia de colaboração e o modelo de Pull Request.

## Estrutura

```text
.github/
├── profile/
│   └── README.md
├── CONTRIBUTING.md
├── PULL_REQUEST_TEMPLATE.md
└── README.md
```

## O que cada arquivo faz

| Arquivo | Para que serve |
|---|---|
| [`profile/README.md`](./profile/README.md) | Página exibida em github.com/projeto-argos, com o projeto, os links publicados, os repositórios e a equipe |
| [`CONTRIBUTING.md`](./CONTRIBUTING.md) | Padrões de branch, commit (Conventional Commits), Pull Request, merge, revisão e segurança |
| [`PULL_REQUEST_TEMPLATE.md`](./PULL_REQUEST_TEMPLATE.md) | Modelo preenchido automaticamente ao abrir um Pull Request em qualquer repositório da organização |

## Fluxo de trabalho

1. Criar uma branch a partir da `main` (por exemplo, `feature/views` ou `docs/organiza-banco`).
2. Fazer commits no padrão `tipo(escopo): descrição`.
3. Abrir um Pull Request para a `main` e pedir a revisão de outro integrante.
4. Integrar após a aprovação: Merge commit no `argos-web-crud` e Squash and merge nos demais.

As demandas, responsáveis e prazos ficam no Jira (projeto `SCRUM`). Senhas, chaves e arquivos `.env` nunca são versionados.

## Repositórios

| Repositório | Conteúdo |
|---|---|
| [argos-web-crud](https://github.com/projeto-argos/argos-web-crud) | Aplicação Java com Servlet, JSP e JDBC |
| [argos-bd](https://github.com/projeto-argos/argos-bd) | Modelagem, scripts SQL e convenção de nomenclatura |
| [argos-landingpage](https://github.com/projeto-argos/argos-landingpage) | Landing page e telas estáticas do sistema |
|
