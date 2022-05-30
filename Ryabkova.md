# Первый заголовок

*Пишем красиво курсивом*

## Второй заголовок

1. Первый элемент списка
2. Второй элемент списка
3. Третий элемент списка

### Третий заголовок

* Список 1
* Список 2
* список 3

**Пишем жирным шрифтом**
>Добавим цитаты

>>Ты — единственный автор всего, что с тобой происходит

>>>Жизнь - это то, что происходит с вами, пока вы строите другие планы

1. Новый список 1

  > Цитата внутри списка 1

2. Новый список 2  

  > Цитата внутри списка 2

  Элемент сверху

  ---

  Элемент снизу

#### Четвертый заголовок

***Текст жирным курсивом***

* Список в списке
  1. Перый
  2. Второй

* Вторая строка
* Конец списка

~~Зачеркнутый текст~~

**Окончание работы :))**

# Seminar 2

* Создание веток

1. Вначале, когда мы делаем свой первый коммит, Git автоматически создает основную ветку.
2. Для создания новой ветки используется команда *git branch_name*, где *branch_name*-название новой ветки.
3. С помощью команды *git branch* можно  создать неограниченное количество веток и переключаться между ними по мере необходимости.

4. Для перехода используется команда *git checkout branch_name*где *branch_name*-название новой ветки.

5. Обычно если ветка больше не нужна, ее сливают с основной и удаляют.
6. Когда вы работаете с большим количеством веток, можно легко забыть имя нужной, а без имени ветки переключится на нее не получится. Для таких ситуаций существует команда просмотра списка веток - это уже знакомая нам *git branch*, но с другими ключами.
7. По умолчанию *git branch* выводит список локальных веток. С ключами -r, -a можно вывести, соответственно, либо только удаленные ветки, либо все ветки.

* Слияние веток

1. Для осуществления слияния веток используется команда *git marge branch_name*
2. **Мастер** - это основная ветка проекта, в которую заливается только рабочий проверенный код.
3. Когда мы заканчиваем работу над веткой, например, сделали новый функционал, мы сливаем ее в мастер. В мастере код проверяется еще раз и выкладывается на сервер.
4. Сливать друг в друга можно любые ветки. Технически, с точки зрения git нет никакой разницы, сливается ветка с новым функционалом в мастер или наоборот. Для нас **мастер** - это основная ветка разработки, а для git это просто ветка.
5. Слияние ветки в **мастер**
Выполняется после завершения работы над своей веткой при помощи команды *git merge*. Чтобы слить ветку в мастер, нужно сначала перейти в мастер, а затем выполнить *git merge branch_name*.
6. Если мы создали ветку, поработали над ней, собрались заливать ее в **мастер**, а за это время новых коммитов там не появилось, то слияние произойдет без конфликта. Git понимает, что это новый код, который можно просто положить поверх старого. Это простая ситуация и git не задает никаких вопросов.


* Конфликты при слиянии

1. Конфликты при слиянии возникают при возникновении противоречищих коммитов слияния веток.

2. Иногда нам приходится править одни и те же участки кода и тогда при их слиянии git не может понять, чей вариант правильный. Это называется возникновения конфликта.
3. Git помечает файл как конфликтующий и останавливает процесс слияния.В этом случае ответственность за разрешение конфликта несут разработчики.
4. Сбой В ПРОЦЕССЕ слияния говорит о наличии конфликта между текущей локальной веткой и веткой, с которой выполняется слияние. 
5. Git сделает все возможное, чтобы объединить файлы, но оставит конфликтующие участки, чтобы вы разрешили их вручную.
6. Обычно принимают обе версии измененных участков. Самый простой способ разрешить конфликт — отредактировать конфликтующий файл.
7. После редактирования файла нужно выполнить команду*git add*
8.  Для завершения слияния нужно создать  новый коммит.
9. Git обнаружит, что конфликт разрешен, и создаст новый коммит слияния для завершения процедуры слияния.


**Итоги семинара**

1. Научились содавать ветки и переходить с одной ветки на другую.
2. Попробовали слияние веток.
3. Создали и разрешили конфликт при слиянии веток.

















