# Como contribuir com o ARGOS

Este documento define o fluxo de colaboração utilizado nos repositórios da organização ARGOS.

## Jira e GitHub

O Jira é a fonte oficial para demandas, responsáveis, prioridades e prazos. O GitHub é utilizado para desenvolver, revisar e armazenar código e documentos.

Sempre que possível, uma alteração deve estar relacionada a uma demanda do Jira.

## Branches

Não desenvolva diretamente na branch `main`. Crie uma branch específica para cada alteração.

Padrões:

```text
feature/ARGOS-12-cadastro-propriedade
fix/ARGOS-18-corrigir-conexao
docs/ARGOS-21-atualizar-modelo-logico
refactor/ARGOS-25-organizar-daos
```

Prefixos:

- `feature/`: nova funcionalidade
- `fix/`: correção de erro
- `docs/`: documentação
- `refactor/`: melhoria interna sem mudar a funcionalidade
- `test/`: criação ou ajuste de testes
- `chore/`: configuração ou manutenção

## Commits

Use mensagens curtas e objetivas:

```text
feat: implementar cadastro de propriedade
fix: corrigir validação de usuário
docs: atualizar modelo lógico
refactor: organizar classes DAO
test: adicionar teste de conexão
chore: atualizar dependências do Maven
```

Evite mensagens genéricas como `alterações`, `teste`, `pronto` ou `versão final`.

## Pull Requests

Ao concluir uma alteração:

1. Atualize sua branch com a versão mais recente da `main`.
2. Revise os arquivos modificados.
3. Confirme que senhas e dados privados não foram adicionados.
4. Abra um Pull Request para a `main`.
5. Relacione a demanda correspondente do Jira.
6. Solicite a revisão de outro integrante.
7. Faça as correções solicitadas antes do merge.

Exemplo de título:

```text
[ARGOS-12] Implementar cadastro de propriedade
```

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
