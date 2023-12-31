[<к содержанию](./readme.md)

# git clean

Команда `git clean` используется для удаления мусора из рабочего каталога. Это могут быть результаты сборки проекта или файлы конфликтов слияний.

`git clean -f -d`   -  удаление всех неодслеживаемых файлов  и каталогов в вашем рабочем каталоге.

Любой файл, который соответствует шаблону в вашем ^.gitignore*, или другие игнорируемые файлы не будут удалены.

Опция ***-x***  позволяет полностью очистить сборку.

Если вы хотите только посмотреть, что будет сделано, вы можете запустить команду с опцией ***-n***, которая означает «имитируй работу команды и скажи мне, что ты будешь удалять».

```
$ git clean -d -n
Would remove test.o
Would remove tmp/
```
Другой способ, который позволяет вам более тщательно контролировать сам процесс — это выполнение команды с опцией ***-i*** (в «интерактивном» режиме). Вы можете просмотреть каждый файл индивидуально или указать шаблоны для удаления в интерактивном режиме.

### **Примечание**
Если вы оказались в рабочем каталоге, в который вы скопировали или клонировали другие репозитории GIT (возможно, в виде подмодулей), даже `git clean -fd` откажется удалить эти каталоги. В таких случаях вам нужно добавить второй параметр ***-f*** для акцентирования.



[![Prev](/assets/prev3.png)](git_add.md "Предыдущий раздел")[![Next](/assets/next3.png)](git_commit.md "Следующий раздел")