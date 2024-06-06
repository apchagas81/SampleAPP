Tagging é uma funcionalidade que permite marcar pontos específicos na história de um repositório como importantes. Geralmente, essas tags são usadas para marcar lançamentos de versões de softwares (por exemplo, v1.0, v2.1.3, etc.), facilitando a identificação de conjuntos de alterações ou a recuperação de estados específicos do código.

### Como Funciona o Tagging:

**1. Tags Leves (Lightweight)**: Uma tag leve é como um apelido para um commit específico. Ela é um ponteiro estático para esse commit. Tags leves são criadas com o comando:

```sh
git tag <tagname>
```

**2. Tags Anotadas (Annotated)**: Uma tag anotada é armazenada como um objeto completo no banco de dados do Git. Ela contém o nome do tagger (a pessoa que criou a tag), e-mail, data e tem uma mensagem associada que pode ser fornecida pelo usuário. Tags anotadas são criadas com o comando:

```sh
git tag -a <tagname> -m "mensagem da tag"
```

Tags anotadas são recomendadas porque incluem informações adicionais úteis, como a identidade do criador da tag e a data.

### Operações Comuns com Tags:

**Listando Tags**:
Para listar todas as tags de um repositório, use:
```sh
git tag
```

**Visualizando Informações da Tag**:
Para ver as informações da tag anotada e o commit que ela marca, use:
```sh
git show <tagname>
```

**Deletando Tags**:
Para deletar uma tag local, use:
```sh
git tag -d <tagname>
```

**Publicando Tags**:
Por padrão, o comando `git push` não transfere tags para repositórios remotos. Para enviar uma tag para o seu repositório remoto, use:
```sh
git push origin <tagname>
```

Para enviar todas as tags locais que ainda não existem no repositório remoto, use:
```sh
git push origin --tags
```

**Checkout de uma Tag**:
Para verificar o código em uma tag específica, você pode fazer checkout com:
```sh
git checkout tags/<tagname>
```
