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
6) Создать item → Создать задачу со свободной конфигурацией
![создание item](https://github.com/minin2000/spring_hello_world/assets/65463411/8f0b4e0b-f217-4a91-87f0-df145e631b59)

7) → добавить шаги сборки → выполнить команду shell → java -jar /tmp/hello/hello.jar 
![настройки item](https://github.com/minin2000/spring_hello_world/assets/65463411/d62be4e5-6e05-489f-9e4e-545d5a875861)


Результат:  
![консоль](https://github.com/minin2000/spring_hello_world/assets/65463411/35acc63d-2a9f-4622-a026-3ef72226352c)
