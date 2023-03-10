[< к содержанию](/readme.md)

## ***Ветвление в GIT***

**Ветвление** - функционал, позволяющий создавать различные версии репозиториев, отличные друг от друга. С помощью ветвления можно вести процесс разработки какого-либо функционала отдельно от основного проекта.


Рассмотрим ветвление на примере следующей ветки:
![](./Branch.png)

Ветка "Main" является основной, от которой отходит новая ветка "Feature", по которой ведется какая-либо работа. В последствии ветку "Feature" мы можем объединить с основной веткой для получения единого продукта на ветке "Main"
![](./Branch1.png)

По данному принципу работают все виды ветвления, но они различаются по методологиям, разберем основные:
- Central Workflow - репозиторий содержит только одну главную ветку "master", все изменения коммитятся в нее.
- Developer Branch Workflow - у каждого разработчика имеются свои отдельные ветки, в которых он вносит изменения. Работа на разных ветках в последствии сливается в одну главную.
- Feature Branch Workflow - репозиторий имеет второстепенную основную ветку (dev), в которой содержится стабильный код для отправки пользователям. Функциональные ветки (фичи) начинают свой код именно от этой ветки и в последствии сливаются с ней.
- Issue Branch Workflow - похожа на предыдущий метод, но ветки создаются по задачам, поставленным перед разработчиками
- Forking Workflow - разработка ведется в полностью скопированном с оригинала репозитории и в последствии изменения переносятся в оригинал
- Github flow - несложная методология, с рядом правил
1. Код в "master" ветке должен быть работоспособным и готовым к развертыванию
2. Все изменения выполняются в отдельных ветках, созданных от "master"
3. Завершенные изменения проверяются руководителем команды и дополнительным специалистом
4. После проверки изменения его вливают в проект и разворачивают на сервере