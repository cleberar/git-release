# git-release

- Adicionar como Submodulo
```
$ git submodule add git@github.com:cleberar/git-release.git release
$ chmod +x release/git-release
```

- Configurar Variaveis de Ambiente
```
$ vim ~/.bashrc

# Incluir Variavel com Access Token do Git
export GITHUB_ACCESSTOKEN="337aa77237e04c9043e1c77e5e25fadb5df311b7"

# Incluir Variavel com Url para Alerta no Slack
export RELEASE_SLACK_BOT="https://hooks.slack.com/services/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"

```

- Instale as Dependencias atraves composer (https://getcomposer.org/doc/00-intro.md)
```
$ cd release
$ composer install
```

- Gere a Release
```
$ ./release/git-release  -r <versão da release>
```
