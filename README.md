# GitGBDZ
* DZ1
1. Выберите какой-нибудь проект на изучаемом вами языке программирования, с которым вы будете тренироваться работать в Git, и инициализируйте в папке этого проекта локальный репозиторий.
   ![Задание](scrin/1.png)
2. Создайте непустой удалённый репозиторий (например, с файлом README.md) с именем, соответствующим имени этого проекта.
   ![Задание](scrin/2.png)
3. Подключите свой проект к этому удалённому репозиторию и отправьте в него код этого проекта. Самостоятельно разрешите конфликты и проблемы, если они возникнут при выполнении данного задания
   ![Задание](scrin/3.png)
    команды:
   - git fetch
   - git merge origin/main --allow-unrelated-histories
   - git push --set-upstream origin main

* DZ2 Работа с изменениями


1. Просмотрите историю коммитов в своём проекте и выберите три случайных коммита. Просмотрите изменения, которые были в них сделаны.

команда: git log --oneline.

   ![Задание](scrin/4.png)

команда: git diff <хэш коммита> позволяет посмотреть какие изменения были сделаны
2. Верните эти изменения командой git revert последовательно, чтобы в итоге получилось тоже три коммита.
   ![Задание](scrin/5.png)
3. Попробуйте отменить эти три коммита:
* последний — командами git reset --soft и git restore;
  Данная команда нас вернула на шаг назад, пришлось удалять изменения командой git restore .src/Hello.java
  ![Задание](scrin/6.png)
* предпоследний — командой git reset --mixed и git restore;

  Результат был такой же как и git reset –soft, , пришлось удалять изменения командой git restore
* первый — командой git reset --hard.
  
  Вернуло нас на изначальное состояния до revert. Использовать git restore не нужно было.
  
* ![Задание](scrin/7.png)

