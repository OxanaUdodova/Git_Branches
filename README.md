# Project
1. На локальном репозитории сделать ветки для:
- Postman  		git branch Postman
- Jmeter 		git branch Jmeter
- CheckLists		git branch CheckLists
- Bag Reports		git branch Bag_Reports
- SQL	 		git branch SQL
- Charles 		git branch Charles
- Mobile testing 	git branch Mobile_testing

2. Запушить все ветки на внешний репозиторий
git push --all

или git push -u origin Postman Jmeter ..и т.д

3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта

git checkout Bag_Reports
nano bag_report.txt
Bug report structure:
        Bug_ID
        Title
        Severety
        Priority
        Enviroment
        Precondition
        Step to reproduce
        Actual result
        Expected result

4. Запушить структуру багрепорта на внешний репозиторий
git add bag_report.txt >> git commit -m "add bag_report.txt" >> git push origin Bag_Reports

5. Вмержить ветку Bag Reports в Main
git checkout main >> git merge Bag_Reports

6. Запушить main на внешний репозиторий.
 git push

7. В ветке CheckLists набросать структуру чек листа.
 git checkout CheckLists
nano check_list.txt
№
Criteria
Status

8. Запушить структуру на внешний репозиторий
git add .>> git commit -m "add check_list.txt" >> git push origin CheckLists

9. На внешнем репозитории сделать Pull Request ветки CheckLists в main
На GitHub перейти в ветку CheckLists >> Compare & pull request >> Сreate pull request >> Merge pull request >> Confirm merge

10. Синхронизировать Внешнюю и Локальную ветки Main
git checkout main >> git pull
