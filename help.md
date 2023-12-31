[<к содержанию](./readme.md)

## Как получить помощь?


Если вам нужна помощь при использовании GIT, есть три способа открыть страницу руководства по любой команде GIT:

```
$ git help <команда>
$ git <команда> --help
$ man git-<команда> 
```

Например, так можно открыть руководство по команде `git config`

``` 
$ git help config 
```

Эти команды хороши тем, что ими можно пользоваться всегда, даже без подключения к сети. 

Eсли вам нужно посмотреть только список опций и вы не хотите читать полную документацию по команде, вы можете использовать опцию ***-h*** для вывода краткой инструкции по использованию:

```
$ git add -h
usage: git add [<options>] [--] <pathspec>...

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
 ```

 [![Prev](/assets/prev3.png)](install.md "Предыдущий раздел")[![Next](/assets/next3.png)](config.md "Следующий раздел")