# Домашнее задание к занятию "ELK" - `Bazylev Artem`


### Инструкция по выполнению домашнего задания

   1. Сделайте `fork` данного репозитория к себе в Github и переименуйте его по названию или номеру занятия, например, https://github.com/имя-вашего-репозитория/git-hw или  https://github.com/имя-вашего-репозитория/7-1-ansible-hw).
   2. Выполните клонирование данного репозитория к себе на ПК с помощью команды `git clone`.
   3. Выполните домашнее задание и заполните у себя локально этот файл README.md:
      - впишите вверху название занятия и вашу фамилию и имя
      - в каждом задании добавьте решение в требуемом виде (текст/код/скриншоты/ссылка)
      - для корректного добавления скриншотов воспользуйтесь [инструкцией "Как вставить скриншот в шаблон с решением](https://github.com/netology-code/sys-pattern-homework/blob/main/screen-instruction.md)
      - при оформлении используйте возможности языка разметки md (коротко об этом можно посмотреть в [инструкции  по MarkDown](https://github.com/netology-code/sys-pattern-homework/blob/main/md-instruction.md))
   4. После завершения работы над домашним заданием сделайте коммит (`git commit -m "comment"`) и отправьте его на Github (`git push origin`);
   5. Для проверки домашнего задания преподавателем в личном кабинете прикрепите и отправьте ссылку на решение в виде md-файла в вашем Github.
   6. Любые вопросы по выполнению заданий спрашивайте в чате учебной группы и/или в разделе “Вопросы по заданию” в личном кабинете.
   
Желаем успехов в выполнении домашнего задания!
   
### Дополнительные материалы, которые могут быть полезны для выполнения задания

1. [Руководство по оформлению Markdown файлов](https://gist.github.com/Jekins/2bf2d0638163f1294637#Code)

---

### Задание 1
Таблица "Сотрудники" (Employees):

    Данные, которые хранятся в этой таблице, включают информацию о сотрудниках, такую как их фамилии, оклады, должности, тип подразделения и связь с структурным подразделением.
    Типы данных для столбцов в PostgreSQL:
        Идентификатор (integer)
        ФИО (varchar(50))
        Оклад (numeric)
        Должность (varchar)
        Тип подразделения (varchar)
        Идентификатор структурного подразделения (integer, внешний ключ)

Таблица "Структурные подразделения" (Departments):

    В этой таблице хранится информация о структурных подразделениях, включая их названия и адреса филиалов.
    Типы данных для столбцов в PostgreSQL:
        Идентификатор (integer)
        Название (varchar)
        Адрес филиала (varchar)

Таблица "Проекты сотрудников" (EmployeeProjects):

    В данной таблице хранятся данные о проектах, которыми занимаются сотрудники, и их связь с соответствующими сотрудниками.
    Типы данных для столбцов в PostgreSQL:
        Идентификатор (integer)
        Идентификатор сотрудника (integer, внешний ключ)
        Название проекта (varchar)

Таблица "Даты найма сотрудников" (EmployeeHireDates):

    В этой таблице хранятся даты найма сотрудников и их связь с соответствующими сотрудниками.
    Типы данных для столбцов в PostgreSQL:
        Идентификатор (integer)
        Идентификатор сотрудника (integer, внешний ключ)
        Дата найма (date)

Таблица "Филиалы" (Branches):

    В этой таблице хранится информация о филиалах компании.
    Типы данных для столбцов в PostgreSQL:
        Идентификатор (integer)
        Название филиала (varchar)

Таблица "Должности" (JobTitles):

    В данной таблице хранится список должностей сотрудников.
    Типы данных для столбцов в PostgreSQL:
        Идентификатор (integer)
        Название должности (varchar)

Таблица "Типы подразделений" (DepartmentTypes):

    В этой таблице хранятся типы подразделений.
    Типы данных для столбцов в PostgreSQL:
        Идентификатор (integer)
        Название типа подразделения (varchar)


