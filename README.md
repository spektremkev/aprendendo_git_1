Testendo o quite na pratica untilisando o livro do Linux torvalds 

usage: git config [<options>]

"Git init" começa o repositorio.
"Git status" mostrara os arquivos que não foram traqueados pelo git.
"Git add -A" Ele adicionara as 
"Git commit -m" - "primeiro commit de teste " - Adicionara as alteraçoes dps ao reositorio local
"Git branch" me retornara todos o "branch" na pasta do arquivoem que estamos trabalhado 



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

