## Шпаргалка по использованию GIT
0. Запушить изменения в мастер: $ git push -u origin master
1. Для создания папки используется команда **mkdir**
2. Для создания файлов используется команда **touch**
3. Для удаления файлов используется команда **rm** 
При этом **rm -r** удаляет всю папку с содержимым
4. Для добавления файлов в очередь для коммита необходимо использовать команду **git add**
5. Для создания коммита используем команду **git commit -m 'сюда добавлем текст коммита'** 
6. Для синхронизации наших коммитов с платформой (в нашем случае GitHub) используем команду **git unit**
7. Для того чтобы изменить последний коммит - команда git commit --amend -m 'текст нового коммита'
Либо если изменения касаются только добавления нового файла используем git commit --amend --no-edit
8. Команда git restore --staged <file> переведёт файл из staged обратно в modified или untracked.
9. Команда git reset --hard <commit hash> «откатит» историю до коммита с хешем <hash>. Более поздние коммиты потеряются!
10. Команда git restore <file> «откатит» изменения в файле до последней сохранённой (в коммите или в staging) версии.
11. Команда git diff дает возможность посмотреть изменения, а git diff --staged - если сделали add
12. Для того чтобы не добавлять ненужные файлы в систему отслеживания версий - создается специальный файл .gitignore
13. Создание ветки происходит командой `git branch %BRANCH_NAME%`
14. Переключение на ветку происходит командой `git checkout %BRANCH_NAME%`
15. Чтобы посмотреть все активные ветки в проекте, нужно вызвать команду `git branch` без аргументов.  
16. Слияние веток происходит командой git merge <название_ветки>
17. После слияния ветку лучше удалить, командой git branch -D <название_ветки>
18. Забрать изменения из удалённого репозитория — git pull
19. git push -u origin my-branch — отправь новую ветку my-branch в удалённый репозиторий и свяжи локальную ветку с удалённой

### Полезности
**&&** - дает возможность выполнять ряд команд сразу
**TAB** - позволяет не дописывать фразы до конца
