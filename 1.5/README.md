## Домашнее задание к занятию «Сетевое взаимодействие в K8S. Часть 1»

# Задание 1
- Создал  Deployment приложения frontend из образа nginx с количеством реплик 3 шт
[Ссылка на yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/1.5/z1/frontend-deployment.yaml)

- Создал   Deployment приложения backend из образа multitool.
[Ссылка на yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/1.5/z1/backend-deployment.yaml)

- Создал Service, которые обеспечат доступ к обоим приложениям внутри кластера
[Ссылка на frontend-service.yaml](https://github.com/bogkofe/Kubernetes/blob/master/1.5/z1/frontend-service.yaml)

[Ссылка на backend-service.yaml](https://github.com/bogkofe/Kubernetes/blob/master/1.5/z1/backend-service.yaml)

- Демонстрация что приложения видят друг друга с помощью Service

![image](https://github.com/bogkofe/Kubernetes/blob/master/1.5/files/1.png)

![image](https://github.com/bogkofe/Kubernetes/blob/master/1.5/files/2.png)

# Задание 2 
- Создал Создать Ingress, обеспечивающий доступ снаружи по IP-адресу кластера MicroK8S так, чтобы при запросе только по адресу открывался frontend а при добавлении /api - backend
[Ссылка на yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/1.5/z2/ingress.yaml)

- Демонстрация доступа с помощью браузера
![image](https://github.com/bogkofe/Kubernetes/blob/master/1.5/files/3.png)

![image](https://github.com/bogkofe/Kubernetes/blob/master/1.5/files/4.png)