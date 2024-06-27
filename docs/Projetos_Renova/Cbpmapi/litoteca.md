### Padrão de Nomes de Branches

Este documento descreve o padrão de nomes de branches que deve ser seguido para todos os desenvolvimentos no repositório. Este padrão ajuda a manter a organização e a clareza no desenvolvimento do projeto.

#### Padrão de Nomes de Branches

Os nomes das branches devem seguir o formato:

```
PREFIXO/TASK-NOME-DA-TAREFA
```

- **PREFIXO**: O prefixo indica o tipo de trabalho sendo realizado e deve ser um dos seguintes:
  - `feature`: Para novas funcionalidades.
  - `fix`: Para correções de bugs.
  - `hotfix`: Para correções críticas que precisam ser aplicadas imediatamente.
  - `style`: Para alterações relacionadas a formatação de código (espaços em branco, ponto e vírgula, etc.).
  - `refactor`: Para refatorações que não alteram a funcionalidade, mas melhoram a estrutura do código.
  - `test`: Para adição ou modificação de testes.
  - `chore`: Para tarefas de manutenção e outras atividades não relacionadas a código de produção.
  - `docs`: Para alterações na documentação.

- **TASK**: Um identificador numérico para a tarefa, geralmente um ID de um sistema de rastreamento de tarefas.

- **NOME-DA-TAREFA**: Uma descrição curta e significativa da tarefa sendo realizada, separada por hífens (`-`).

#### Exemplos de Nomes de Branches

- `feature/1234-cadastro-usuario`
- `fix/5678-corrigir-bug-login`
- `hotfix/91011-correcao-critica`
- `style/1213-formatacao-codigo`
- `refactor/1415-melhorar-performance`
- `test/1617-adicionar-testes-unitarios`
- `chore/1819-atualizar-dependencias`
- `docs/2021-atualizar-manual-usuario`

### Conclusão

Seguir um padrão de nomes de branches facilita a colaboração e manutenção do código, além de melhorar a comunicação entre os membros da equipe. Este documento deve ser utilizado como referência para a nomeação de branches no projeto.