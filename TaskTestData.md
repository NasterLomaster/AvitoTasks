# Тестовое задание №1 для Avito

```postgresql
select distinct inf.issue_key as "Номер задачи", inf."name" as "Название задачи" 
from task_info inf 
join task_status st on inf.issue_key=st.issue_key
where inf."type"='Bug' and st.status='in progress' and st.start_time >= '2021-04-01' and st.start_time < '2021-05-01'
```




 # Тестовое задание №2 для Avito



Класс | Значения баллов | % скидки | Позитивные проверки
------|-----------------| ---------|------
1     | от 0 до 100     |   1%     | 1; 50; 99
2     | от 100 до 200   |   3%     | 100; 101; 150; 199
3     | от 200 до 500   |   4%     | 200; 201; 300; 499
4     | от 500          |   5%     | 500; 501; 550