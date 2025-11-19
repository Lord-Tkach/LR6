# Отчёт по лабораторной работе №6  
## Тема: Работа с системой контроля версий Git  
**Студент:** *Матвеев Н.С.*  
**Группа:** *4414*  

---

## 1. После установки Git, я настроил имя пользователя и email

Использовались команды:

![](git_config.png)
![](git_config_list.png)

## 2. Клонирование удалённого репозитория

Удалённый репозиторий был клонирован командой:

![](git_clone.png)

## 3. Добавление файла через GitHub и получение изменений

Файл был добавлен в интерфейсе GitHub → затем выполнено получение изменений:

![](create_fail.png)
![](git_pull.png)

## 4. История операций

Для просмотра истории использована команда:

![](git_log.png)

## 5. Просмотр последних изменений в файлах

![](git_diff.png)

## 6. Слияние ветки и разрешение конфликта
### 6.1. Добавление строк, попытка слияния

![](new-feature_add.png)
![](add_master.png)
![](conflict_readme.png)

### 6.2. Разрешение конфликта
После корректировки вручную:

![](correct_readme.png)
![](commit_correct.png)

## 7. Удаление побочной ветки

![](delete_branch.png)

## 8. Несколько коммитов подряд

Выполнены изменения и создано несколько коммитов:

![](first_change.png)
![](second_change.png)
![](third_change.png)
![](all_change_readme.png)


## 9. Откат коммита (revert)

![](revert_vim.png)

## 10. Создание ветки для отчёта

![](report_branch.png)

## 11. Коммит отчёта

![](first_commit_report.png)

## 12. Лог команд

git init
git remote add origin ...
git add .
git commit -m "Initial commit"
git checkout -b new-feature
git add README.md
git commit -m "Добавлена строка из ветки new-feature"
git checkout master
git merge new-feature
git add README.md
git commit -m "Merge ветки new-feature в master, конфликт решён"
git branch -d new-feature
git add README.md
git commit -m "Изменение №1"
git add README.md
git commit -m "Изменение №2"
git add README.md
git commit -m "Изменение №3"
git revert <hash>
git add README.md
git revert --continue
git push origin master

## 13. История операций в форматированном виде

![](history_operation.png)
