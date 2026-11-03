# Como contribuir com o ARGOS

Este documento define o fluxo de colaboração utilizado nos repositórios da organização ARGOS.

## Jira e GitHub

O Jira é a fonte oficial para demandas, responsáveis, prioridades e prazos. O GitHub é utilizado para desenvolver, revisar e armazenar código e documentos.

Quando a alteração tiver uma demanda no Jira (projeto `SCRUM`), informe a chave no Pull Request.

## Branches

Não desenvolva diretamente na branch `main`. Crie uma branch para cada alteração ou para a camada sob sua responsabilidade.

Padrões:

```text
feature/views
fix/corrigir-conexao
docs/organiza-banco
refactor/organizar-daos
servlet
```

Prefixos:

- `feature/` ou `feat/`: nova funcionalidade
- `fix/`: correção de erro
- `docs/`: documentação
- `refactor/`: melhoria interna sem mudar a funcionalidade
- `test/`: criação ou ajuste de testes
- `chore/`: configuração ou manutenção

Uma branch sem prefixo, com o nome da camada (por exemplo, `servlet`), pode ser usada pelo integrante responsável por ela durante todo o desenvolvimento.

## Commits

Use o padrão Conventional Commits, `tipo(escopo): descrição`. O escopo é o arquivo ou o módulo alterado e pode ser omitido quando a mudança é geral:

```text
feat(login): botão para voltar à landing page
fix(userUpdateServlet.java): trata id ausente na mensagem de erro
docs(env.example): documenta DB_POOL_MAX
refactor(authFilter.java): traduz nomes para inglês
style(loginServlet.java): corrige comentário
test(validator): adiciona teste de CPF
chore(pom.xml): atualiza dependências
fix: corrige a validação do peso
```

Tipos: `feat`, `fix`, `docs`, `refactor`, `style`, `test` e `chore`.

Evite mensagens genéricas como `alterações`, `teste`, `pronto` ou `versão final`.

## Pull Requests

Ao concluir uma alteração:

1. Atualize sua branch com a versão mais recente da `main`.
2. Revise os arquivos modificados.
3. Confirme que senhas e dados privados não foram adicionados.
4. Abra um Pull Request para a `main`.
5. Informe a demanda do Jira, quando houver.
6. Solicite a revisão de outro integrante.
7. Faça as correções solicitadas antes do merge.

O título é uma frase curta que descreve a entrega:

```text
Adiciona scripts SQL atualizados
Telas do CRUD em HTML, CSS e JavaScript
```

## Merge

- `argos-web-crud`: **Merge commit**, para manter o histórico de commits de cada camada.
- Demais repositórios: **Squash and merge**, com um commit por Pull Request.

## Revisão

O revisor deve verificar:

- Se a alteração atende à demanda
- Se o código ou documento está compreensível
- Se não existem credenciais ou dados sensíveis
- Se a aplicação continua funcionando
- Se a documentação necessária foi atualizada

## Segurança

Nunca envie:

- Senhas
- Chaves de API
- Credenciais do banco
- Arquivos `.env` reais
- Dados pessoais sem autorização
- Arquivos compilados ou temporários

Use `.env.example` apenas com nomes de variáveis e valores fictícios.
