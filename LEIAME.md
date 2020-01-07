# Vertigo Konga Helm Chart

Este projeto é um fork do original (https://github.com/pantsel/konga). Seu objetivo é manter um pipeline para build de um helm chart público enquanto não existir um chart oficial do Konga.

O chart da Vertigo encontra-se em https://vertigobr.gitlab.io/ipaas/konga/ (mantido em Gitlab Pages). O gitlab da Vertigo mantém um mirror deste projeto em https://gitlab.com/vertigobr/ipaas/konga e é este mirror que mantém o chart publicado.

## Como importar

Este chart pode ser importado via linha de comando:

```sh
helm repo add konga https://vertigobr.gitlab.io/ipaas/konga/
```

Este chart também pode ser importado como subchart na forma de dependência:

```yaml
dependencies:
- name: konga
  version: 1.0.0
  repository: https://vertigobr.gitlab.io/ipaas/konga
```
