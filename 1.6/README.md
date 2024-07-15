## Домашнее задание к занятию «Хранение в K8s. Часть 1»

# Задание 1
- Создал  Deployment приложения, состоящего из контейнеров busybox и multitool
[Ссылка на yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/1.6/z1/deployment_z1.yaml)

- Демонстрация что multitool может читать файл, который периодоически обновляется

![image](https://github.com/bogkofe/Kubernetes/blob/master/1.6/files/1.1.png)

![image](https://github.com/bogkofe/Kubernetes/blob/master/1.6/files/1.png)

# Задание 2 
- Создал DaemonSet приложения, состоящего из multitool
[Ссылка на yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/1.5/z2/ingress.yaml)

- Демонстрация возможности чтения файла /var/log/syslog кластера MicroK8S изнутри пода
![image](https://github.com/bogkofe/Kubernetes/blob/master/1.6/files/2.png)
