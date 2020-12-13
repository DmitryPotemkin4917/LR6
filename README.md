# LR6

Лабораторная работа №6

**Цель лабораторной работы:** изучение базовых возможностей системы управления версиями, опыт работы с Git Api, опыт работы с локальным и удаленным репозиторием.

**Порядок выполнения работы:**

Создадим аккаунт на github

Сделаем копию в личное хранилище из https://github.com/Kurtyanik/LR6/

![1](D:\Git\LR6\screenshots\1.png)

установим git

![2](D:\Git\LR6\screenshots\2.png)

настроим клиент git, введя имя пользователя (Группа Фамилия И.О.) и email. 

![3](D:\Git\LR6\screenshots\3.png)

Команды:

```
git config --global user.name "4917 Potemkin D.V."
git config --global user.email 'dmitry.potemkin@gmail.com'
```

Клонируем удалённый репозиторий на компьютер, после чего сделаем коммит:

![4](D:\Git\LR6\screenshots\4.png)

Команды:

```
git clone https://github.com/DmitryPotemkin4917/LR6
git add LR6
git commit -m "комментарий"
```

Добавим файл через интерфейс github:

![5](D:\Git\LR6\screenshots\5.png)



![6](D:\Git\LR6\screenshots\6.png)

Подтянем изменения в локальный репозиторий:

![7](D:\Git\LR6\screenshots\7.png)

Команды:

```
git pull
```

сделаем коммит

![8](D:\Git\LR6\screenshots\8.png)

Получим историю операций:

![9](D:\Git\LR6\screenshots\9.png)

Команды:

```
git log
```

Создадим новую ветку, в которой создадим текстовый файл и закоммитим его:

![10](D:\Git\LR6\screenshots\10.png)

![11](D:\Git\LR6\screenshots\11.png)

Команды:

```
git checkout -b название_ветки
nano название_файла
git add имя_файла
git commit -m "комментарий"
```

Произведём слияние:

![12](D:\Git\LR6\screenshots\12.png)

Код:

```
git checkout Ветка_в_которую_нужно_перейти
git merge Ветка_с_которой_нужно_произвести_слияние
```

