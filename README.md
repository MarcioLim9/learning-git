# Learning git

- [x] Você deseja criar pontos na história da produção do seu projeto
      `_(git init: inicia um repo)`
      `_(git commit -m "")`
      `_(git add .)`
      `_(git -am "ele adiciona e coloca a mensagem")`

- [x] Você deseja verificar mudanças feitas no seu projeto
      `\*(git log), (git status), (git show 'número do commit')`

- [x] Você começa uma nova funcionalidade no seu projeto, sem estragar o que já foi feito.
      `_(git branch 'sua nova funcionalidade'), sem aspas`
      `_(git -b 'sua nova funcionalidade'), sem aspas`
      `_(git checkout -b 'nome da branch'), você cria e muda de branch`
      `_(git branch), lista minhas branchs`
      `_(ls -al, para conferir as mudanças)`

- [x] Você adiciona as novas funcionalidades ao seu projeto em produção
      `_(git merge 'nome da branch')`
      `_(ls -al, para conferir as mudanças)`

- [x] Você quer deletar a branch da nova funcionalidade, depois de aplicar em seu projeto.
      `\*(git branch -D 'nome da branch')`

- [x] Você quer colocar seu projeto na nuvem.
      `_(git remote add origin 'link do github')`
      `_(git remote -v), para ver os repositórios`
      `\*(git push -u origin master (só na primeira vez))`

- [x] Você vai pegar um projeto já iniciado, para trabalhar com o time
      `\*(git clone 'link do github')`

- [x] Você precisa resolver um conflito.
      `\*(o github já é uma mão na roda)`

- [x] Antes de enviar a resolução, precisamos atualizar o projeto local.
      `\*(git pull)`

- [x] Você precisa voltar um arquivo para um determinado momento da linha do tempo.
      `\*( git checkout nome-do-arquivo.ext (antes do comit))`
      `\*( git checkout 'numero do commit' nome-do-arquivo.ext)`

- [x] Você precisa recuperar algo deletado.
      `\*(git checkout -- 'nome do arquivo')`

- [x] Você precisa desfazer seus commits
      `\*(git reset --soft)` pega minhas modificações e mata o commit, mas o arquivo continua modificado e pronto pra ser comitado
      `\*(git reset --mixed (melhor pra mim))` pega minhas modificações e mata o commit, mas o arquivo continua modificado e volta para antes de ser comitado
      `\*(git reset --hard)` só ignora tudo e apaga

- `git init` // inicia a linha do tempo
- `git add` // adiciona ou atualiza mudanças para irem para a linha do tempoo
- `git commit` // adiciona um ponto na linha do tempo
- `git log --author, --graph` // visualiza os pontos na linha do tempo / commit
- `git shortlog -sn` // visualiza os pontos na linha do tempo de uma maneira reduzida
- `git reset HEAD "nome-do-arquivo.ext"` // você tira o arquivo do unstaged, tira ele do "add"
- `git status` // informa o estado das alterações do nosso projeto
- `git diff --name-only` // mostra a alteração que fizemos no arquivo direto no terminal
- `git show` // apresenta determinado ponto na história
- `git branch` // gerenciar novas linhas do tempo
- `git checkout` // manipula as linhas do tempo
- `git merge` // unir linhas do tempo
- `git push` // envia alterações locais para o repositório remoto
- `git clone` // clonar um projeto / repositório
- `git pull` // puxa do repositório remoto
- `git stash "list", "clear"` // cria uma 'pastinha' e guarda minhas mudanças para ser usadas depois com o `git stash apply`
- `git revert` // deu problema em produção, então usa o git revert, mas você pode dar um checkout no commit que quebrou e depois modificá-lo
- `git tag -a 1.0.0 -m "Mensagem"` // para definir as versões
