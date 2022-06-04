# Git_HW_2
1. На локальном репозитории сделать ветки для:
- Postman

git branch Postman

- Jmeter

git branch Jmeter

- CheckLists

git branch CheckLists

- Bag Reports

git branch Bug_Reports

- SQL

git branch SQL

- Charles

git branch Charles

- Mobile testing

git branch Mobile_testing

2. Запушить все ветки на внешний репозиторий

git push origin --all

3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта

git checkout Bug_Reports
cat > Bug_Reports.txt
Environment:
ID:
Summary:
Steps to reproduce:
Actual Result:
Expected Result:
Attachments:

Ctr C

4. Запушить структуру багрепорта на внешний репозиторий

git add Bug_Reports.txt
git commit -m "add file bug_reports"
git push --set-upstream origin Bag_reports

5. Вмержить ветку Bag Reports в Main

git checkout main
git merge Bug_Reports

6. Запушить main на внешний репозиторий.

 git push

7. В ветке CheckLists набросать структуру чек листа.

git checkout CheckLists
cat > CheckLists.txt
ID:
Check:
Result:
Comment:

Ctr C

8. Запушить структуру на внешний репозиторий

git add .
git commit -m "add file checklis"
git push - u origin CheckLists

9. На внешнем репозитории сделать Pull Request ветки CheckLists в main

Compare & pull request
Create pull request
Merge pull request
Confirm merge

10. Синхронизировать Внешнюю и Локальную ветки Main

git checkout main
git fetch
git pull
