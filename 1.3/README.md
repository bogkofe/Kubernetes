## Домашнее задание к занятию «Запуск приложений в K8S»

# Задание 1
- Создал Deployment приложения, состоящего из двух контейнеров — nginx и multitool
[Ссылка на yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/1.3/z1/deployment.yaml)

- Вывод до создания реплики и после

![image](https://github.com/bogkofe/Kubernetes/blob/master/1.3/files/1.png)

![image](https://github.com/bogkofe/Kubernetes/blob/master/1.3/files/2.png)

- Создал service, который обеспечит доступ до реплик приложений из п.1
[Ссылка на yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/1.3/z1/service.yaml)

- Создал отдельный Pod с приложением multitool
[Ссылка на yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/1.3/z1/multitool-pod.yaml)

- Убедился с помощью curl, что из пода есть доступ до приложений из п.1
![image](https://github.com/bogkofe/Kubernetes/blob/master/1.3/files/5.png)

# Задание 2 
- Создал Deployment приложения nginx с init контейнером busybox
[Ссылка на yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/1.3/z2/deployment2.yaml)

- Создал и запустил Service
[Ссылка на yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/1.3/z2/service2.yaml)

![image](https://github.com/bogkofe/Kubernetes/blob/master/1.3/files/z2.1.png)