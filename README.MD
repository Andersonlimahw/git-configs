<h1 align="center">
  Domine o Jogo dos Commits! 🚀  
</h1>
<h2> 
  Commits Convencionais + Aliases Git para uma História Impecável no Seu Repositório!
</h2>
<p>
  <a href="#" target="_blank">
    <img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-yellow.svg" />
  </a>
  <a href="https://twitter.com/anderson.lima.dev" target="_blank">
    <img alt="Twitter: anderson.lima.dev" src="https://img.shields.io/twitter/follow/anderson.lima.dev.svg?style=social" />
  </a>
</p>

## Aliases do Git
O Git oferece a capacidade de criar aliases, ou atalhos, para comandos frequentemente usados. Isso pode economizar tempo e fornecer uma maneira conveniente de acessar funcionalidades específicas do Git. Aqui estão algumas dicas e exemplos para começar:

## Configuração global
Para configurar aliases globalmente, você pode usar o comando:

```bash
  git config -e --global
```

Isto abrirá seu editor de texto padrão com o arquivo de configuração global do Git. Você pode adicionar ou editar aliases na seção [alias]. Salve e feche o arquivo para aplicar as alterações.

## Exemplos de Aliases
Aqui estão alguns exemplos de aliases úteis que você pode adicionar ao seu arquivo de configuração:

```ini
[alias]
    st = status
    visual = !gitk
    co = checkout
    ec = config --global -e
    up = !git pull --rebase --prune $@ && git submodule update --init --recursive
    cob = checkout -b
    cm = !git add -A && git commit -m
    savepoint = !git add -A && git commit -m '🆗 SAVEPOINT'
    wip = !git add -u && git commit -m "WIP"
    undo = reset HEAD~1 --mixed
    amend = commit -a --amend
    wipe = !git add -A && git commit -qm 'WIPE SAVEPOINT' && git reset HEAD~1 --hard
    save = "!f() { git status && git add . && git commit -m \"💾 [style] ${1}\" && git status && git push;}; f"
    ...
```

## Como Consultar Aliases

Para ver todos os aliases configurados, você pode consultar o arquivo .gitconfig. Este arquivo pode estar localizado em seu diretório de usuário ou na raiz do repositório, dependendo de onde você configurou o alias.

Lembre-se, ao usar aliases, é essencial entender o que cada alias faz. Considere consultar a documentação do Git ou usando o comando git help para obter mais informações sobre os comandos subjacentes.

Comandos Úteis:

Visualizar aliases: 

```bash
  git config --get-regexp alias
```

Consultar ajuda sobre um alias específico: 

```bash
  git alias-name --help
```

## Bônus!

## Commits Convencionais
O uso de commits convencionais, em conjunto com aliases do Git, pode proporcionar um histórico de commit mais claro e fácil de entender. Aqui está uma adição à documentação que aborda commits convencionais:

Commits convencionais seguem uma convenção padronizada para mensagens de commit, tornando mais fácil entender as mudanças no histórico do repositório. Um formato comum é o Conventional Commits, que inclui um tipo, um escopo opcional e uma descrição:

```plaintext
  <tipo>(<escopo>): <descrição>
```

Exemplos de tipos:

* feat: para uma nova funcionalidade
* fix: para uma correção de bug
* chore: para tarefas de manutenção

## Consultando Commits Convencionais
Ao utilizar commits convencionais, ferramentas como semantic versioning (SemVer) e changelogs automáticos podem ser mais facilmente integradas, melhorando a rastreabilidade e a comunicação das alterações no projeto.

Observação: Certifique-se de adaptar o estilo de commits convencionais ao padrão preferido em seu projeto ou equipe.

Referências Adicionais:

[Conventional Commits Specification](https://www.conventionalcommits.org/en/v1.0.0/)

[Semantic Versioning (SemVer)](https://semver.org/)


## Oficial documentation:
https://docs.github.com/pt/copilot/quickstart

## Author

👤 **anderson.lima.dev**

* Website: instagram.com/anderson.lima.dev
* Twitter: [@anderson.lima.dev](https://twitter.com/anderson.lima.dev)
* Github: [@andersonlimahw](https://github.com/andersonlimahw)
* LinkedIn: [@andersonlimahw](https://linkedin.com/in/andersonlimahw)