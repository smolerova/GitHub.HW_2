# GitHub.HW_2
Creating new branches

1. На локальном репозитории сделать ветки
- Postman  git checkout -b Postman
- Jmeter  git checkout -b Jmeter
- CheckLists  git checkout -b CheckLists
- Bag Reports  git checkout -b Bag_Reports
- SQL  git checkout -b SQL
- Charles git checkout -b Charles
- Mobile testing  git checkout -b Mobile_testing

2.  Запушить все ветки на внешний репозиторий
 git push --set-upstream origin Postman
 git push --set-upstream origin Jmeter
 git push --set-upstream origin CheckLists
 git push --set-upstream origin Bag_Reports
 git push --set-upstream origin SQL
 git push --set-upstream origin Charles
 git push --set-upstream origin Mobile_testing

3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта
git checkout Bag_Reports
touch bagreport.txt

Summary
Project
Component
Version
Severity(Blocker,Critical,Major,Minor,Trivial)
Priority(High,Medium,Low)
Status
Author
Assigned To
Environment
Steps to Reproduce
Actual Result
Expected Result
Attachment
4. Запушить структуру багрепорта на внешний репозиторий
 git add bagreport.txt
 git commit -m "fill data in bagreport"
 git push

5. Вмержить ветку Bag Reports в Main
 git checkout main
 git merge Bag_Reports

6. Запушить main на внешний репозиторий.
git push
7. В ветке CheckLists набросать структуру чек листа.
 git checkout CheckLists
 touch checklist.txt
  
 Test Case ID
 Test Description
 Assumptions and Pre-Conditions
 Module
 Test Data
 Priority
 Test Steps
 Expected Result
 Actual Result
 Pass/Fail
 Tester/Date
 Comments
8. Запушить структуру на внешний репозиторий
 git add checklist.txt
 git commit -m "adding data"
 git push

9. На внешнем репозитории сделать Pull Request ветки CheckLists в main
10. Синхронизировать Внешнюю и Локальную ветки Main 
 git fetch
 git pull