# LR6

Лабораторная работа №6                                                                                  Потемкин Дмитрий (4917)

**Цель лабораторной работы:** изучение базовых возможностей системы управления версиями, опыт работы с Git Api, опыт работы с локальным и удаленным репозиторием.

**Порядок выполнения работы:**

Создадим аккаунт на github:

Сделаем копию в личное хранилище из https://github.com/Kurtyanik/LR6/

![1](https://github.com/DmitryPotemkin4917/LR6/blob/ReportBranch/screenshots/1.png)

установим git

![2](https://github.com/DmitryPotemkin4917/LR6/blob/ReportBranch/screenshots/2.png)

настроим клиент git, введя имя пользователя (Группа Фамилия И.О.) и email. 

![3](https://github.com/DmitryPotemkin4917/LR6/blob/ReportBranch/screenshots/3.png)

Команды:

```
git config --global user.name "4917 Potemkin D.V."
git config --global user.email 'dmitry.potemkin@gmail.com'
```

Клонируем удалённый репозиторий на компьютер, после чего сделаем коммит:

![4](https://github.com/DmitryPotemkin4917/LR6/blob/ReportBranch/screenshots/4.png)

Команды:

```
git clone https://github.com/DmitryPotemkin4917/LR6
git add LR6
git commit -m "комментарий"
```

Добавим файл через интерфейс github:

![5](https://github.com/DmitryPotemkin4917/LR6/blob/ReportBranch/screenshots/5.png)



![6](https://github.com/DmitryPotemkin4917/LR6/blob/ReportBranch/screenshots/6.png)

Подтянем изменения в локальный репозиторий:

![7](https://github.com/DmitryPotemkin4917/LR6/blob/ReportBranch/screenshots/7.png)

Команды:

```
git pull
```

сделаем коммит

![8](https://github.com/DmitryPotemkin4917/LR6/blob/ReportBranch/screenshots/8.png)

Получим историю операций:

![9](https://github.com/DmitryPotemkin4917/LR6/blob/ReportBranch/screenshots/9.png)

Команды:

```
git log
```

Создадим новую ветку, в которой создадим текстовый файл и закоммитим его:

![10](https://github.com/DmitryPotemkin4917/LR6/blob/ReportBranch/screenshots/10.png)

![11](https://github.com/DmitryPotemkin4917/LR6/blob/ReportBranch/screenshots/11.png)

Команды:

```
git checkout -b название_ветки
nano название_файла
git add имя_файла
git commit -m "комментарий"
```

Произведём слияние:

![12](https://github.com/DmitryPotemkin4917/LR6/blob/ReportBranch/screenshots/12.png)

Команды:

```
git checkout Ветка_в_которую_нужно_перейти
git merge Ветка_с_которой_нужно_произвести_слияние
```

После успешного слияния удалим побочную ветку:

![13](https://github.com/DmitryPotemkin4917/LR6/blob/ReportBranch/screenshots/13.png)

Команды:

```
git branch -d newbranch
```

Сделаем несколько изменений и зафиксируем их:

![14](https://github.com/DmitryPotemkin4917/LR6/blob/ReportBranch/screenshots/14.png)

Сделаем "Хард" откат коммита

![15](https://github.com/DmitryPotemkin4917/LR6/blob/ReportBranch/screenshots/15.png)

Команды:

```
git reset --hard хэш
```

Создадим ветку для отчёта:

![16](https://github.com/DmitryPotemkin4917/LR6/blob/ReportBranch/screenshots/16.png)

Команды: 

```
git checkout -b ReportBranch
```

Получим историю операций в форматированном виде (сокращённый хэш + сокращённая дата + имя автора + комментарий), разделим данные символом “|”. 

Для ветки ReportBranch:

![17](https://github.com/DmitryPotemkin4917/LR6/blob/ReportBranch/screenshots/17.png)

Для ветки master:

![18](https://github.com/DmitryPotemkin4917/LR6/blob/ReportBranch/screenshots/18.png)

Команды:

```
git log --pretty=format:"%h | %ad | %an | %s" --date=short
```

**Вывод:** в ходе выполнения лабораторной работы были изучены базовые возможности системы управления версиями, был получен опыт работы с Git Api, а также опыт работы с локальным и удаленным репозиторием.
