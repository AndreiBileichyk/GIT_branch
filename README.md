GitHub. HW_2
1. На локальном репозитории сделать ветки для:
- Postman
- Jmeter
- CheckLists
- Bag Reports
- SQL
- Charles
- Mobile testing

Заходим в локальный репозиторий , где надо создать ветки :

git branch Postman

git branch Jmeter

git branch CheckLists

git branch BagReports

git branch SQL

git branch Charles

git branch Mobile_testing

2. Запушить все ветки на внешний репозиторий

git push -u origin Postman 

git push -u origin Jmeter

git push -u origin CheckLists

git push -u origin BagReports

git push -u origin SQL

git push -u origin Charles

git push -u origin Mobile_testing

3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта

git checkout BagReports

cat>> bag.txt

Summary: Что? Где? При каких условиях?

Description: STR, result, expected result

Priority": Low

Environment: windows 10, google chrom ver..

Attachment: scrin

cntr+c

4. Запушить структуру багрепорта на внешний репозиторий

git add . 

git commit -m "add bag.txt"

git push

5. Вмержить ветку Bag Reports в Main

git checkout main

git merge BagReports -m "merge bagreports"

6. Запушить main на внешний репозиторий.

git push

7. В ветке CheckLists набросать структуру чек листа.

git checkout CheckLists

cat>> checklist.txt

Type : possitiv

Title / Summary: Проверить возможность загрузки специальной соли

Expected result : Отсек для загрузки соли открывается, заполнен водой, соль засыпается и отсек с засыпанной солью закрывается

Status : passed

cntr +c

8. Запушить структуру на внешний репозиторий

git add . 

git commit -m "add checklist.txt"

git push

9. На внешнем репозитории сделать Pull Request ветки CheckLists в main

Находясь в ветке checklist нажимаем Pull requests

Compare pull request

Create pull request

Merge pull request

Confirm merge

10. Синхронизировать Внешнюю и Локальную ветки Main 

В гит баш находясь в main : 

git fetch

git pull
