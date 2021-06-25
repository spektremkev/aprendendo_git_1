Testendo o quite na pratica untilisando o livro do Linux torvalds 

usage: git config [<options>]

"Git init" começa o repositorio.

"Git status" mostrara os arquivos que não foram traqueados pelo git.

"Git add -A" Ele adicionara as 

"Git commit -m" - "primeiro commit de teste " - Adicionara as alteraçoes dps ao reositorio local

"Git commint -a" -  ira faser a adção a o repostitorio utilisando o "git add -A"

"Git branch" me retornara todos o "branch" na pasta do arquivo em que estamos trabalhado 

"Git log " me mostra o indereço do commit.

"git reset" existe tres tipos de git recete e estes são "git reset --soft" - "git reset --mixed" - "git reset --hard" 
todo este devem ser seguitod da seguite endereço do commit como esta exemplo "git reset - hard '03024fe9ad22290b6f1cb3892a40d638a6004a57'"
---------------------------------------------------------------------------------------------------------------
Vamos trabalhar com diferentes tipos de 'branch'  

"Git branch" me retornara todos o "branch" na pasta do arquivo em que estamos trabalhado 

Para a criação de um novo branch e bem simples basta escrever "Git branch" seguido do nome do nomo branch desta forma "Git branch novo 'bransh' "

"git checkout master" e utilizado para alterar de um "branch" 

-----------------------------------------------------------------------------------------------------------------

"git diff " me mostrar o que foi alterado no as arquivos antes dele serem comitados 


"git diff --nome-only" mostrar somente o nome dos arquivos que foram alterados 

"git diff nomedoarquivo .xxx " mostrar somente o que foi alterado arquivo

"git diff HEAD -- nomedoarquivo .xxx" não ira altera o arquivo que voi alterado 
--------------------------------------------------------------------------------------------------------------------
Enviando o repositpriao para git rub

"git remote add origin 'link do repositorio'" para cogicionar um repositorio online, para ve se funcionou "git remote "

para mais mais detalhes do repositorio eu usso o comando " git remote -v"

para faser o envio do cos comites usamos o " git push -u origin master "

alteraçao teste git hub



Config file location
    --global              use global config file

    --system              use system config file

    --local               use repository config file

    --worktree            use per-worktree config file

    -f, --file <file>     use given config file

    --blob <blob-id>      read config from given blob object

Action
    --get                 get value: name [value-regex]

    --get-all             get all values: key [value-regex]

    --get-regexp          get values for regexp: name-regex [value-regex]

    --get-urlmatch        get value specific for the URL: section[.var] URL

    --replace-all         replace all matching variables: name value [value_regex]

    --add                 add a new variable: name value

    --unset               remove a variable: name [value-regex]

    --unset-all           remove all matches: name [value-regex]

    --rename-section      rename section: old-name new-name

    --remove-section      remove a section: name

    -l, --list            list all

    -e, --edit            open an editor

    --get-color           find the color configured: slot [default]

    --get-colorbool       find the color setting: slot [stdout-is-tty]

Type
    -t, --type <>         value is given this type

    --bool                value is "true" or "false"

    --int                 value is decimal number

    --bool-or-int         value is --bool or --int

    --path                value is a path (file or directory name)

    --expiry-date         value is an expiry date

Other
    -z, --null            terminate values with NUL byte

    --name-only           show variable names only

    --includes            respect include directives on lookup

    --show-origin         show origin of config (file, standard input, blob, command line)

    --default <value>     with --get, use default value when missing entry

Junto como o "git add -A" comomado no temos abaxo.
    git add [<options>] [--] <pathspec>...
    -n, --dry-run         dry run
    -v, --verbose         be verbose

    -i, --interactive     interactive picking
    -p, --patch           select hunks interactively
    -e, --edit            edit current diff and apply
    -f, --force           allow adding otherwise ignored files
    -u, --update          update tracked files
    --renormalize         renormalize EOL of tracked files (implies -u)
    -N, --intent-to-add   record only the fact that the path will be added later
    -A, --all             add changes from all tracked and untracked files
    --ignore-removal      ignore paths removed in the working tree (same as --no-all)
    --refresh             don't add, only refresh the index
    --ignore-errors       just skip files which cannot be added because of errors
    --ignore-missing      check if - even missing - files are ignored in dry run
    --chmod (+|-)x        override the executable bit of the listed files
    --pathspec-from-file <file>
                          read pathspec from file
    --pathspec-file-nul   with --pathspec-from-file, pathspec elements are separated with NUL character

> git rev-parse --git-dir

> git status -z -u
> git symbolic-ref --short HEAD
> git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track) refs/heads/main refs/remotes/main
> git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname)
> git remote --verbose
> git config --get commit.template
> git config --global user.email
> git config --local branch.main.github-pr-owner-number
> git config --global user.name
> git status -z -u
> git symbolic-ref --short HEAD
> git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track) refs/heads/main refs/remotes/main
> git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname)
> git remote --verbose
> git config --get commit.template
> git show -s --format=%an <%ae> [%ai] e5fb28694251d36100b2ab5a3820f08728342dff
> git show -s --format=%H%n%aN%n%aE%n%at%n%ct%n%P%n%B -z e5fb28694251d36100b2ab5a3820f08728342dff
> git show -s --format=%an <%ae> [%ai] 15e24b03b30857146e8a6b703aaa0a2469dddf9e
> git show -s --format=%H%n%aN%n%aE%n%at%n%ct%n%P%n%B -z 15e24b03b30857146e8a6b703aaa0a2469dddf9e
> git show -s --format=%an <%ae> [%ai] 2194d0724fe5eec6843718d204413a877b22fb79
> git show -s --format=%H%n%aN%n%aE%n%at%n%ct%n%P%n%B -z 2194d0724fe5eec6843718d204413a877b22fb79
> git check-ignore -v -z --stdin
> git status -z -u
> git symbolic-ref --short HEAD
> git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track) refs/heads/main refs/remotes/main
> git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname)
> git remote --verbose
> git config --get commit.template
> git check-ignore -v -z --stdin
> git status -z -u
> git check-ignore -v -z --stdin
> git symbolic-ref --short HEAD
> git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track) refs/heads/main refs/remotes/main
> git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname)
> git remote --verbose
> git config --get commit.template
> git status -z -u
> git symbolic-ref --short HEAD
> git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track) refs/heads/main refs/remotes/main
> git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname)
> git remote --verbose
> git config --get commit.template
> git status -z -u
> git symbolic-ref --short HEAD
> git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track) refs/heads/main refs/remotes/main
> git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname)
> git remote --verbose
> git config --get commit.template
> git status -z -u
> git symbolic-ref --short HEAD
> git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track) refs/heads/main refs/remotes/main
> git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname)
> git remote --verbose
> git config --get commit.template
> git check-ignore -v -z --stdin
> git show --textconv :Rails-test/railsTest/bin/yarn
> git ls-files --stage -- E:\Ruby\Rails-test\railsTest\bin\yarn
> git status -z -u
> git symbolic-ref --short HEAD
> git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track) refs/heads/main refs/remotes/main
> git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname)
> git remote --verbose
> git config --get commit.template
> git check-ignore -v -z --stdin
> git check-ignore -v -z --stdin
> git show --textconv :Rails-test/railsTest/app/jobs/application_job.rb
> git ls-files --stage -- E:\Ruby\Rails-test\railsTest\app\jobs\application_job.rb
> git check-ignore -v -z --stdin
> git check-ignore -v -z --stdin
> git check-ignore -v -z --stdin
> git show --textconv :Rails-test/railsTest/app/javascript/channels/index.js
> git ls-files --stage -- E:\Ruby\Rails-test\railsTest\app\javascript\channels\index.js
> git show --textconv :Rails-test/railsTest/app/javascript/channels/consumer.js
> git ls-files --stage -- E:\Ruby\Rails-test\railsTest\app\javascript\channels\consumer.js
> git show --textconv :Rails-test/railsTest/app/javascript/channels/index.js
> git ls-files --stage -- E:\Ruby\Rails-test\railsTest\app\javascript\channels\index.js
> git show --textconv :Rails-test/railsTest/app/mailers/application_mailer.rb
> git ls-files --stage -- E:\Ruby\Rails-test\railsTest\app\mailers\application_mailer.rb
> git check-ignore -v -z --stdin
> git check-ignore -v -z --stdin
> git show --textconv :Rails-test/railsTest/app/assets/config/manifest.js
> git ls-files --stage -- E:\Ruby\Rails-test\railsTest\app\assets\config\manifest.js
> git check-ignore -v -z --stdin
> git show --textconv :Rails-test/railsTest/app/assets/images/.keep
> git ls-files --stage -- E:\Ruby\Rails-test\railsTest\app\assets\images\.keep
> git check-ignore -v -z --stdin
> git show --textconv :Rails-test/railsTest/app/assets/stylesheets/application.css
> git ls-files --stage -- E:\Ruby\Rails-test\railsTest\app\assets\stylesheets\application.css
> git show --textconv :Rails-test/railsTest/.gitignore
> git ls-files --stage -- E:\Ruby\Rails-test\railsTest\.gitignore
> git show --textconv :Rails-test/railsTest/Gemfile.lock
> git ls-files --stage -- E:\Ruby\Rails-test\railsTest\Gemfile.lock
> git check-ignore -v -z --stdin
> git check-ignore -v -z --stdin
> git check-ignore -v -z --stdin
> git check-ignore -v -z --stdin
> git check-ignore -v -z --stdin
> git check-ignore -v -z --stdin
> git log --format=%H%n%aN%n%aE%n%at%n%ct%n%P%n%B -z -n21 -- e:\Ruby\Rails-test\railsTest\tmp\cache\bootsnap\compile-cache\00\1d811dfddae2f5
> git show --textconv :Rails-test/railsTest/README.md
> git ls-files --stage -- E:\Ruby\Rails-test\railsTest\README.md
> git status -z -u
> git symbolic-ref --short HEAD
> git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track) refs/heads/main refs/remotes/main
> git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname)
> git remote --verbose
> git config --get commit.template
> git add -A -- .
error: 'Rails-test/railsTest/' does not have a commit checked out
fatal: adding files failed
> git status -z -u
> git ls-files --stage -- E:\Ruby\Rails-test\railsTest\README.md
> git symbolic-ref --short HEAD
> git show --textconv :Rails-test/railsTest/README.md
> git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track) refs/heads/main refs/remotes/main
> git for-each-ref --sort -committerdate --format %(refname) %(objectname) %(*objectname)
> git remote --verbose
> git config --get commit.template