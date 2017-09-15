## Laboratory work II

Данная лабораторная работа посвещена изучению утилит для разработки проектов

## Tasks

- [x] 1. Ознакомиться со ссылками учебного материала
- [x] 2. Выполнить инструкцию учебного материала
- [x] 3. Составить отчет и отправить ссылку личным сообщением в **Slack**
 
## Tutorial

```bash
$ export GITHUB_USERNAME=Toshuxanoff 	#создает переменную окружения
$ export GIST_TOKEN=****************************************
$ alias edit=vim 			#переопределение команды
```

```bash
$ npm install -g gistup 	#работа с пакетным менежджером
```

```bash
$ cat > ~/.gistup.json <<EOF 	#просмотр файла
{
  "token": "${GIST_TOKEN}"
}
EOF
```

```bash
$ cd ~ 					#переход в заданную директорию
$ mkdir -p workspace/labs/projects/ 	#создание новой директории
$ mkdir -p workspace/labs/tasks/
$ mkdir -p workspace/labs/reports/
```

## Report

```bash
$ cd ~/workspace/labs/
$ export LAB_NUMBER=02
$ git clone https://github.com/tp-labs/lab${LAB_NUMBER} tasks/lab${LAB_NUMBER}
$ mkdir reports/lab${LAB_NUMBER}
$ cp tasks/lab${LAB_NUMBER}/README.md reports/lab${LAB_NUMBER}/REPORT.md 	#копирование
$ cd reports/lab${LAB_NUMBER}
$ edit REPORT.md 								#редактирование в vim
$ gistup -m "lab${LAB_NUMBER}"
```

