# GitHub.HW_2

1. На локальном репозитории сделать ветки (Postman, Jmeter, CheckLists, Bug Reports, SQL, Charles, Mobile testing)
``` git checkout -b Postman
 git checkout -b Jmeter
 git checkout -b CheckLists
 git checkout -b Bug_Reports
 git checkout -b SQL
 git checkout -b Charles
 git checkout -b Mobile_testing
```

2.  Запушить все ветки на внешний репозиторий
 ```git push --set-upstream origin Postman
 git push --set-upstream origin Jmeter
 git push --set-upstream origin CheckLists
 git push --set-upstream origin Bug_Reports
 git push --set-upstream origin SQL
 git push --set-upstream origin Charles
 git push --set-upstream origin Mobile_testing
 ```

3. В ветке Bug Reports сделать текстовый документ со структурой баг репорта
```
git checkout Bug_Reports
touch bugreport.txt

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
```

4. Запушить структуру багрепорта на внешний репозиторий
```
 git add bugreport.txt
 git commit -m "fill data in bugreport"
 git push
 ```

5. Вмержить ветку Bug Reports в Main
```
 git checkout main
 git merge Bug_Reports
 ```

6. Запушить main на внешний репозиторий.
```
git push
```
7. В ветке CheckLists набросать структуру чек листа.
```
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
 ```
8. Запушить структуру на внешний репозиторий
```
 git add checklist.txt
 git commit -m "adding data"
 git push
 ```
9. На внешнем репозитории сделать Pull Request ветки CheckLists в main
10. Синхронизировать Внешнюю и Локальную ветки Main 
```
 git fetch
 git pull
 ```
