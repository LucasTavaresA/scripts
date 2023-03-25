# Shellscripts

**Lembre-se de mudar as flags caso for usar os scripts em uma outra build do dmenu**

**Recomendo modificar/analizar os scripts ao seu gosto, ou ver/entender como eles funcionam antes de usa-los**

## wayland/xorg print

Varias formas de captura de tela, com temporizadores

## transadd

Chamado pelo `transmission-remote.desktop`, adiciona torrent e notifica

## checar_updates

Checa updates e manda notificação caso existam mais de 30 updates pendentes

Dependencias pacman: pacman-contrib

**Caso o sistema não use o pacman é necessário habilitar execução sem senha do comando que atualiza a lista de pacotes no doas,sudo,etc.**

## gerar_números

Gera números aleatórios ate ser cancelado

## musica

Separa nome da musica tocando no mpd e a posição da musica na playlist

Notifica com `musica notificar`, Retorna nome e posição se usado com `musica tocando`

Troca de musica com `musica ante e musica prox`

## volume

Mostra porcentagem de volume e ícone que muda dependendo do volume

## fzf_emojis

Seleciona e copia um emoji com o fzf

## fzf_man

Abra manpages e cheatsheets com o fzf, necessário criar/atualizar uma lista com `fzf_man update`

Dependências para cheatsheets: `cheat`

## term_open

Abre o terminal na variável `$TERMINAL` e adapta flags ao terminal usado
Mais detalhes usando `term_open -h` ou lendo a ajuda no código fonte

## menu mont

Monta e desmonta drives e isos

## menu pesquisar

Abre uma lista de engines para pesquisa usando "aliases" como no qutebrowser

## xchecklog

Dentro de um repo [void-packages](https://github.com/void-linux/void-packages) checa o ultimo git log the uma lista de pacotes xbps

Exemplo: `xpkg -m | xchecklog`

Dependências: xtools
