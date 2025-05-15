# Git

## Fluxo básico de controle de versão

### Incializar um repositório

> A partir de um diretório, execute o comando abaixo

```shell
git init
```

# Proposta de Fluxo com Controle de versão
## TCC
```mermaid
gitGraph
    commit id: "Inclusão de README"
    commit id: "Página inicial"
    branch about-us
        commit id: "About"
    checkout main
    branch contact-us
    commit id: "Contact Form"
    checkout main
    merge about-us
    checkout main
    merge contact-us
    branch login
    commit
    commit
    checkout main
    merge login
    branch feed
    commit
    commit
    branch feed-backend
    commit
    commit
    checkout feed
    merge feed-backend
    checkout main
    merge feed
```