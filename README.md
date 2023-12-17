# Инструкция  
1) Скачать образ jenkins
```bash
docker pull jenkins/jenkins
```
2) В директории проекта запустить
```bash
docker-compose up -d
```
3) Перейти http://localhost:8080
4) Авторизоваться как администратор (взять пароль из контейнера /var/jenkins_home/secrets/initialAdminPassword)
5) Установить все плагины
6) Создать item → Создать задачу со свободной конфигурацией → добавить шаги сборки → выполнить команду shell → java -jar /tmp/hello/hello.jar
