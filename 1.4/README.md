## Домашнее задание к занятию «Сетевое взаимодействие в K8S. Часть 1»

# Задание 1
- Создал Deployment приложения, состоящего из двух контейнеров — nginx и multitool с количеством реплик 3 шт
[Ссылка на yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/1.4/z1/deployment.yaml)

- Создал Service, который обеспечит доступ внутри кластера до контейнеров приложения из п.1 по порту 9001 — nginx 80, по 9002 — multitool 8080
[Ссылка на yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/1.4/z1/service-z1.yaml)

- Демонстрация доступа с помощью curl по доменному имени сервиса

![image](https://github.com/bogkofe/Kubernetes/blob/master/1.4/files/1.png)

![image](https://github.com/bogkofe/Kubernetes/blob/master/1.4/files/2.png)

# Задание 2 
- Создал отдельный Service приложения из Задания 1 с возможностью доступа снаружи кластера к nginx, используя тип NodePort
[Ссылка на yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/1.4/z2/service-z2.yaml)

- Демонстрация доступа  с помощью curl с локального компьютера
![image](https://github.com/bogkofe/Kubernetes/blob/master/1.4/files/3.png)

