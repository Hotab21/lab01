## Laboratory work I

Данная лабораторная работа посвещена изучению утилит для разработки проектов

## Tasks

- [x] 1. Ознакомиться со ссылками учебного материала
- [x] 2. Выполнить инструкцию учебного материала
- [x] 3. Составить отчет и отправить ссылку личным сообщением в **Slack**

## Tutorial

```bash
$ export GITHUB_USERNAME=Hotab21# Создание переменной
$ export GIST_TOKEN=<сохраненный_токен> # Создание переменной
$ alias edit=<nano|vi|vim|subl> # Создание синонима
```

```ShellSession
$ mkdir -p ${GITHUB_USERNAME}/workspace #Создание папки /Hotab21/workspace
$ cd ${GITHUB_USERNAME}/workspace #Переход в папку /Hotab21/workspace
$ pwd # Вывод текущей директории
$ cd .. #Переход в домашнюю директорию ~$
$ pwd # Вывод текущей директории
```

```ShellSession
$ mkdir -p workspace/tasks/ #Создание папки /tasks/
$ mkdir -p workspace/projects/ #Создание папки /projects/
$ mkdir -p workspace/reports/ #Создание папки /reports/ 
$ cd workspace #Переход в папку /Hotab21/workspace
```

```ShellSession
# Debian
$ wget https://nodejs.org/dist/v6.11.5/node-v6.11.5-linux-x64.tar.xz #Скачивание архива
$ tar -xf node-v6.11.5-linux-x64.tar.xz #Распаковка архива
$ rm -rf node-v6.11.5-linux-x64.tar.xz #Удаление архива
$ mv node-v6.11.5-linux-x64 node #Переименование 
```

```ShellSession
$ ls node/bin #Вывод содержимого
$ echo ${PATH} # Вывод переменной
$ export PATH=${PATH}:`pwd`/node/bin # Дописать в PATH папку с node js
$ echo ${PATH} # Вывод переменной
$ mkdir scripts #Создание папки /scripts/
$ cat > scripts/activate<<EOF #Запись указанной строки в файл /FalaleevDanila/workspace/scripts/activate
export PATH=\${PATH}:`pwd`/node/bin
EOF
$ source scripts/activate # Выполнить указанный скрипт
```

```ShellSession
$ npm install -g gistup # Установка пакета gistup в node js
$ ls node/bin # Вывод директорий и файлов
```

```ShellSession
$ cat > ~/.gistup.json <<EOF #Запись указанной строки в файл
{
  "token": "${GIST_TOKEN}"
}
EOF
```

## Report

```ShellSession
$ export LAB_NUMBER=01
$ git clone https://github.com/tp-labs/lab${LAB_NUMBER} tasks/lab${LAB_NUMBER}
$ mkdir reports/lab${LAB_NUMBER}
$ cp tasks/lab${LAB_NUMBER}/README.md reports/lab${LAB_NUMBER}/REPORT.md
$ cd reports/lab${LAB_NUMBER}
$ edit REPORT.md
$ gistup -m "lab${LAB_NUMBER}" # enter: yes↵
```

## Links

### Unix commands

- [ar](https://en.wikipedia.org/wiki/Ar_(Unix))
- [cat](https://en.wikipedia.org/wiki/Cat_(Unix))
- [cd](https://en.wikipedia.org/wiki/Cd_(command))
- [cp](https://en.wikipedia.org/wiki/Cp_(Unix))
- [cut](https://en.wikipedia.org/wiki/Cut_(Unix))
- [echo](https://en.wikipedia.org/wiki/Echo_(command))
- [env](https://en.wikipedia.org/wiki/Env_(shell))
- [ex](https://en.wikipedia.org/wiki/Ex_(editor))
- [file](https://en.wikipedia.org/wiki/File_(command))
- [find](https://en.wikipedia.org/wiki/Find)
- [ls](https://en.wikipedia.org/wiki/Ls)
- [man](https://en.wikipedia.org/wiki/Man_page)
- [mkdir](https://en.wikipedia.org/wiki/Mkdir)
- [mv](https://en.wikipedia.org/wiki/Mv)
- [nm](https://en.wikipedia.org/wiki/Nm_(Unix))
- [ps](https://en.wikipedia.org/wiki/Ps_(Unix))
- [pwd](https://en.wikipedia.org/wiki/Pwd)
- [rm](https://en.wikipedia.org/wiki/Rm_(Unix))
- [sed](https://en.wikipedia.org/wiki/Sed)
- [touch](https://en.wikipedia.org/wiki/Touch_(Unix))

### Package Managers

- [apt](http://help.ubuntu.ru/wiki/apt) | [dnf](https://en.wikipedia.org/wiki/DNF_(software)) | [yum](https://fedoraproject.org/wiki/Yum/ru)
- [brew](https://brew.sh) | [linuxbrew](http://linuxbrew.sh)
- [npm](https://docs.npmjs.com)

### Software

- [curl](https://www.gitbook.com/book/bagder/everything-curl/details)
- [wget](https://www.gnu.org/software/wget/manual/wget.pdf)
- [clang](https://clang.llvm.org)
- [g++](https://gcc.gnu.org/onlinedocs/gcc-4.0.2/gcc/G_002b_002b-and-GCC.html)
- [make](https://en.wikipedia.org/wiki/Make_(software))
- [open](https://developer.apple.com/legacy/library/documentation/Darwin/Reference/ManPages/man1/open.1.html)
- [openssl](https://www.openssl.org)
- [nano](https://www.nano-editor.org)
- [tree](https://linux.die.net/man/1/tree)
- [vim](http://www.vim.org)

```
Copyright (c) 2015-2019 The ISC Authors
```
