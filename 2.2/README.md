## Домашнее задание к занятию «Хранение в K8s. Часть 2»

# Задание 1
- Создал  Deployment приложения, состоящего из контейнеров busybox и multitool
[Ссылка на yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/2.2/z1/deployment_z1.yaml)

- Создал PV и PVC для подключения папки на локальной ноде, которая будет использована в поде
[Ссылка на yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/2.2/z1/pv_z1.yaml)

[Ссылка на yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/2.2/z1/pvc_z1.yaml)

- Демонстрация, что multitool может читать файл, в который busybox пишет каждые пять секунд в общей директории

![image](https://github.com/bogkofe/Kubernetes/blob/master/2.2/files/1.png)

- Удалил Deployment и PVC

![image](https://github.com/bogkofe/Kubernetes/blob/master/2.2/files/2.png)

PV с политикой ReclaimPolicy "Retain" не удаляется автоматически после удаления PVC, что позволяет сохранить данные.

- Удалил и PV

![image](https://github.com/bogkofe/Kubernetes/blob/master/2.2/files/3.png)

Файл сохраняется на локальном диске ноды, так как PV использует hostPath

# Задание 2 
- Включил и настроил NFS-сервер на MicroK8S.

- Создал Deployment приложения состоящего из multitool, и подключил к нему PV, созданный автоматически на сервере NFS

[Ссылка на yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/2.2/z2/deployment_z2.yaml)

[Ссылка на yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/2.2/z2/pvc_z2.yaml)

[Ссылка на yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/2.2/z2/sc_z2.yaml)

![image](https://github.com/bogkofe/Kubernetes/blob/master/2.2/files/4.png)

- Демонстрация возможности чтения и записи файла изнутри пода
![image](https://github.com/bogkofe/Kubernetes/blob/master/2.2/files/5.png)
