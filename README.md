### jedgement_system :bomb:
## Руководство пользователя для установки и запуска PC^2
Следуйте этим шагам, чтобы установить и настроить PC^2 на вашем компьютере:
## Шаг 1: Установка Java
Для начала установите Java с помощью следующих команд:
```diff
+sudo apt update
+sudo apt install default-jre
+sudo apt install default-jdk
```
## Шаг 2: Распаковка PC^2
Распакуйте архив PC^2 из папки "pc2" и переместите файл "pc2v9.ini" в вашу домашнюю директорию "/home/ваш_пользователь/".
Откройте файл `~/.bashrc` в любом текстовом редакторе, например, `nano`.
В конце файла `~/.bashrc` добавьте следующие переменные среды:
```diff
export JAVAHOME=Путь_до_openjdk-amd64/ (указывая путь до OpenJDK)
export PC2HOME=Путь_до_PC^2 (указывая путь до распакованной папки PC^2)
export PATH="$PC2HOME/bin:$PATH:$JAVAHOME/bin" (добавьте эти пути к переменной $PATH)
```
Пример:
![Screenshot](https://github.com/gehat/jedgement_system/master/image/1.png)
