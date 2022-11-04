# LR6
Лабораторная работа №6
# Лабораторная работа №6
*Сначала нужно создать копию [репозитория](https://github.com/Kurtyanik/LR6/) в личное хранилище.*

![image](https://github.com/4018KChepurnovaSS/LR6/blob/master/screens/1%20%D1%81%D0%BA%D1%80%D0%B8%D0%BD%202%20%D0%BB%D0%B0%D0%B1%D0%B0.png)

*Затем нужно настроить клиент git, для этого вводим имя пользователя и email. Комманды: `git config --global user.name <username>`; `git config --global user.email <email>`.*

![image](https://github.com/4018KChepurnovaSS/LR6/blob/master/screens/%D0%BD%D0%B0%D1%81%D1%82%D1%80%D0%BE%D0%B9%D0%BA%D0%B0%20%D0%BA%D0%BB%D0%B8%D0%B5%D0%BD%D1%82%D0%B0%20git.png)

*Теперь клонируем удалённый репозиторий на компьютер. Комманда: `git clone <url>`.*

![image](https://github.com/4018KChepurnovaSS/LR6/blob/master/screens/%D0%BA%D0%BB%D0%BE%D0%BD%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5%20%D1%83%D0%B4%D0%B0%D0%BB%D0%B5%D0%BD%D0%BD%D0%BE%D0%B3%D0%BE%20%D1%80%D0%B5%D0%BF%D0%BE%D0%B7%D0%B8%D1%82%D0%BE%D1%80%D0%B8%D1%8F.png)

*Переходим в директорию. Комманда: `cd LR6/`.*

![image](https://github.com/4018KChepurnovaSS/LR6/blob/master/screens/%D0%BF%D0%B5%D1%80%D0%B5%D1%85%D0%BE%D0%B4%20%D0%B2%20%D0%B4%D0%B8%D1%80%D0%B5%D0%BA%D1%82%D0%BE%D1%80%D0%B8%D1%8E%20cd.png)

*Поддтягиваем изменения в локальный репозиторий. Комманда: `git pull`.*

![image](https://github.com/4018KChepurnovaSS/LR6/blob/master/screens/pull.png)

*Посмотрим коммиты ветки master. Комманда: `git log`.*

![image](https://github.com/4018KChepurnovaSS/LR6/blob/master/screens/git%20log.png)

*Просмотрим существующие ветки в текущем репозитории, затем перейдем в ветку branch1. Комманды: `git branch`; `git checkout branch1`.*

![image](https://github.com/4018KChepurnovaSS/LR6/blob/master/screens/git%20Branch.png)

*Посмотрим коммиты ветки branch1. Комманда: `git log`.*

![image](https://github.com/4018KChepurnovaSS/LR6/blob/master/screens/Branch%20git%20log.png)

*Подробно рассмотрим коммиты. Комманда: `git log -p`.*

![image](https://github.com/4018KChepurnovaSS/LR6/blob/master/screens/log%20-p.png)

*Выполняем слияние в ветку master. Комманда: `git merge branch1`.*

*Разрешаем возникший конфликт: в теории конфликт возник из-за того, что файл mergefile.txt не отслеживается. Проверив это и убедившись, добавляем файл для отслеживания, оставляем коммит. Команды:`git status`; `git add mergefile.txt`; `git commit -m "Branches"`.*

![image](https://github.com/4018KChepurnovaSS/LR6/blob/master/screens/2021-11-18%20(11).png)

![image](https://github.com/4018KChepurnovaSS/LR6/blob/master/screens/2021-11-18%20(12).png)

*Удаляем побочную ветку после успешного слияния. Комманда: `git branch -d branch1`*

![image](https://github.com/4018KChepurnovaSS/LR6/blob/master/screens/2021-11-18%20(13).png)

*Создаем изменения и фиксируем их, оставляя комментарии,несколько раз. Команды:`echo hello > change1.txt/change2.txt`; `git add change1.txt/change2.txt`; `ggit commit -m "Change1.txt/Change2.txt"`*

![image](https://github.com/4018KChepurnovaSS/LR6/blob/master/screens/2021-11-18%20(16).png)
![image](https://github.com/4018KChepurnovaSS/LR6/blob/master/screens/2021-11-18%20(15).png)

*Просмотр комментариев.*

![image](https://github.com/4018KChepurnovaSS/LR6/blob/master/screens/2021-11-18%20(17).png)
![image](https://github.com/4018KChepurnovaSS/LR6/blob/master/screens/2021-11-18%20(18).png)

*Делаем «хард» откат коммита. Комманда: `git reset --hard HEAD~1`* 
*И создаем ветку для отчёта. Комманда: `git branch report`*

![image](https://github.com/4018KChepurnovaSS/LR6/blob/master/screens/report.jpg)

Оформляем отчёт в файле README.md 

*Получаем итоговую историю операций.  Комманда: `git log`*

![image](https://github.com/4018KChepurnovaSS/LR6/blob/master/screens/report_log1.png)
![image](https://github.com/4018KChepurnovaSS/LR6/blob/master/screens/report_log2.png)

После редактирования отчета, его нужно будет сохранить и произвести команды `git add` и `git commit`.

В конце работы необходимо будет отправить все локальные изменения в сетевое хранилище GitHub командой `git push`.